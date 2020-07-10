_________________________________________________________________________________________________________
## For connecting to Kubernetes(k8s) via 
      FROM centos 
      RUN curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl

      RUN chmod +x kubectl
      RUN mv kubectl /usr/bin
      RUN mkdir /root/.kube/
      COPY /config /root/.kube/
      COPY /essentials/* /root/
      RUN yum install git -y
      RUN yum install java -y
      RUN yum install sudo -y
      RUN yum install openssh-server -y
      RUN mkdir /jenkins
      RUN ssh-keygen -A
      EXPOSE 22
      CMD ["/usr/sbin/sshd","-D"] && /bin/bash
_____________________________________________________________________________________________________________________________________________________________________
### The DOCKERFILE to expose HTTPD is:-

            FROM centos
            RUN yum install httpd -y
            RUN echo /usr/sbin/httpd >> /etc/bashrc
            COPY / /var/www/html/
            EXPOSE 80
      
### The config.YAML file can be seen as :-

            apiVersion: v1
            kind: Config

            clusters:
            - cluster:
                server: https://192.168.42.236:4243
                certificate-authority: /root/ca.crt
              name: kubecluster

            contexts:
            - context:
                cluster: kubecluster
                user: Vedant

            users:
            - name: Vedant
              user:
                client-key: /root/client.key
                client-certificate: /root/client.crt
