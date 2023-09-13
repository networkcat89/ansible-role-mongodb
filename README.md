# ansible_role_mongodb

Ansible role for mongodb installing without internet connections

adminDatabase:
  password: string # (default: undefined)

ansibleUser:
  password: string # (default: undefined)

mongodb_replicaset: enabled # (default: disabled) enable MongoDB replicaset cluster

mongoDatabase: # (default: undefined)
  - database: string # (default: undefined)\
    user: string # (default: undefined)\
    password: string # (default: undefined)\
    role: string # (default: undefined) ‘read’, ‘readWrite’, ‘dbAdmin’, ‘userAdmin’, ‘clusterAdmin’, ‘readAnyDatabase’, ‘readWriteAnyDatabase’, ‘userAdminAnyDatabase’, ‘dbAdminAnyDatabase’

Usage:

ansible-playbook mongo-deploy-configure.yml

