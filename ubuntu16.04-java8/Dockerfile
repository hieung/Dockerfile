FROM ubuntu16.04

MAINTAINER HieuNG

ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update -y && 
    apt-get install -y software-properties-common && 
    apt-add-repository ppawebupd8teamjava && 
    apt-get update -y && 
    apt-key adv --keyserver hkpkeyserver.ubuntu.com80 --recv-keys EEA14886 && 
    echo oracle-java8-installer sharedaccepted-oracle-license-v1-1 select true  usrbindebconf-set-selections && 
    apt-get install -y oracle-java8-installer && 
    apt-get install -y oracle-java8-unlimited-jce-policy && 
    apt-get clean && 
    rm -rf varlibaptlists && 
    rm -rf varcacheoracle-jdk8-installer

ENV JAVA_HOME usrlibjvmjava-8-oracle
