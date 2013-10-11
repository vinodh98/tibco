tibco
=====

test edit 1

# Tibco Demo Application

### Build the config file
./AppManage -export -out /opt/deploy/TIBCODemo.xml -ear /opt/deploy/TIBCODemo.ear

### Deploy the app
./AppManage -deploy -ear /opt/deploy/TIBCODemo.ear -app TIBCODemo -user admin -pw password -domain tibco_domain -deployConfig /opt/deploy/TIBCODemo.xml

### Buildear
./buildear -ear "/TIBCODemo.archive" -o "/opt/TIBCODemo.ear" -p "/opt/TIBCODemo/" -x -v -a /opt/jars/demo.conf

### TO export an exisitng app config
./AppManage -export -out /opt/myconf.xml -app TIBCODemo -user admin -pw password -domain tibco_domain

### Config xml
/opt/deploy/poi-3.7.1.jar:/opt/deploy/poi-3.9-20121203.jar:
