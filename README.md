# SAP-CODE-CHALLENGE-JUNE24-SAP-HANA-MULTIMODAL
Learnings and pointers from SAP Code Challenge Jun2024 - SAP HANA Multimodel

BAS - https://69e91dd6trial.us10cf.trial.applicationstudio.cloud.sap/index.html#ws-5j5mc
BTP-HANA-COCKPIT - https://69e91dd6trial.hana-tooling.ingress.orchestration.trial-us10.hanacloud.ondemand.com/hcs/sap/hana/cloud/index.html?#/&/databases/instance/3a1937b5-4d91-460b-81ea-727702c8872f/TwoColumnsMidExpanded/?tab=servicesSelection

DBADMIN PASS - VectorHanaCode@JUN2024

### 1.Basic BAS Commands - 
whoami
pwd
ls
hostname
echo ${WORKSPACE_ID}
clear

Check the available locale and set the missing values.
locale -a
export LC_ALL=C.utf8
locale

### 2. Install HANA in dev space 

https://github.com/sap-samples/sap-community-developer-challenge-hana-multimodel/blob/main/setup/setup.md#6-install-sap-hana-client-in-the-dev-space

### 3. COnfiguring BAS for HDB
HDB-ENDPOINT: 3a1937b5-4d91-460b-81ea-727702c8872f.hana.trial-us10.hanacloud.ondemand.com:443

~/sap/hdbclient/hdbuserstore -i SET myDBAdmin ${sap_hana_db_endpoint} DBAdmin:
~/sap/hdbclient/hdbuserstore -i SET myDBAdmin 3a1937b5-4d91-460b-81ea-727702c8872f.hana.trial-us10.hanacloud.ondemand.com:443 DBAdmin
~/sap/hdbclient/hdbuserstore -i SET myDevChallenger 3a1937b5-4d91-460b-81ea-727702c8872f.hana.trial-us10.hanacloud.ondemand.com:443 DevChallenger
DevChallenger-Up2TheChallenge!Iam

~/sap/hdbclient/hdbuserstore LIST
