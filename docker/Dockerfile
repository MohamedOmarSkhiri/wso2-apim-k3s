FROM wso2/wso2am:4.6.0

ARG USER_HOME=/home/wso2carbon
ARG WSO2_SERVER_NAME=wso2am
ARG WSO2_SERVER_VERSION=4.6.0
ARG WSO2_SERVER=${WSO2_SERVER_NAME}-${WSO2_SERVER_VERSION}
ARG WSO2_SERVER_HOME=${USER_HOME}/${WSO2_SERVER}

# Copy JDBC MySQL driver
COPY --chown=wso2carbon:wso2carbon mysql-connector-java-8.0.28.jar ${WSO2_SERVER_HOME}/repository/components/lib/
COPY --chown=wso2carbon:wso2carbon profileSetup.sh ${WSO2_SERVER_HOME}/bin

# version 1.0
