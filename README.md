# Stephane ROBERT ansible Core Snippets for Visual Studio Code

This Visual Studio Code extension provides snippets to help you write Ansible code faster.
It works like usual autocomplete : start typing to have suggestions or press 'CTRL+space' to force it.

You may find DevOps tips on my [own blog](https://blog.stephane-robert.info/).

[**You can support me on ko-fi**](https://ko-fi.com/stephanerobert89902)

![ansible snippets vscode](https://github.com/stephrobert/ansible-snippets/raw/main/img/sr-ansible-snippet.gif)


**Format :**

* **module** : Text to type

## `ansible.builtin` collection

* **ansible.builtin.add_host** : Add a host (and alternatively a group) to the ansible-playbook in-memory inventory
* **ansible.builtin.apt** : Manages apt-packages
* **ansible.builtin.apt_key** : Add or remove an apt key
* **ansible.builtin.apt_repository** : Add and remove APT repositories
* **ansible.builtin.assemble** : Assemble configuration files from fragments
* **ansible.builtin.assert** : Asserts given expressions are true
* **ansible.builtin.async_status** : Obtain status of asynchronous task
* **ansible.builtin.blockinfile** : Insert/update/remove a text block surrounded by marker lines
* **ansible.builtin.command** : Execute commands on targets
* **ansible.builtin.copy** : Copy files to remote locations
* **ansible.builtin.cron** : Manage cron.d and crontab entries
* **ansible.builtin.debconf** : Configure a .deb package
* **ansible.builtin.debug** : Print statements during execution
* **ansible.builtin.dnf** : Manages packages with the I(dnf) package manager
* **ansible.builtin.dpkg_selections** : Dpkg package selection selections
* **ansible.builtin.expect** : Executes a command and responds to prompts
* **ansible.builtin.fail** : Fail with custom message
* **ansible.builtin.fetch** : Fetch files from remote nodes
* **ansible.builtin.file** : Manage files and file properties
* **ansible.builtin.find** : Return a list of files based on specific criteria
* **ansible.builtin.setup** : Gathers facts about remote hosts
* **ansible.builtin.get_url** : Downloads files from HTTP, HTTPS, or FTP to node
* **ansible.builtin.getent** : A wrapper to the unix getent utility
* **ansible.builtin.git** : Deploy software (or files) from git checkouts
* **ansible.builtin.group** : Add or remove groups
* **ansible.builtin.group_by** : Create Ansible groups based on facts
* **ansible.builtin.hostname** : Manage hostname
* **ansible.builtin.import_playbook** : Import a playbook
* **ansible.builtin.import_role** : Import a role into a play
* **ansible.builtin.import_tasks** : Import a task list
* **ansible.builtin.include_role** : Load and execute a role
* **ansible.builtin.include_tasks** : Dynamically include a task list
* **ansible.builtin.include_vars** : Load variables from files, dynamically within a task
* **ansible.builtin.iptables** : Modify iptables rules
* **ansible.builtin.known_hosts** : Add or remove a host from the C(known_hosts) file
* **ansible.builtin.lineinfile** : Manage lines in text files
* **ansible.builtin.meta** : Execute Ansible &#39;actions&#39;
* **ansible.builtin.package** : Generic OS package manager
* **ansible.builtin.package_facts** : Package information as facts
* **ansible.builtin.pause** : Pause playbook execution
* **ansible.builtin.ping** : Try to connect to host, verify a usable python and return C(pong) on success
* **ansible.builtin.pip** : Manages Python library dependencies
* **ansible.builtin.raw** : Executes a low-down and dirty command
* **ansible.builtin.reboot** : Reboot a machine
* **ansible.builtin.replace** : Replace all instances of a particular string in a file using a back-referenced regular expression
* **ansible.builtin.rpm_key** : Adds or removes a gpg key from the rpm db
* **ansible.builtin.script** : Runs a local script on a remote node after transferring it
* **ansible.builtin.service** : Manage services
* **ansible.builtin.service_facts** : Return service state information as fact data
* **ansible.builtin.set_fact** : Set host variable(s) and fact(s).
* **ansible.builtin.set_stats** : Define and display stats for the current ansible run
* **ansible.builtin.shell** : Execute shell commands on targets
* **ansible.builtin.slurp** : Slurps a file from remote nodes
* **ansible.builtin.stat** : Retrieve file or file system status
* **ansible.builtin.subversion** : Deploys a subversion repository
* **ansible.builtin.systemd_service** : Manage systemd units
* **ansible.builtin.sysvinit** : Manage SysV services.
* **ansible.builtin.tempfile** : Creates temporary files and directories
* **ansible.builtin.template** : Template a file out to a target host
* **ansible.builtin.unarchive** : Unpacks an archive after (optionally) copying it from the local machine
* **ansible.builtin.uri** : Interacts with webservices
* **ansible.builtin.user** : Manage user accounts
* **ansible.builtin.validate_argument_spec** : Validate role argument specs.
* **ansible.builtin.wait_for** : Waits for a condition before continuing
* **ansible.builtin.wait_for_connection** : Waits until remote system is reachable/usable
* **ansible.builtin.yum** : Manages packages with the I(yum) package manager
* **ansible.builtin.yum_repository** : Add or remove YUM repositories

## `ansible.netcommon` collection

* **ansible.netcommon.cli_command** : Run a cli command on cli-based network devices
* **ansible.netcommon.cli_config** : Push text based configuration to network devices over network_cli
* **ansible.netcommon.grpc_get** : Fetch configuration/state data from gRPC enabled target hosts.
* **ansible.netcommon.net_get** : Copy a file from a network device to Ansible Controller
* **ansible.netcommon.net_ping** : Tests reachability using ping from a network device
* **ansible.netcommon.net_put** : Copy a file from Ansible Controller to a network device
* **ansible.netcommon.netconf_config** : netconf device configuration
* **ansible.netcommon.netconf_get** : Fetch configuration/state data from NETCONF enabled network devices.
* **ansible.netcommon.netconf_rpc** : Execute operations on NETCONF enabled network devices.
* **ansible.netcommon.network_resource** : Manage resource modules
* **ansible.netcommon.restconf_config** : Handles create, update, read and delete of configuration data on RESTCONF enabled devices.
* **ansible.netcommon.restconf_get** : Fetch configuration/state data from RESTCONF enabled devices.
* **ansible.netcommon.telnet** : Executes a low-down and dirty telnet command

## `ansible.posix` collection

* **ansible.posix.acl** : Set and retrieve file ACL information.
* **ansible.posix.at** : Schedule the execution of a command or script file via the at command
* **ansible.posix.authorized_key** : Adds or removes an SSH authorized key
* **ansible.posix.firewalld** : Manage arbitrary ports/services with firewalld
* **ansible.posix.firewalld_info** : Gather information about firewalld
* **ansible.posix.mount** : Control active and configured mount points
* **ansible.posix.patch** : Apply patch files using the GNU patch tool
* **ansible.posix.rhel_facts** : Facts module to set or override RHEL specific facts.
* **ansible.posix.rhel_rpm_ostree** : Ensure packages exist in a RHEL for Edge rpm-ostree based system
* **ansible.posix.rpm_ostree_upgrade** : Manage rpm-ostree upgrade transactions
* **ansible.posix.seboolean** : Toggles SELinux booleans
* **ansible.posix.selinux** : Change policy and state of SELinux
* **ansible.posix.synchronize** : A wrapper around rsync to make common tasks in your playbooks quick and easy
* **ansible.posix.sysctl** : Manage entries in sysctl.conf.

## `ansible.windows` collection

* **ansible.windows.async_status** : Obtain status of asynchronous task
* **ansible.windows.setup** : Gathers facts about remote hosts
* **ansible.windows.slurp** : Slurps a file from remote nodes
* **ansible.windows.win_acl** : Set file/directory/registry permissions for a system user or group
* **ansible.windows.win_acl_inheritance** : Change ACL inheritance
* **ansible.windows.win_certificate_store** : Manages the certificate store
* **ansible.windows.win_command** : Executes a command on a remote Windows node
* **ansible.windows.win_copy** : Copies files to remote locations on windows hosts
* **ansible.windows.win_dns_client** : Configures DNS lookup on Windows hosts
* **ansible.windows.win_domain** : Ensures the existence of a Windows domain
* **ansible.windows.win_domain_controller** : Manage domain controller/member server state for a Windows host
* **ansible.windows.win_domain_membership** : Manage domain/workgroup membership for a Windows host
* **ansible.windows.win_dsc** : Invokes a PowerShell DSC configuration
* **ansible.windows.win_environment** : Modify environment variables on windows hosts
* **ansible.windows.win_feature** : Installs and uninstalls Windows Features on Windows Server
* **ansible.windows.win_file** : Creates, touches or removes files or directories
* **ansible.windows.win_find** : Return a list of files based on specific criteria
* **ansible.windows.win_get_url** : Downloads file from HTTP, HTTPS, or FTP to node
* **ansible.windows.win_group** : Add and remove local groups
* **ansible.windows.win_group_membership** : Manage Windows local group membership
* **ansible.windows.win_hostname** : Manages local Windows computer name
* **ansible.windows.win_optional_feature** : Manage optional Windows features
* **ansible.windows.win_owner** : Set owner
* **ansible.windows.win_package** : Installs/uninstalls an installable package
* **ansible.windows.win_path** : Manage Windows path environment variables
* **ansible.windows.win_ping** : A windows version of the classic ping module
* **ansible.windows.win_powershell** : Run PowerShell scripts
* **ansible.windows.win_reboot** : Reboot a windows machine
* **ansible.windows.win_reg_stat** : Get information about Windows registry keys
* **ansible.windows.win_regedit** : Add, change, or remove registry keys and values
* **ansible.windows.win_service** : Manage and query Windows services
* **ansible.windows.win_service_info** : Gather information about Windows services
* **ansible.windows.win_share** : Manage Windows shares
* **ansible.windows.win_shell** : Execute shell commands on target hosts
* **ansible.windows.win_stat** : Get information about Windows files
* **ansible.windows.win_tempfile** : Creates temporary files and directories
* **ansible.windows.win_template** : Template a file out to a remote server
* **ansible.windows.win_updates** : Download and install Windows updates
* **ansible.windows.win_uri** : Interacts with webservices
* **ansible.windows.win_user** : Manages local Windows user accounts
* **ansible.windows.win_user_right** : Manage Windows User Rights
* **ansible.windows.win_wait_for** : Waits for a condition before continuing
* **ansible.windows.win_whoami** : Get information about the current user and process

## `community.general` collection

* **community.general.aerospike_migrations** : Check or wait for migrations between nodes
* **community.general.airbrake_deployment** : Notify airbrake about app deployments
* **community.general.aix_devices** : Manages AIX devices
* **community.general.aix_filesystem** : Configure LVM and NFS file systems for AIX
* **community.general.aix_inittab** : Manages the inittab on AIX
* **community.general.aix_lvg** : Manage LVM volume groups on AIX
* **community.general.aix_lvol** : Configure AIX LVM logical volumes
* **community.general.alerta_customer** : Manage customers in Alerta
* **community.general.ali_instance** : Create, Start, Stop, Restart or Terminate an Instance in ECS; Add or Remove Instance to/from a Security Group
* **community.general.ali_instance_info** : Gather information on instances of Alibaba Cloud ECS
* **community.general.alternatives** : Manages alternative programs for common commands
* **community.general.ansible_galaxy_install** : Install Ansible roles or collections using ansible-galaxy
* **community.general.apache2_mod_proxy** : Set and/or get members&#39; attributes of an Apache httpd 2.4 mod_proxy balancer pool
* **community.general.apache2_module** : Enables/disables a module of the Apache2 webserver
* **community.general.apk** : Manages apk packages
* **community.general.apt_repo** : Manage APT repositories via apt-repo
* **community.general.apt_rpm** : APT-RPM package manager
* **community.general.archive** : Creates a compressed archive of one or more files or trees
* **community.general.atomic_container** : Manage the containers on the atomic host platform
* **community.general.atomic_host** : Manage the atomic host platform
* **community.general.atomic_image** : Manage the container images on the atomic host platform
* **community.general.awall** : Manage awall policies
* **community.general.beadm** : Manage ZFS boot environments on FreeBSD/Solaris/illumos systems
* **community.general.bearychat** : Send BearyChat notifications
* **community.general.bigpanda** : Notify BigPanda about deployments
* **community.general.bitbucket_access_key** : Manages Bitbucket repository access keys
* **community.general.bitbucket_pipeline_key_pair** : Manages Bitbucket pipeline SSH key pair
* **community.general.bitbucket_pipeline_known_host** : Manages Bitbucket pipeline known hosts
* **community.general.bitbucket_pipeline_variable** : Manages Bitbucket pipeline variables
* **community.general.bower** : Manage bower packages with bower
* **community.general.bundler** : Manage Ruby Gem dependencies with Bundler
* **community.general.bzr** : Deploy software (or files) from bzr branches
* **community.general.campfire** : Send a message to Campfire
* **community.general.capabilities** : Manage Linux capabilities
* **community.general.cargo** : Manage Rust packages with cargo
* **community.general.catapult** : Send a sms / mms using the catapult bandwidth api
* **community.general.circonus_annotation** : Create an annotation in circonus
* **community.general.cisco_webex** : Send a message to a Cisco Webex Teams Room or Individual
* **community.general.clc_aa_policy** : Create or Delete Anti Affinity Policies at CenturyLink Cloud
* **community.general.clc_alert_policy** : Create or Delete Alert Policies at CenturyLink Cloud
* **community.general.clc_blueprint_package** : Deploys a blue print package on a set of servers in CenturyLink Cloud
* **community.general.clc_firewall_policy** : Create/delete/update firewall policies
* **community.general.clc_group** : Create/delete Server Groups at Centurylink Cloud
* **community.general.clc_loadbalancer** : Create, Delete shared loadbalancers in CenturyLink Cloud
* **community.general.clc_modify_server** : Modify servers in CenturyLink Cloud
* **community.general.clc_publicip** : Add and Delete public ips on servers in CenturyLink Cloud
* **community.general.clc_server** : Create, Delete, Start and Stop servers in CenturyLink Cloud
* **community.general.clc_server_snapshot** : Create, Delete and Restore server snapshots in CenturyLink Cloud
* **community.general.cloud_init_data_facts** : Retrieve facts of cloud-init
* **community.general.cloudflare_dns** : Manage Cloudflare DNS records
* **community.general.cobbler_sync** : Sync Cobbler
* **community.general.cobbler_system** : Manage system objects in Cobbler
* **community.general.composer** : Dependency Manager for PHP
* **community.general.consul** : Add, modify &amp; delete services within a consul cluster
* **community.general.consul_acl** : Manipulate Consul ACL keys and rules
* **community.general.consul_kv** : Manipulate entries in the key/value store of a consul cluster
* **community.general.consul_session** : Manipulate consul sessions
* **community.general.copr** : Manage one of the Copr repositories
* **community.general.cpanm** : Manages Perl library dependencies
* **community.general.cronvar** : Manage variables in crontabs
* **community.general.crypttab** : Encrypted Linux block devices
* **community.general.datadog_downtime** : Manages Datadog downtimes
* **community.general.datadog_event** : Posts events to Datadog  service
* **community.general.datadog_monitor** : Manages Datadog monitors
* **community.general.dconf** : Modify and read dconf database
* **community.general.deploy_helper** : Manages some of the steps common in deploying projects
* **community.general.dimensiondata_network** : Create, update, and delete MCP 1.0 &amp; 2.0 networks
* **community.general.dimensiondata_vlan** : Manage a VLAN in a Cloud Control network domain
* **community.general.discord** : Send Discord messages
* **community.general.django_manage** : Manages a Django application
* **community.general.dnf_versionlock** : Locks package versions in C(dnf) based systems
* **community.general.dnsimple** : Interface with dnsimple.com (a DNS hosting service)
* **community.general.dnsimple_info** : Pull basic info from DNSimple API
* **community.general.dnsmadeeasy** : Interface with dnsmadeeasy.com (a DNS hosting service)
* **community.general.dpkg_divert** : Override a debian package&#39;s version of a file
* **community.general.easy_install** : Installs Python libraries
* **community.general.ejabberd_user** : Manages users for ejabberd servers
* **community.general.elasticsearch_plugin** : Manage Elasticsearch plugins
* **community.general.emc_vnx_sg_member** : Manage storage group member on EMC VNX
* **community.general.etcd3** : Set or delete key value pairs from an etcd3 cluster
* **community.general.facter** : Runs the discovery program I(facter) on the remote system
* **community.general.filesize** : Create a file with a given size, or resize it if it exists
* **community.general.filesystem** : Makes a filesystem
* **community.general.flatpak** : Manage flatpaks
* **community.general.flatpak_remote** : Manage flatpak repository remotes
* **community.general.flowdock** : Send a message to a flowdock
* **community.general.gandi_livedns** : Manage Gandi LiveDNS records
* **community.general.gconftool2** : Edit GNOME Configurations
* **community.general.gconftool2_info** : Retrieve GConf configurations
* **community.general.gem** : Manage Ruby gems
* **community.general.git_config** : Read and write git configuration
* **community.general.github_deploy_key** : Manages deploy keys for GitHub repositories
* **community.general.github_issue** : View GitHub issue
* **community.general.github_key** : Manage GitHub access keys
* **community.general.github_release** : Interact with GitHub Releases
* **community.general.github_repo** : Manage your repositories on Github
* **community.general.github_webhook** : Manage GitHub webhooks
* **community.general.github_webhook_info** : Query information about GitHub webhooks
* **community.general.gitlab_branch** : Create or delete a branch
* **community.general.gitlab_deploy_key** : Manages GitLab project deploy keys
* **community.general.gitlab_group** : Creates/updates/deletes GitLab Groups
* **community.general.gitlab_group_members** : Manage group members on GitLab Server
* **community.general.gitlab_group_variable** : Creates, updates, or deletes GitLab groups variables
* **community.general.gitlab_hook** : Manages GitLab project hooks
* **community.general.gitlab_project** : Creates/updates/deletes GitLab Projects
* **community.general.gitlab_project_badge** : Manage project badges on GitLab Server
* **community.general.gitlab_project_members** : Manage project members on GitLab Server
* **community.general.gitlab_project_variable** : Creates/updates/deletes GitLab Projects Variables
* **community.general.gitlab_protected_branch** : Manage protection of existing branches
* **community.general.gitlab_runner** : Create, modify and delete GitLab Runners
* **community.general.gitlab_user** : Creates/updates/deletes/blocks/unblocks GitLab Users
* **community.general.grove** : Sends a notification to a grove.io channel
* **community.general.gunicorn** : Run gunicorn with various settings
* **community.general.hana_query** : Execute SQL on HANA
* **community.general.haproxy** : Enable, disable, and set weights for HAProxy backend servers using socket commands
* **community.general.heroku_collaborator** : Add or delete app collaborators on Heroku
* **community.general.hg** : Manages Mercurial (hg) repositories
* **community.general.hipchat** : Send a message to Hipchat
* **community.general.homebrew** : Package manager for Homebrew
* **community.general.homebrew_cask** : Install and uninstall homebrew casks
* **community.general.homebrew_tap** : Tap a Homebrew repository
* **community.general.homectl** : Manage user accounts with systemd-homed
* **community.general.honeybadger_deployment** : Notify Honeybadger.io about app deployments
* **community.general.hpilo_boot** : Boot system using specific media through HP iLO interface
* **community.general.hpilo_info** : Gather information through an HP iLO interface
* **community.general.hponcfg** : Configure HP iLO interface using hponcfg
* **community.general.htpasswd** : Manage user files for basic authentication
* **community.general.hwc_ecs_instance** : Creates a resource of Ecs/Instance in Huawei Cloud
* **community.general.hwc_evs_disk** : Creates a resource of Evs/Disk in Huawei Cloud
* **community.general.hwc_network_vpc** : Creates a Huawei Cloud VPC
* **community.general.hwc_smn_topic** : Creates a resource of SMNTopic in Huaweicloud Cloud
* **community.general.hwc_vpc_eip** : Creates a resource of Vpc/EIP in Huawei Cloud
* **community.general.hwc_vpc_peering_connect** : Creates a resource of Vpc/PeeringConnect in Huawei Cloud
* **community.general.hwc_vpc_port** : Creates a resource of Vpc/Port in Huawei Cloud
* **community.general.hwc_vpc_private_ip** : Creates a resource of Vpc/PrivateIP in Huawei Cloud
* **community.general.hwc_vpc_route** : Creates a resource of Vpc/Route in Huawei Cloud
* **community.general.hwc_vpc_security_group** : Creates a resource of Vpc/SecurityGroup in Huawei Cloud
* **community.general.hwc_vpc_security_group_rule** : Creates a resource of Vpc/SecurityGroupRule in Huawei Cloud
* **community.general.hwc_vpc_subnet** : Creates a resource of Vpc/Subnet in Huawei Cloud
* **community.general.ibm_sa_domain** : Manages domains on IBM Spectrum Accelerate Family storage systems
* **community.general.ibm_sa_host** : Adds hosts to or removes them from IBM Spectrum Accelerate Family storage systems
* **community.general.ibm_sa_host_ports** : Add host ports on IBM Spectrum Accelerate Family storage systems
* **community.general.ibm_sa_pool** : Handles pools on IBM Spectrum Accelerate Family storage systems
* **community.general.ibm_sa_vol** : Handle volumes on IBM Spectrum Accelerate Family storage systems
* **community.general.ibm_sa_vol_map** : Handles volume mapping on IBM Spectrum Accelerate Family storage systems
* **community.general.icinga2_feature** : Manage Icinga2 feature
* **community.general.icinga2_host** : Manage a host in Icinga2
* **community.general.idrac_redfish_command** : Manages Out-Of-Band controllers using iDRAC OEM Redfish APIs
* **community.general.idrac_redfish_config** : Manages servers through iDRAC using Dell Redfish APIs
* **community.general.idrac_redfish_info** : Gather PowerEdge server information through iDRAC using Redfish APIs
* **community.general.ilo_redfish_config** : Sets or updates configuration attributes on HPE iLO with Redfish OEM extensions
* **community.general.ilo_redfish_info** : Gathers server information through iLO using Redfish APIs
* **community.general.imc_rest** : Manage Cisco IMC hardware through its REST API
* **community.general.imgadm** : Manage SmartOS images
* **community.general.infinity** : Manage Infinity IPAM using Rest API
* **community.general.influxdb_database** : Manage InfluxDB databases
* **community.general.influxdb_query** : Query data points from InfluxDB
* **community.general.influxdb_retention_policy** : Manage InfluxDB retention policies
* **community.general.influxdb_user** : Manage InfluxDB users
* **community.general.influxdb_write** : Write data points into InfluxDB
* **community.general.ini_file** : Tweak settings in INI files
* **community.general.installp** : Manage packages on AIX
* **community.general.interfaces_file** : Tweak settings in /etc/network/interfaces files
* **community.general.ip_netns** : Manage network namespaces
* **community.general.ipa_config** : Manage Global FreeIPA Configuration Settings
* **community.general.ipa_dnsrecord** : Manage FreeIPA DNS records
* **community.general.ipa_dnszone** : Manage FreeIPA DNS Zones
* **community.general.ipa_group** : Manage FreeIPA group
* **community.general.ipa_hbacrule** : Manage FreeIPA HBAC rule
* **community.general.ipa_host** : Manage FreeIPA host
* **community.general.ipa_hostgroup** : Manage FreeIPA host-group
* **community.general.ipa_otpconfig** : Manage FreeIPA OTP Configuration Settings
* **community.general.ipa_otptoken** : Manage FreeIPA OTPs
* **community.general.ipa_pwpolicy** : Manage FreeIPA password policies
* **community.general.ipa_role** : Manage FreeIPA role
* **community.general.ipa_service** : Manage FreeIPA service
* **community.general.ipa_subca** : Manage FreeIPA Lightweight Sub Certificate Authorities
* **community.general.ipa_sudocmd** : Manage FreeIPA sudo command
* **community.general.ipa_sudocmdgroup** : Manage FreeIPA sudo command group
* **community.general.ipa_sudorule** : Manage FreeIPA sudo rule
* **community.general.ipa_user** : Manage FreeIPA users
* **community.general.ipa_vault** : Manage FreeIPA vaults
* **community.general.ipify_facts** : Retrieve the public IP of your internet gateway
* **community.general.ipinfoio_facts** : Retrieve IP geolocation facts of a host&#39;s IP address
* **community.general.ipmi_boot** : Management of order of boot devices
* **community.general.ipmi_power** : Power management for machine
* **community.general.iptables_state** : Save iptables state into a file or restore it from a file
* **community.general.ipwcli_dns** : Manage DNS Records for Ericsson IPWorks via ipwcli
* **community.general.irc** : Send a message to an IRC channel or a nick
* **community.general.iso_create** : Generate ISO file with specified files or folders
* **community.general.iso_customize** : Add/remove/change files in ISO file
* **community.general.iso_extract** : Extract files from an ISO image
* **community.general.jabber** : Send a message to jabber user or chat room
* **community.general.java_cert** : Uses keytool to import/remove certificate to/from java keystore (cacerts)
* **community.general.java_keystore** : Create a Java keystore in JKS format
* **community.general.jboss** : Deploy applications to JBoss
* **community.general.jenkins_build** : Manage jenkins builds
* **community.general.jenkins_job** : Manage jenkins jobs
* **community.general.jenkins_job_info** : Get information about Jenkins jobs
* **community.general.jenkins_plugin** : Add or remove Jenkins plugin
* **community.general.jenkins_script** : Executes a groovy script in the jenkins instance
* **community.general.jira** : Create and modify issues in a JIRA instance
* **community.general.kernel_blacklist** : Blacklist kernel modules
* **community.general.keycloak_authentication** : Configure authentication in Keycloak
* **community.general.keycloak_client** : Allows administration of Keycloak clients via Keycloak API
* **community.general.keycloak_client_rolemapping** : Allows administration of Keycloak client_rolemapping with the Keycloak API
* **community.general.keycloak_clientscope** : Allows administration of Keycloak client_scopes via Keycloak API
* **community.general.keycloak_clientsecret_info** : Retrieve client secret via Keycloak API
* **community.general.keycloak_clientsecret_regenerate** : Regenerate Keycloak client secret via Keycloak API
* **community.general.keycloak_clienttemplate** : Allows administration of Keycloak client templates via Keycloak API
* **community.general.keycloak_group** : Allows administration of Keycloak groups via Keycloak API
* **community.general.keycloak_identity_provider** : Allows administration of Keycloak identity providers via Keycloak API
* **community.general.keycloak_realm** : Allows administration of Keycloak realm via Keycloak API
* **community.general.keycloak_realm_info** : Allows obtaining Keycloak realm public information via Keycloak API
* **community.general.keycloak_role** : Allows administration of Keycloak roles via Keycloak API
* **community.general.keycloak_user_federation** : Allows administration of Keycloak user federations via Keycloak API
* **community.general.keycloak_user_rolemapping** : Allows administration of Keycloak user_rolemapping with the Keycloak API
* **community.general.keyring** : Set or delete a passphrase using the Operating System&#39;s native keyring
* **community.general.keyring_info** : Get a passphrase using the Operating System&#39;s native keyring
* **community.general.kibana_plugin** : Manage Kibana plugins
* **community.general.launchd** : Manage macOS services
* **community.general.layman** : Manage Gentoo overlays
* **community.general.lbu** : Local Backup Utility for Alpine Linux
* **community.general.ldap_attrs** : Add or remove multiple LDAP attribute values
* **community.general.ldap_entry** : Add or remove LDAP entries
* **community.general.ldap_passwd** : Set passwords in LDAP
* **community.general.ldap_search** : Search for entries in a LDAP server
* **community.general.librato_annotation** : Create an annotation in librato
* **community.general.linode** : Manage instances on the Linode Public Cloud
* **community.general.linode_v4** : Manage instances on the Linode cloud
* **community.general.listen_ports_facts** : Gather facts on processes listening on TCP and UDP ports
* **community.general.lldp** : Get details reported by lldp
* **community.general.locale_gen** : Creates or removes locales
* **community.general.logentries** : Module for tracking logs via logentries.com
* **community.general.logentries_msg** : Send a message to logentries
* **community.general.logstash_plugin** : Manage Logstash plugins
* **community.general.lvg** : Configure LVM volume groups
* **community.general.lvol** : Configure LVM logical volumes
* **community.general.lxc_container** : Manage LXC Containers
* **community.general.lxca_cmms** : Custom module for lxca cmms inventory utility
* **community.general.lxca_nodes** : Custom module for lxca nodes inventory utility
* **community.general.lxd_container** : Manage LXD instances
* **community.general.lxd_profile** : Manage LXD profiles
* **community.general.lxd_project** : Manage LXD projects
* **community.general.macports** : Package manager for MacPorts
* **community.general.mail** : Send an email
* **community.general.make** : Run targets in a Makefile
* **community.general.manageiq_alert_profiles** : Configuration of alert profiles for ManageIQ
* **community.general.manageiq_alerts** : Configuration of alerts in ManageIQ
* **community.general.manageiq_group** : Management of groups in ManageIQ
* **community.general.manageiq_policies** : Management of resource policy_profiles in ManageIQ
* **community.general.manageiq_policies_info** : Listing of resource policy_profiles in ManageIQ
* **community.general.manageiq_provider** : Management of provider in ManageIQ
* **community.general.manageiq_tags** : Management of resource tags in ManageIQ
* **community.general.manageiq_tags_info** : Retrieve resource tags in ManageIQ
* **community.general.manageiq_tenant** : Management of tenants in ManageIQ
* **community.general.manageiq_user** : Management of users in ManageIQ
* **community.general.mas** : Manage Mac App Store applications with mas-cli
* **community.general.matrix** : Send notifications to matrix
* **community.general.mattermost** : Send Mattermost notifications
* **community.general.maven_artifact** : Downloads an Artifact from a Maven Repository
* **community.general.memset_dns_reload** : Request reload of Memset&#39;s DNS infrastructure,
* **community.general.memset_memstore_info** : Retrieve Memstore product usage information
* **community.general.memset_server_info** : Retrieve server information
* **community.general.memset_zone** : Creates and deletes Memset DNS zones
* **community.general.memset_zone_domain** : Create and delete domains in Memset DNS zones
* **community.general.memset_zone_record** : Create and delete records in Memset DNS zones
* **community.general.mksysb** : Generates AIX mksysb rootvg backups
* **community.general.modprobe** : Load or unload kernel modules
* **community.general.monit** : Manage the state of a program monitored via Monit
* **community.general.mqtt** : Publish a message on an MQTT topic for the IoT
* **community.general.mssql_db** : Add or remove MSSQL databases from a remote host
* **community.general.mssql_script** : Execute SQL scripts on a MSSQL database
* **community.general.nagios** : Perform common tasks in Nagios related to downtime and notifications
* **community.general.netcup_dns** : Manage Netcup DNS records
* **community.general.newrelic_deployment** : Notify New Relic about app deployments
* **community.general.nexmo** : Send a SMS via nexmo
* **community.general.nginx_status_info** : Retrieve information on nginx status
* **community.general.nictagadm** : Manage nic tags on SmartOS systems
* **community.general.nmcli** : Manage Networking
* **community.general.nomad_job** : Launch a Nomad Job
* **community.general.nomad_job_info** : Get Nomad Jobs info
* **community.general.nosh** : Manage services with nosh
* **community.general.npm** : Manage node.js packages with npm
* **community.general.nsupdate** : Manage DNS records
* **community.general.ocapi_info** : Manages Out-Of-Band controllers using Open Composable API (OCAPI)
* **community.general.oci_vcn** : Manage Virtual Cloud Networks(VCN) in OCI
* **community.general.odbc** : Execute SQL via ODBC
* **community.general.office_365_connector_card** : Use webhooks to create Connector Card messages within an Office 365 group
* **community.general.ohai** : Returns inventory data from I(Ohai)
* **community.general.omapi_host** : Setup OMAPI hosts
* **community.general.one_host** : Manages OpenNebula Hosts
* **community.general.one_image** : Manages OpenNebula images
* **community.general.one_image_info** : Gather information on OpenNebula images
* **community.general.one_service** : Deploy and manage OpenNebula services
* **community.general.one_template** : Manages OpenNebula templates
* **community.general.one_vm** : Creates or terminates OpenNebula instances
* **community.general.oneandone_firewall_policy** : Configure 1&amp;1 firewall policy
* **community.general.oneandone_load_balancer** : Configure 1&amp;1 load balancer
* **community.general.oneandone_monitoring_policy** : Configure 1&amp;1 monitoring policy
* **community.general.oneandone_private_network** : Configure 1&amp;1 private networking
* **community.general.oneandone_public_ip** : Configure 1&amp;1 public IPs
* **community.general.oneandone_server** : Create, destroy, start, stop, and reboot a 1&amp;1 Host server
* **community.general.onepassword_info** : Gather items from 1Password
* **community.general.oneview_datacenter_info** : Retrieve information about the OneView Data Centers
* **community.general.oneview_enclosure_info** : Retrieve information about one or more Enclosures
* **community.general.oneview_ethernet_network** : Manage OneView Ethernet Network resources
* **community.general.oneview_ethernet_network_info** : Retrieve the information about one or more of the OneView Ethernet Networks
* **community.general.oneview_fc_network** : Manage OneView Fibre Channel Network resources
* **community.general.oneview_fc_network_info** : Retrieve the information about one or more of the OneView Fibre Channel Networks
* **community.general.oneview_fcoe_network** : Manage OneView FCoE Network resources
* **community.general.oneview_fcoe_network_info** : Retrieve the information about one or more of the OneView FCoE Networks
* **community.general.oneview_logical_interconnect_group** : Manage OneView Logical Interconnect Group resources
* **community.general.oneview_logical_interconnect_group_info** : Retrieve information about one or more of the OneView Logical Interconnect Groups
* **community.general.oneview_network_set** : Manage HPE OneView Network Set resources
* **community.general.oneview_network_set_info** : Retrieve information about the OneView Network Sets
* **community.general.oneview_san_manager** : Manage OneView SAN Manager resources
* **community.general.oneview_san_manager_info** : Retrieve information about one or more of the OneView SAN Managers
* **community.general.online_server_info** : Gather information about Online servers
* **community.general.online_user_info** : Gather information about Online user
* **community.general.open_iscsi** : Manage iSCSI targets with Open-iSCSI
* **community.general.openbsd_pkg** : Manage packages on OpenBSD
* **community.general.opendj_backendprop** : Will update the backend configuration of OpenDJ via the dsconfig set-backend-prop command
* **community.general.openwrt_init** : Manage services on OpenWrt
* **community.general.opkg** : Package manager for OpenWrt and Openembedded/Yocto based Linux distributions
* **community.general.osx_defaults** : Manage macOS user defaults
* **community.general.ovh_ip_failover** : Manage OVH IP failover address
* **community.general.ovh_ip_loadbalancing_backend** : Manage OVH IP LoadBalancing backends
* **community.general.ovh_monthly_billing** : Manage OVH monthly billing
* **community.general.pacemaker_cluster** : Manage pacemaker clusters
* **community.general.packet_device** : Manage a bare metal server in the Packet Host
* **community.general.packet_ip_subnet** : Assign IP subnet to a bare metal server
* **community.general.packet_project** : Create/delete a project in Packet host
* **community.general.packet_sshkey** : Create/delete an SSH key in Packet host
* **community.general.packet_volume** : Create/delete a volume in Packet host
* **community.general.packet_volume_attachment** : Attach/detach a volume to a device in the Packet host
* **community.general.pacman** : Manage packages with I(pacman)
* **community.general.pacman_key** : Manage pacman&#39;s list of trusted keys
* **community.general.pagerduty** : Create PagerDuty maintenance windows
* **community.general.pagerduty_alert** : Trigger, acknowledge or resolve PagerDuty incidents
* **community.general.pagerduty_change** : Track a code or infrastructure change as a PagerDuty change event
* **community.general.pagerduty_user** : Manage a user account on PagerDuty
* **community.general.pam_limits** : Modify Linux PAM limits
* **community.general.pamd** : Manage PAM Modules
* **community.general.parted** : Configure block device partitions
* **community.general.pear** : Manage pear/pecl packages
* **community.general.pids** : Retrieves process IDs list if the process is running otherwise return empty list
* **community.general.pingdom** : Pause/unpause Pingdom alerts
* **community.general.pip_package_info** : Pip package information
* **community.general.pipx** : Manages applications installed with pipx
* **community.general.pipx_info** : Rretrieves information about applications installed with pipx
* **community.general.pkg5** : Manages packages with the Solaris 11 Image Packaging System
* **community.general.pkg5_publisher** : Manages Solaris 11 Image Packaging System publishers
* **community.general.pkgin** : Package manager for SmartOS, NetBSD, et al
* **community.general.pkgng** : Package manager for FreeBSD &gt;= 9.0
* **community.general.pkgutil** : OpenCSW package management on Solaris
* **community.general.pmem** : Configure Intel Optane Persistent Memory modules
* **community.general.portage** : Package manager for Gentoo
* **community.general.portinstall** : Installing packages from FreeBSD&#39;s ports system
* **community.general.pritunl_org** : Manages Pritunl Organizations using the Pritunl API
* **community.general.pritunl_org_info** : List Pritunl Organizations using the Pritunl API
* **community.general.pritunl_user** : Manage Pritunl Users using the Pritunl API
* **community.general.pritunl_user_info** : List Pritunl Users using the Pritunl API
* **community.general.profitbricks** : Create, destroy, start, stop, and reboot a ProfitBricks virtual machine
* **community.general.profitbricks_datacenter** : Create or destroy a ProfitBricks Virtual Datacenter
* **community.general.profitbricks_nic** : Create or Remove a NIC
* **community.general.profitbricks_volume** : Create or destroy a volume
* **community.general.profitbricks_volume_attachments** : Attach or detach a volume
* **community.general.proxmox** : Management of instances in Proxmox VE cluster
* **community.general.proxmox_disk** : Management of a disk of a Qemu(KVM) VM in a Proxmox VE cluster
* **community.general.proxmox_domain_info** : Retrieve information about one or more Proxmox VE domains
* **community.general.proxmox_group_info** : Retrieve information about one or more Proxmox VE groups
* **community.general.proxmox_kvm** : Management of Qemu(KVM) Virtual Machines in Proxmox VE cluster
* **community.general.proxmox_nic** : Management of a NIC of a Qemu(KVM) VM in a Proxmox VE cluster
* **community.general.proxmox_snap** : Snapshot management of instances in Proxmox VE cluster
* **community.general.proxmox_storage_info** : Retrieve information about one or more Proxmox VE storages
* **community.general.proxmox_tasks_info** : Retrieve information about one or more Proxmox VE tasks
* **community.general.proxmox_template** : Management of OS templates in Proxmox VE cluster
* **community.general.proxmox_user_info** : Retrieve information about one or more Proxmox VE users
* **community.general.pubnub_blocks** : PubNub blocks management module
* **community.general.pulp_repo** : Add or remove Pulp repos from a remote host
* **community.general.puppet** : Runs puppet
* **community.general.pushbullet** : Sends notifications to Pushbullet
* **community.general.pushover** : Send notifications via U(https://pushover.net)
* **community.general.python_requirements_info** : Show python path and assert dependency versions
* **community.general.rax** : Create / delete an instance in Rackspace Public Cloud
* **community.general.rax_cbs** : Manipulate Rackspace Cloud Block Storage Volumes
* **community.general.rax_cbs_attachments** : Manipulate Rackspace Cloud Block Storage Volume Attachments
* **community.general.rax_cdb** : Create/delete or resize a Rackspace Cloud Databases instance
* **community.general.rax_cdb_database** : Create / delete a database in the Cloud Databases
* **community.general.rax_cdb_user** : Create / delete a Rackspace Cloud Database
* **community.general.rax_clb** : Create / delete a load balancer in Rackspace Public Cloud
* **community.general.rax_clb_nodes** : Add, modify and remove nodes from a Rackspace Cloud Load Balancer
* **community.general.rax_clb_ssl** : Manage SSL termination for a Rackspace Cloud Load Balancer
* **community.general.rax_dns** : Manage domains on Rackspace Cloud DNS
* **community.general.rax_dns_record** : Manage DNS records on Rackspace Cloud DNS
* **community.general.rax_facts** : Gather facts for Rackspace Cloud Servers
* **community.general.rax_files** : Manipulate Rackspace Cloud Files Containers
* **community.general.rax_files_objects** : Upload, download, and delete objects in Rackspace Cloud Files
* **community.general.rax_identity** : Load Rackspace Cloud Identity
* **community.general.rax_keypair** : Create a keypair for use with Rackspace Cloud Servers
* **community.general.rax_meta** : Manipulate metadata for Rackspace Cloud Servers
* **community.general.rax_mon_alarm** : Create or delete a Rackspace Cloud Monitoring alarm
* **community.general.rax_mon_check** : Create or delete a Rackspace Cloud Monitoring check for an existing entity.
* **community.general.rax_mon_entity** : Create or delete a Rackspace Cloud Monitoring entity
* **community.general.rax_mon_notification** : Create or delete a Rackspace Cloud Monitoring notification
* **community.general.rax_mon_notification_plan** : Create or delete a Rackspace Cloud Monitoring notification plan.
* **community.general.rax_network** : Create / delete an isolated network in Rackspace Public Cloud
* **community.general.rax_queue** : Create / delete a queue in Rackspace Public Cloud
* **community.general.rax_scaling_group** : Manipulate Rackspace Cloud Autoscale Groups
* **community.general.rax_scaling_policy** : Manipulate Rackspace Cloud Autoscale Scaling Policy
* **community.general.read_csv** : Read a CSV file
* **community.general.redfish_info** : Manages Out-Of-Band controllers using Redfish APIs
* **community.general.redhat_subscription** : Manage registration and subscriptions to RHSM using the C(subscription-manager) command
* **community.general.redis** : Various redis commands, replica and flush
* **community.general.redis_data** : Set key value pairs in Redis
* **community.general.redis_data_incr** : Increment keys in Redis
* **community.general.redis_data_info** : Get value of key in Redis database
* **community.general.redis_info** : Gather information about Redis servers
* **community.general.rhevm** : RHEV/oVirt automation
* **community.general.rhn_channel** : Adds or removes Red Hat software channels
* **community.general.rhn_register** : Manage Red Hat Network registration using the C(rhnreg_ks) command
* **community.general.rhsm_release** : Set or Unset RHSM Release version
* **community.general.rhsm_repository** : Manage RHSM repositories using the subscription-manager command
* **community.general.riak** : This module handles some common Riak operations
* **community.general.rocketchat** : Send notifications to Rocket Chat
* **community.general.rollbar_deployment** : Notify Rollbar about app deployments
* **community.general.rpm_ostree_pkg** : Install or uninstall overlay additional packages
* **community.general.rundeck_acl_policy** : Manage Rundeck ACL policies
* **community.general.rundeck_job_executions_info** : Query executions for a Rundeck job
* **community.general.rundeck_job_run** : Run a Rundeck job
* **community.general.rundeck_project** : Manage Rundeck projects
* **community.general.runit** : Manage runit services
* **community.general.sap_task_list_execute** : Perform SAP Task list execution
* **community.general.sapcar_extract** : Manages SAP SAPCAR archives
* **community.general.say** : Makes a computer to speak
* **community.general.scaleway_compute** : Scaleway compute management module
* **community.general.scaleway_compute_private_network** : Scaleway compute - private network management
* **community.general.scaleway_container** : Scaleway Container management
* **community.general.scaleway_container_info** : Retrieve information on Scaleway Container
* **community.general.scaleway_container_namespace** : Scaleway Container namespace management
* **community.general.scaleway_container_namespace_info** : Retrieve information on Scaleway Container namespace
* **community.general.scaleway_container_registry** : Scaleway Container registry management module
* **community.general.scaleway_container_registry_info** : Scaleway Container registry info module
* **community.general.scaleway_database_backup** : Scaleway database backups management module
* **community.general.scaleway_function** : Scaleway Function management
* **community.general.scaleway_function_info** : Retrieve information on Scaleway Function
* **community.general.scaleway_function_namespace** : Scaleway Function namespace management
* **community.general.scaleway_function_namespace_info** : Retrieve information on Scaleway Function namespace
* **community.general.scaleway_image_info** : Gather information about the Scaleway images available
* **community.general.scaleway_ip** : Scaleway IP management module
* **community.general.scaleway_ip_info** : Gather information about the Scaleway ips available
* **community.general.scaleway_lb** : Scaleway load-balancer management module
* **community.general.scaleway_organization_info** : Gather information about the Scaleway organizations available
* **community.general.scaleway_private_network** : Scaleway private network management
* **community.general.scaleway_security_group** : Scaleway Security Group management module
* **community.general.scaleway_security_group_info** : Gather information about the Scaleway security groups available
* **community.general.scaleway_security_group_rule** : Scaleway Security Group Rule management module
* **community.general.scaleway_server_info** : Gather information about the Scaleway servers available
* **community.general.scaleway_snapshot_info** : Gather information about the Scaleway snapshots available
* **community.general.scaleway_sshkey** : Scaleway SSH keys management module
* **community.general.scaleway_user_data** : Scaleway user_data management module
* **community.general.scaleway_volume** : Scaleway volumes management module
* **community.general.scaleway_volume_info** : Gather information about the Scaleway volumes available
* **community.general.sefcontext** : Manages SELinux file context mapping definitions
* **community.general.selinux_permissive** : Change permissive domain in SELinux policy
* **community.general.selogin** : Manages linux user to SELinux user mapping
* **community.general.sendgrid** : Sends an email with the SendGrid API
* **community.general.sensu_check** : Manage Sensu checks
* **community.general.sensu_client** : Manages Sensu client configuration
* **community.general.sensu_handler** : Manages Sensu handler configuration
* **community.general.sensu_silence** : Manage Sensu silence entries
* **community.general.sensu_subscription** : Manage Sensu subscriptions
* **community.general.seport** : Manages SELinux network port type definitions
* **community.general.serverless** : Manages a Serverless Framework project
* **community.general.shutdown** : Shut down a machine
* **community.general.sl_vm** : Create or cancel a virtual instance in SoftLayer
* **community.general.slack** : Send Slack notifications
* **community.general.slackpkg** : Package manager for Slackware &gt;= 12.2
* **community.general.smartos_image_info** : Get SmartOS image details
* **community.general.snap** : Manages snaps
* **community.general.snap_alias** : Manages snap aliases
* **community.general.snmp_facts** : Retrieve facts for a device using SNMP
* **community.general.solaris_zone** : Manage Solaris zones
* **community.general.sorcery** : Package manager for Source Mage GNU/Linux
* **community.general.spectrum_device** : Creates/deletes devices in CA Spectrum
* **community.general.spectrum_model_attrs** : Enforce a model&#39;s attributes in CA Spectrum
* **community.general.spotinst_aws_elastigroup** : Create, update or delete Spotinst AWS Elastigroups
* **community.general.ss_3par_cpg** : Manage HPE StoreServ 3PAR CPG
* **community.general.ssh_config** : Manage SSH config for user
* **community.general.stackdriver** : Send code deploy and annotation events to stackdriver
* **community.general.stacki_host** : Add or remove host to stacki front-end
* **community.general.statsd** : Send metrics to StatsD
* **community.general.statusio_maintenance** : Create maintenance windows for your status.io dashboard
* **community.general.sudoers** : Manage sudoers files
* **community.general.supervisorctl** : Manage the state of a program or group of programs running via supervisord
* **community.general.svc** : Manage daemontools services
* **community.general.svr4pkg** : Manage Solaris SVR4 packages
* **community.general.swdepot** : Manage packages with swdepot package manager (HP-UX)
* **community.general.swupd** : Manages updates and bundles in ClearLinux systems
* **community.general.syslogger** : Log messages in the syslog
* **community.general.syspatch** : Manage OpenBSD system patches
* **community.general.sysrc** : Manage FreeBSD using sysrc
* **community.general.sysupgrade** : Manage OpenBSD system upgrades
* **community.general.taiga_issue** : Creates/deletes an issue in a Taiga Project Management Platform
* **community.general.telegram** : Send notifications via telegram
* **community.general.terraform** : Manages a Terraform deployment (and plans)
* **community.general.timezone** : Configure timezone setting
* **community.general.twilio** : Sends a text message to a mobile phone through Twilio
* **community.general.typetalk** : Send a message to typetalk
* **community.general.udm_dns_record** : Manage dns entries on a univention corporate server
* **community.general.udm_dns_zone** : Manage dns zones on a univention corporate server
* **community.general.udm_group** : Manage of the posix group
* **community.general.udm_share** : Manage samba shares on a univention corporate server
* **community.general.udm_user** : Manage posix users on a univention corporate server
* **community.general.ufw** : Manage firewall with UFW
* **community.general.uptimerobot** : Pause and start Uptime Robot monitoring
* **community.general.urpmi** : Urpmi manager
* **community.general.utm_aaa_group** : Create, update or destroy an aaa group object in Sophos UTM
* **community.general.utm_aaa_group_info** : Get info for reverse_proxy frontend entry in Sophos UTM
* **community.general.utm_ca_host_key_cert** : Create, update or destroy ca host_key_cert entry in Sophos UTM
* **community.general.utm_ca_host_key_cert_info** : Get info for a ca host_key_cert entry in Sophos UTM
* **community.general.utm_dns_host** : Create, update or destroy dns entry in Sophos UTM
* **community.general.utm_network_interface_address** : Create, update or destroy network/interface_address object
* **community.general.utm_network_interface_address_info** : Get info for a network/interface_address object
* **community.general.utm_proxy_auth_profile** : Create, update or destroy reverse_proxy auth_profile entry in Sophos UTM
* **community.general.utm_proxy_exception** : Create, update or destroy reverse_proxy exception entry in Sophos UTM
* **community.general.utm_proxy_frontend_info** : Create, update or destroy reverse_proxy frontend entry in Sophos UTM
* **community.general.utm_proxy_location_info** : Create, update or destroy reverse_proxy location entry in Sophos UTM
* **community.general.vdo** : Module to control VDO
* **community.general.vertica_configuration** : Updates Vertica configuration parameters
* **community.general.vertica_info** : Gathers Vertica database facts
* **community.general.vertica_role** : Adds or removes Vertica database roles and assigns roles to them
* **community.general.vertica_schema** : Adds or removes Vertica database schema and roles
* **community.general.vertica_user** : Adds or removes Vertica database users and assigns roles
* **community.general.vexata_eg** : Manage export groups on Vexata VX100 storage arrays
* **community.general.vexata_volume** : Manage volumes on Vexata VX100 storage arrays
* **community.general.vmadm** : Manage SmartOS virtual machines and zones
* **community.general.wakeonlan** : Send a magic Wake-on-LAN (WoL) broadcast packet
* **community.general.wdc_redfish_info** : Manages WDC UltraStar Data102 Out-Of-Band controllers using Redfish APIs
* **community.general.webfaction_app** : Add or remove applications on a Webfaction host
* **community.general.webfaction_db** : Add or remove a database on Webfaction
* **community.general.webfaction_domain** : Add or remove domains and subdomains on Webfaction
* **community.general.webfaction_mailbox** : Add or remove mailboxes on Webfaction
* **community.general.webfaction_site** : Add or remove a website on a Webfaction host
* **community.general.xattr** : Manage user defined extended attributes
* **community.general.xbps** : Manage packages with XBPS
* **community.general.xcc_redfish_command** : Manages Lenovo Out-Of-Band controllers using Redfish APIs
* **community.general.xenserver_facts** : Get facts reported on xenserver
* **community.general.xenserver_guest** : Manages virtual machines running on Citrix Hypervisor/XenServer host or pool
* **community.general.xenserver_guest_info** : Gathers information for virtual machines running on Citrix Hypervisor/XenServer host or pool
* **community.general.xenserver_guest_powerstate** : Manages power states of virtual machines running on Citrix Hypervisor/XenServer host or pool
* **community.general.xfconf** : Edit XFCE4 Configurations
* **community.general.xfconf_info** : Retrieve XFCE4 configurations
* **community.general.xfs_quota** : Manage quotas on XFS filesystems
* **community.general.xml** : Manage bits and pieces of XML files or strings
* **community.general.yarn** : Manage node.js packages with Yarn
* **community.general.yum_versionlock** : Locks / unlocks a installed package(s) from being updated by yum package manager
* **community.general.zfs** : Manage zfs
* **community.general.zfs_delegate_admin** : Manage ZFS delegated administration (user admin privileges)
* **community.general.zfs_facts** : Gather facts about ZFS datasets
* **community.general.znode** : Create, delete, retrieve, and update znodes using ZooKeeper
* **community.general.zpool_facts** : Gather facts about ZFS pools
* **community.general.zypper** : Manage packages on SUSE and openSUSE
* **community.general.zypper_repository** : Add and remove Zypper repositories

## `community.crypto` collection

* **community.crypto.acme_account** : Create, modify or delete ACME accounts
* **community.crypto.acme_account_info** : Retrieves information on ACME accounts
* **community.crypto.acme_certificate** : Create SSL/TLS certificates with the ACME protocol
* **community.crypto.acme_certificate_revoke** : Revoke certificates with the ACME protocol
* **community.crypto.acme_challenge_cert_helper** : Prepare certificates required for ACME challenges such as C(tls-alpn-01)
* **community.crypto.acme_inspect** : Send direct requests to an ACME server
* **community.crypto.certificate_complete_chain** : Complete certificate chain given a set of untrusted and root certificates
* **community.crypto.crypto_info** : Retrieve cryptographic capabilities
* **community.crypto.ecs_certificate** : Request SSL/TLS certificates with the Entrust Certificate Services (ECS) API
* **community.crypto.ecs_domain** : Request validation of a domain with the Entrust Certificate Services (ECS) API
* **community.crypto.get_certificate** : Get a certificate from a host:port
* **community.crypto.luks_device** : Manage encrypted (LUKS) devices
* **community.crypto.openssh_cert** : Generate OpenSSH host or user certificates.
* **community.crypto.openssh_keypair** : Generate OpenSSH private and public keys
* **community.crypto.openssl_csr_pipe** : Generate OpenSSL Certificate Signing Request (CSR)
* **community.crypto.openssl_csr_info** : Provide information of OpenSSL Certificate Signing Requests (CSR)
* **community.crypto.openssl_dhparam** : Generate OpenSSL Diffie-Hellman Parameters
* **community.crypto.openssl_pkcs12** : Generate OpenSSL PKCS#12 archive
* **community.crypto.openssl_privatekey** : Generate OpenSSL private keys
* **community.crypto.openssl_privatekey_convert** : Convert OpenSSL private keys
* **community.crypto.openssl_privatekey_info** : Provide information for OpenSSL private keys
* **community.crypto.openssl_privatekey_pipe** : Generate OpenSSL private keys without disk access
* **community.crypto.openssl_publickey** : Generate an OpenSSL public key from its private key.
* **community.crypto.openssl_publickey_info** : Provide information for OpenSSL public keys
* **community.crypto.openssl_signature** : Sign data with openssl
* **community.crypto.openssl_signature_info** : Verify signatures with openssl
* **community.crypto.x509_certificate_pipe** : Generate and/or check OpenSSL certificates
* **community.crypto.x509_certificate_info** : Provide information of OpenSSL X.509 certificates
* **community.crypto.x509_crl** : Generate Certificate Revocation Lists (CRLs)
* **community.crypto.x509_crl_info** : Retrieve information on Certificate Revocation Lists (CRLs)

## `community.docker` collection

* **community.docker.current_container_facts** : Return facts about whether the module runs in a container
* **community.docker.docker_compose** : Manage multi-container Docker applications with Docker Compose.
* **community.docker.docker_config** : Manage docker configs.
* **community.docker.docker_container** : manage Docker containers
* **community.docker.docker_container_copy_into** : Copy a file into a Docker container
* **community.docker.docker_container_exec** : Execute command in a docker container
* **community.docker.docker_container_info** : Retrieves facts about docker container
* **community.docker.docker_host_info** : Retrieves facts about docker host and lists of objects of the services.
* **community.docker.docker_image** : Manage docker images
* **community.docker.docker_image_info** : Inspect docker images
* **community.docker.docker_image_load** : Load docker image(s) from archives
* **community.docker.docker_login** : Log into a Docker registry.
* **community.docker.docker_network** : Manage Docker networks
* **community.docker.docker_network_info** : Retrieves facts about docker network
* **community.docker.docker_node** : Manage Docker Swarm node
* **community.docker.docker_node_info** : Retrieves facts about docker swarm node from Swarm Manager
* **community.docker.docker_plugin** : Manage Docker plugins
* **community.docker.docker_prune** : Allows to prune various docker objects
* **community.docker.docker_secret** : Manage docker secrets.
* **community.docker.docker_stack** : docker stack module
* **community.docker.docker_stack_info** : Return information on a docker stack
* **community.docker.docker_stack_task_info** : Return information of the tasks on a docker stack
* **community.docker.docker_swarm** : Manage Swarm cluster
* **community.docker.docker_swarm_info** : Retrieves facts about Docker Swarm cluster.
* **community.docker.docker_swarm_service** : docker swarm service
* **community.docker.docker_swarm_service_info** : Retrieves information about docker services from a Swarm Manager
* **community.docker.docker_volume** : Manage Docker volumes
* **community.docker.docker_volume_info** : Retrieve facts about Docker volumes

## `kubernetes.core` collection

* **kubernetes.core.helm** : Manages Kubernetes packages with the Helm package manager
* **kubernetes.core.helm_info** : Get information from Helm package deployed inside the cluster
* **kubernetes.core.helm_plugin** : Manage Helm plugins
* **kubernetes.core.helm_plugin_info** : Gather information about Helm plugins
* **kubernetes.core.helm_pull** : download a chart from a repository and (optionally) unpack it in local directory.
* **kubernetes.core.helm_repository** : Manage Helm repositories.
* **kubernetes.core.helm_template** : Render chart templates
* **kubernetes.core.k8s** : Manage Kubernetes (K8s) objects
* **kubernetes.core.k8s_cluster_info** : Describe Kubernetes (K8s) cluster, APIs available and their respective versions
* **kubernetes.core.k8s_cp** : Copy files and directories to and from pod.
* **kubernetes.core.k8s_drain** : Drain, Cordon, or Uncordon node in k8s cluster
* **kubernetes.core.k8s_exec** : Execute command in Pod
* **kubernetes.core.k8s_info** : Describe Kubernetes (K8s) objects
* **kubernetes.core.k8s_json_patch** : Apply JSON patch operations to existing objects
* **kubernetes.core.k8s_log** : Fetch logs from Kubernetes resources
* **kubernetes.core.k8s_rollback** : Rollback Kubernetes (K8S) Deployments and DaemonSets
* **kubernetes.core.k8s_scale** : Set a new size for a Deployment, ReplicaSet, Replication Controller, or Job.
* **kubernetes.core.k8s_service** : Manage Services on Kubernetes
* **kubernetes.core.k8s_taint** : Taint a node in a Kubernetes/OpenShift cluster

## `community.mysql` collection

* **community.mysql.mysql_db** : Add or remove MySQL databases from a remote host
* **community.mysql.mysql_info** : Gather information about MySQL servers
* **community.mysql.mysql_query** : Run MySQL queries
* **community.mysql.mysql_replication** : Manage MySQL replication
* **community.mysql.mysql_role** : Adds, removes, or updates a MySQL role
* **community.mysql.mysql_user** : Adds or removes a user from a MySQL database
* **community.mysql.mysql_variables** : Manage MySQL global variables

## `community.postgresql` collection

* **community.postgresql.postgresql_copy** : Copy data between a file/program and a PostgreSQL table
* **community.postgresql.postgresql_db** : Add or remove PostgreSQL databases from a remote host
* **community.postgresql.postgresql_ext** : Add or remove PostgreSQL extensions from a database
* **community.postgresql.postgresql_idx** : Create or drop indexes from a PostgreSQL database
* **community.postgresql.postgresql_info** : Gather information about PostgreSQL servers
* **community.postgresql.postgresql_lang** : Adds, removes or changes procedural languages with a PostgreSQL database
* **community.postgresql.postgresql_membership** : Add or remove PostgreSQL roles from groups
* **community.postgresql.postgresql_owner** : Change an owner of PostgreSQL database object
* **community.postgresql.postgresql_pg_hba** : Add, remove or modify a rule in a pg_hba file
* **community.postgresql.postgresql_ping** : Check remote PostgreSQL server availability
* **community.postgresql.postgresql_privs** : Grant or revoke privileges on PostgreSQL database objects
* **community.postgresql.postgresql_publication** : Add, update, or remove PostgreSQL publication
* **community.postgresql.postgresql_query** : Run PostgreSQL queries
* **community.postgresql.postgresql_schema** : Add or remove PostgreSQL schema
* **community.postgresql.postgresql_script** : Run PostgreSQL statements from a file
* **community.postgresql.postgresql_sequence** : Create, drop, or alter a PostgreSQL sequence
* **community.postgresql.postgresql_set** : Change a PostgreSQL server configuration parameter
* **community.postgresql.postgresql_slot** : Add or remove replication slots from a PostgreSQL database
* **community.postgresql.postgresql_subscription** : Add, update, or remove PostgreSQL subscription
* **community.postgresql.postgresql_table** : Create, drop, or modify a PostgreSQL table
* **community.postgresql.postgresql_tablespace** : Add or remove PostgreSQL tablespaces from remote hosts
* **community.postgresql.postgresql_user** : Create, alter, or remove a user (role) from a PostgreSQL server instance
* **community.postgresql.postgresql_user_obj_stat_info** : Gather statistics about PostgreSQL user objects

