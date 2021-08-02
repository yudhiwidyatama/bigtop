FROM bigtop/puppet:1.4.0-centos-7
ADD startup.sh /startup.sh
ADD bigtop-puppet /bigtop-puppet
ADD bigtop-puppet/hiera.yaml /etc/puppet/hiera.yaml
ADD bigtop-puppet/hieradata /etc/puppet/hieradata
ADD site.yaml.template /etc/puppet/hieradata/site.yaml.template
RUN /startup.sh --bootstrap
CMD /startup.sh --foreground
