# Stephane ROBERT ansible Snippets for Visual Studio Code

This Visual Studio Code extension provides snippets to help you write Ansible code faster.
It works like usual autocomplete : start typing to have suggestions or press 'CTRL+space' to force it.

You may find DevOps tips on my [own blog](https://blog.stephane-robert.info/).

[**You can support me on ko-fi**](https://ko-fi.com/stephanerobert89902)

![ansible snippets vscode](https://github.com/stephrobert/ansible-snippets/raw/main/img/sr-ansible-snippet.gif)

- [Stephane ROBERT ansible Snippets for Visual Studio Code](#stephane-robert-ansible-snippets-for-visual-studio-code)
  - [`amazon.aws` collection](#amazonaws-collection)
  - [`ansible.builtin` collection](#ansiblebuiltin-collection)
  - [`ansible.netcommon` collection](#ansiblenetcommon-collection)
  - [`ansible.posix` collection](#ansibleposix-collection)
  - [`ansible.utils` collection](#ansibleutils-collection)
  - [`ansible.windows` collection](#ansiblewindows-collection)
  - [`arista.eos` collection](#aristaeos-collection)
  - [`awx.awx` collection](#awxawx-collection)
  - [`azure.azcollection` collection](#azureazcollection-collection)
  - [`check_point.mgmt` collection](#check_pointmgmt-collection)
  - [`chocolatey.chocolatey` collection](#chocolateychocolatey-collection)
  - [`cisco.aci` collection](#ciscoaci-collection)
  - [`cisco.asa` collection](#ciscoasa-collection)
  - [`cisco.dnac` collection](#ciscodnac-collection)
  - [`cisco.intersight` collection](#ciscointersight-collection)
  - [`cisco.ios` collection](#ciscoios-collection)
  - [`cisco.iosxr` collection](#ciscoiosxr-collection)
  - [`cisco.ise` collection](#ciscoise-collection)
  - [`cisco.meraki` collection](#ciscomeraki-collection)
  - [`cisco.mso` collection](#ciscomso-collection)
  - [`cisco.nso` collection](#cisconso-collection)
  - [`cisco.nxos` collection](#cisconxos-collection)
  - [`cisco.ucs` collection](#ciscoucs-collection)
  - [`cloud.common` collection](#cloudcommon-collection)
  - [`cloudscale_ch.cloud` collection](#cloudscale_chcloud-collection)
  - [`community.aws` collection](#communityaws-collection)
  - [`community.ciscosmb` collection](#communityciscosmb-collection)
  - [`community.crypto` collection](#communitycrypto-collection)
  - [`community.digitalocean` collection](#communitydigitalocean-collection)
  - [`community.dns` collection](#communitydns-collection)
  - [`community.docker` collection](#communitydocker-collection)
  - [`community.fortios` collection](#communityfortios-collection)
  - [`community.general` collection](#communitygeneral-collection)
  - [`community.google` collection](#communitygoogle-collection)
  - [`community.grafana` collection](#communitygrafana-collection)
  - [`community.hashi_vault` collection](#communityhashi_vault-collection)
  - [`community.hrobot` collection](#communityhrobot-collection)
  - [`community.libvirt` collection](#communitylibvirt-collection)
  - [`community.mongodb` collection](#communitymongodb-collection)
  - [`community.mysql` collection](#communitymysql-collection)
  - [`community.network` collection](#communitynetwork-collection)
  - [`community.okd` collection](#communityokd-collection)
  - [`community.postgresql` collection](#communitypostgresql-collection)
  - [`community.proxysql` collection](#communityproxysql-collection)
  - [`community.rabbitmq` collection](#communityrabbitmq-collection)
  - [`community.routeros` collection](#communityrouteros-collection)
  - [`community.sap` collection](#communitysap-collection)
  - [`community.sap_libs` collection](#communitysap_libs-collection)
  - [`community.skydive` collection](#communityskydive-collection)
  - [`community.sops` collection](#communitysops-collection)
  - [`community.vmware` collection](#communityvmware-collection)
  - [`community.windows` collection](#communitywindows-collection)
  - [`community.zabbix` collection](#communityzabbix-collection)
  - [`containers.podman` collection](#containerspodman-collection)
  - [`cyberark.pas` collection](#cyberarkpas-collection)
  - [`dellemc.enterprise_sonic` collection](#dellemcenterprise_sonic-collection)
  - [`dellemc.openmanage` collection](#dellemcopenmanage-collection)
  - [`dellemc.os10` collection](#dellemcos10-collection)
  - [`dellemc.os6` collection](#dellemcos6-collection)
  - [`dellemc.os9` collection](#dellemcos9-collection)
  - [`dellemc.powerflex` collection](#dellemcpowerflex-collection)
  - [`dellemc.unity` collection](#dellemcunity-collection)
  - [`f5networks.f5_modules` collection](#f5networksf5_modules-collection)
  - [`fortinet.fortimanager` collection](#fortinetfortimanager-collection)
  - [`fortinet.fortios` collection](#fortinetfortios-collection)
  - [`frr.frr` collection](#frrfrr-collection)
  - [`gluster.gluster` collection](#glustergluster-collection)
  - [`google.cloud` collection](#googlecloud-collection)
  - [`grafana.grafana` collection](#grafanagrafana-collection)
  - [`hetzner.hcloud` collection](#hetznerhcloud-collection)
  - [`hpe.nimble` collection](#hpenimble-collection)
  - [`ibm.qradar` collection](#ibmqradar-collection)
  - [`ibm.spectrum_virtualize` collection](#ibmspectrum_virtualize-collection)
  - [`infinidat.infinibox` collection](#infinidatinfinibox-collection)
  - [`infoblox.nios_modules` collection](#infobloxnios_modules-collection)
  - [`inspur.ispim` collection](#inspurispim-collection)
  - [`inspur.sm` collection](#inspursm-collection)
  - [`junipernetworks.junos` collection](#junipernetworksjunos-collection)
  - [`kubernetes.core` collection](#kubernetescore-collection)
  - [`lowlydba.sqlserver` collection](#lowlydbasqlserver-collection)
  - [`mellanox.onyx` collection](#mellanoxonyx-collection)
  - [`netapp.aws` collection](#netappaws-collection)
  - [`netapp.azure` collection](#netappazure-collection)
  - [`netapp.cloudmanager` collection](#netappcloudmanager-collection)
  - [`netapp.elementsw` collection](#netappelementsw-collection)
  - [`netapp.ontap` collection](#netappontap-collection)
  - [`netapp.storagegrid` collection](#netappstoragegrid-collection)
  - [`netapp.um_info` collection](#netappum_info-collection)
  - [`netapp_eseries.santricity` collection](#netapp_eseriessantricity-collection)
  - [`netbox.netbox` collection](#netboxnetbox-collection)
  - [`ngine_io.cloudstack` collection](#ngine_iocloudstack-collection)
  - [`ngine_io.exoscale` collection](#ngine_ioexoscale-collection)
  - [`ngine_io.vultr` collection](#ngine_iovultr-collection)
  - [`openstack.cloud` collection](#openstackcloud-collection)
  - [`openvswitch.openvswitch` collection](#openvswitchopenvswitch-collection)
  - [`ovirt.ovirt` collection](#ovirtovirt-collection)
  - [`purestorage.flasharray` collection](#purestorageflasharray-collection)
  - [`purestorage.flashblade` collection](#purestorageflashblade-collection)
  - [`purestorage.fusion` collection](#purestoragefusion-collection)
  - [`sensu.sensu_go` collection](#sensusensu_go-collection)
  - [`splunk.es` collection](#splunkes-collection)
  - [`t_systems_mms.icinga_director` collection](#t_systems_mmsicinga_director-collection)
  - [`theforeman.foreman` collection](#theforemanforeman-collection)
  - [`vmware.vmware_rest` collection](#vmwarevmware_rest-collection)
  - [`vultr.cloud` collection](#vultrcloud-collection)
  - [`vyos.vyos` collection](#vyosvyos-collection)
  - [`wti.remote` collection](#wtiremote-collection)

**Format :**

* **module** : Text to type

## `amazon.aws` collection

* **amazon.aws.autoscaling_group** : Create or delete AWS AutoScaling Groups (ASGs)
* **amazon.aws.autoscaling_group_info** : Gather information about EC2 Auto Scaling Groups (ASGs) in AWS
* **amazon.aws.aws_az_info** : Gather information about availability zones in AWS
* **amazon.aws.aws_caller_info** : Get information about the user and account being used to make AWS calls
* **amazon.aws.cloudformation** : Create or delete an AWS CloudFormation stack
* **amazon.aws.cloudformation_info** : Obtain information about an AWS CloudFormation stack
* **amazon.aws.cloudtrail** : manage CloudTrail create, delete, update
* **amazon.aws.cloudtrail_info** : Gather information about trails in AWS Cloud Trail.
* **amazon.aws.cloudwatch_metric_alarm** : Create/update or delete AWS CloudWatch &#39;metric alarms&#39;
* **amazon.aws.cloudwatch_metric_alarm_info** : Gather information about the alarms for the specified metric
* **amazon.aws.cloudwatchevent_rule** : Manage CloudWatch Event rules and targets
* **amazon.aws.cloudwatchlogs_log_group** : create or delete log_group in CloudWatchLogs
* **amazon.aws.cloudwatchlogs_log_group_info** : Get information about log_group in CloudWatchLogs
* **amazon.aws.cloudwatchlogs_log_group_metric_filter** : Manage CloudWatch log group metric filter
* **amazon.aws.ec2_ami** : Create or destroy an image (AMI) in EC2
* **amazon.aws.ec2_ami_info** : Gather information about ec2 AMIs
* **amazon.aws.ec2_eip** : manages EC2 elastic IP (EIP) addresses.
* **amazon.aws.ec2_eip_info** : List EC2 EIP details
* **amazon.aws.ec2_eni** : Create and optionally attach an Elastic Network Interface (ENI) to an instance
* **amazon.aws.ec2_eni_info** : Gather information about EC2 ENI interfaces in AWS
* **amazon.aws.ec2_instance** : Create &amp; manage EC2 instances
* **amazon.aws.ec2_instance_info** : Gather information about ec2 instances in AWS
* **amazon.aws.ec2_key** : Create or delete an EC2 key pair
* **amazon.aws.ec2_metadata_facts** : Gathers facts (instance metadata) about remote hosts within EC2
* **amazon.aws.ec2_security_group** : Maintain an EC2 security group
* **amazon.aws.ec2_security_group_info** : Gather information about EC2 security groups in AWS
* **amazon.aws.ec2_snapshot** : Creates a snapshot from an existing volume
* **amazon.aws.ec2_snapshot_info** : Gathers information about EC2 volume snapshots in AWS
* **amazon.aws.ec2_spot_instance** : Request, stop, reboot or cancel spot instance
* **amazon.aws.ec2_spot_instance_info** : Gather information about ec2 spot instance requests
* **amazon.aws.ec2_tag** : Create and remove tags on ec2 resources
* **amazon.aws.ec2_tag_info** : List tags on ec2 resources
* **amazon.aws.ec2_vol** : Create and attach a volume, return volume ID and device map
* **amazon.aws.ec2_vol_info** : Gather information about EC2 volumes in AWS
* **amazon.aws.ec2_vpc_dhcp_option** : Manages DHCP Options, and can ensure the DHCP options for the given VPC match what&#39;s requested
* **amazon.aws.ec2_vpc_dhcp_option_info** : Gather information about DHCP options sets in AWS
* **amazon.aws.ec2_vpc_endpoint** : Create and delete AWS VPC endpoints
* **amazon.aws.ec2_vpc_endpoint_info** : Retrieves AWS VPC endpoints details using AWS methods
* **amazon.aws.ec2_vpc_endpoint_service_info** : Retrieves AWS VPC endpoint service details
* **amazon.aws.ec2_vpc_igw** : Manage an AWS VPC Internet gateway
* **amazon.aws.ec2_vpc_igw_info** : Gather information about internet gateways in AWS
* **amazon.aws.ec2_vpc_nat_gateway** : Manage AWS VPC NAT Gateways
* **amazon.aws.ec2_vpc_nat_gateway_info** : Retrieves AWS VPC Managed Nat Gateway details using AWS methods
* **amazon.aws.ec2_vpc_net** : Configure AWS Virtual Private Clouds
* **amazon.aws.ec2_vpc_net_info** : Gather information about ec2 VPCs in AWS
* **amazon.aws.ec2_vpc_route_table** : Manage route tables for AWS Virtual Private Clouds
* **amazon.aws.ec2_vpc_route_table_info** : Gather information about ec2 VPC route tables in AWS
* **amazon.aws.ec2_vpc_subnet** : Manage subnets in AWS virtual private clouds
* **amazon.aws.ec2_vpc_subnet_info** : Gather information about ec2 VPC subnets in AWS
* **amazon.aws.elb_application_lb** : Manage an Application Load Balancer
* **amazon.aws.elb_application_lb_info** : Gather information about Application Load Balancers in AWS
* **amazon.aws.elb_classic_lb** : Creates, updates or destroys an Amazon ELB
* **amazon.aws.iam_policy** : Manage inline IAM policies for users, groups, and roles
* **amazon.aws.iam_policy_info** : Retrieve inline IAM policies for users, groups, and roles
* **amazon.aws.iam_user** : Manage AWS IAM users
* **amazon.aws.iam_user_info** : Gather IAM user(s) facts in AWS
* **amazon.aws.kms_key** : Perform various KMS key management tasks
* **amazon.aws.kms_key_info** : Gather information about AWS KMS keys
* **amazon.aws.lambda** : Manage AWS Lambda functions
* **amazon.aws.lambda_alias** : Creates, updates or deletes AWS Lambda function aliases
* **amazon.aws.lambda_event** : Creates, updates or deletes AWS Lambda function event mappings
* **amazon.aws.lambda_execute** : Execute an AWS Lambda function
* **amazon.aws.lambda_info** : Gathers AWS Lambda function details
* **amazon.aws.lambda_policy** : Creates, updates or deletes AWS Lambda policy statements.
* **amazon.aws.rds_cluster** : rds_cluster module
* **amazon.aws.rds_cluster_info** : Obtain information about one or more RDS clusters
* **amazon.aws.rds_cluster_snapshot** : Manage Amazon RDS snapshots of DB clusters
* **amazon.aws.rds_instance** : Manage RDS instances
* **amazon.aws.rds_instance_info** : obtain information about one or more RDS instances
* **amazon.aws.rds_instance_snapshot** : Manage Amazon RDS instance snapshots
* **amazon.aws.rds_option_group** : Manages the creation, modification, deletion of RDS option groups
* **amazon.aws.rds_option_group_info** : rds_option_group_info module
* **amazon.aws.rds_param_group** : manage RDS parameter groups
* **amazon.aws.rds_snapshot_info** : obtain information about one or more RDS snapshots
* **amazon.aws.rds_subnet_group** : manage RDS database subnet groups
* **amazon.aws.route53** : add or delete entries in Amazons Route 53 DNS service
* **amazon.aws.route53_health_check** : Manage health-checks in Amazons Route53 DNS service
* **amazon.aws.route53_info** : Retrieves route53 details using AWS methods
* **amazon.aws.route53_zone** : add or delete Route53 zones
* **amazon.aws.s3_bucket** : Manage S3 buckets in AWS, DigitalOcean, Ceph, Walrus, FakeS3 and StorageGRID
* **amazon.aws.s3_object** : Manage objects in S3
* **amazon.aws.s3_object_info** : Gather information about objects in S3

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

## `ansible.utils` collection

* **ansible.utils.cli_parse** : Parse cli output or text using a variety of parsers
* **ansible.utils.fact_diff** : Find the difference between currently set facts
* **ansible.utils.update_fact** : Update currently set facts
* **ansible.utils.validate** : Validate data with provided criteria

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

## `arista.eos` collection

* **arista.eos.eos_acl_interfaces** : ACL interfaces resource module
* **arista.eos.eos_acls** : ACLs resource module
* **arista.eos.eos_banner** : Manage multiline banners on Arista EOS devices
* **arista.eos.eos_bgp_address_family** : Manages BGP address family resource module
* **arista.eos.eos_bgp_global** : Manages BGP global resource module
* **arista.eos.eos_command** : Run arbitrary commands on an Arista EOS device
* **arista.eos.eos_config** : Manage Arista EOS configuration sections
* **arista.eos.eos_eapi** : Manage and configure Arista EOS eAPI.
* **arista.eos.eos_facts** : Collect facts from remote devices running Arista EOS
* **arista.eos.eos_hostname** : Manages hostname resource module
* **arista.eos.eos_interfaces** : Interfaces resource module
* **arista.eos.eos_l2_interfaces** : L2 interfaces resource module
* **arista.eos.eos_l3_interfaces** : L3 interfaces resource module
* **arista.eos.eos_lacp** : LACP resource module
* **arista.eos.eos_lacp_interfaces** : LACP interfaces resource module
* **arista.eos.eos_lag_interfaces** : LAG interfaces resource module
* **arista.eos.eos_lldp** : Manage LLDP configuration on Arista EOS network devices
* **arista.eos.eos_lldp_global** : LLDP resource module
* **arista.eos.eos_lldp_interfaces** : LLDP interfaces resource module
* **arista.eos.eos_logging_global** : Manages logging resource module
* **arista.eos.eos_ntp_global** : Manages ntp resource module
* **arista.eos.eos_ospf_interfaces** : OSPF Interfaces Resource Module.
* **arista.eos.eos_ospfv2** : OSPFv2 resource module
* **arista.eos.eos_ospfv3** : OSPFv3 resource module
* **arista.eos.eos_prefix_lists** : Manages Prefix lists resource module
* **arista.eos.eos_route_maps** : Manages Route Maps resource module
* **arista.eos.eos_snmp_server** : Manages snmp_server resource module
* **arista.eos.eos_static_routes** : Static routes resource module
* **arista.eos.eos_system** : Manage the system attributes on Arista EOS devices
* **arista.eos.eos_user** : Manage the collection of local users on EOS devices
* **arista.eos.eos_vlans** : VLANs resource module
* **arista.eos.eos_vrf** : Manage VRFs on Arista EOS network devices

## `awx.awx` collection

* **awx.awx.ad_hoc_command** : create, update, or destroy Automation Platform Controller ad hoc commands.
* **awx.awx.ad_hoc_command_cancel** : Cancel an Ad Hoc Command.
* **awx.awx.ad_hoc_command_wait** : Wait for Automation Platform Controller Ad Hoc Command to finish.
* **awx.awx.application** : create, update, or destroy Automation Platform Controller applications
* **awx.awx.controller_meta** : Returns metadata about the collection this module lives in.
* **awx.awx.credential** : create, update, or destroy Automation Platform Controller credential.
* **awx.awx.credential_input_source** : create, update, or destroy Automation Platform Controller credential input sources.
* **awx.awx.credential_type** : Create, update, or destroy custom Automation Platform Controller credential type.
* **awx.awx.execution_environment** : create, update, or destroy Execution Environments in Automation Platform Controller.
* **awx.awx.export** : export resources from Automation Platform Controller.
* **awx.awx.group** : create, update, or destroy Automation Platform Controller group.
* **awx.awx.host** : create, update, or destroy Automation Platform Controller host.
* **awx.awx.import** : import resources into Automation Platform Controller.
* **awx.awx.instance** : create, update, or destroy Automation Platform Controller instances.
* **awx.awx.instance_group** : create, update, or destroy Automation Platform Controller instance groups.
* **awx.awx.inventory** : create, update, or destroy Automation Platform Controller inventory.
* **awx.awx.inventory_source** : create, update, or destroy Automation Platform Controller inventory source.
* **awx.awx.inventory_source_update** : Update inventory source(s).
* **awx.awx.job_cancel** : Cancel an Automation Platform Controller Job.
* **awx.awx.job_launch** : Launch an Ansible Job.
* **awx.awx.job_list** : List Automation Platform Controller jobs.
* **awx.awx.job_template** : create, update, or destroy Automation Platform Controller job templates.
* **awx.awx.job_wait** : Wait for Automation Platform Controller job to finish.
* **awx.awx.label** : create, update, or destroy Automation Platform Controller labels.
* **awx.awx.license** : Set the license for Automation Platform Controller
* **awx.awx.notification_template** : create, update, or destroy Automation Platform Controller notification.
* **awx.awx.organization** : create, update, or destroy Automation Platform Controller organizations
* **awx.awx.project** : create, update, or destroy Automation Platform Controller projects
* **awx.awx.project_update** : Update a Project in Automation Platform Controller
* **awx.awx.role** : grant or revoke an Automation Platform Controller role.
* **awx.awx.schedule** : create, update, or destroy Automation Platform Controller schedules.
* **awx.awx.settings** : Modify Automation Platform Controller settings.
* **awx.awx.subscriptions** : Get subscription list
* **awx.awx.team** : create, update, or destroy Automation Platform Controller team.
* **awx.awx.token** : create, update, or destroy Automation Platform Controller tokens.
* **awx.awx.user** : create, update, or destroy Automation Platform Controller users.
* **awx.awx.workflow_approval** : Approve an approval node in a workflow job.
* **awx.awx.workflow_job_template** : create, update, or destroy Automation Platform Controller workflow job templates.
* **awx.awx.workflow_job_template_node** : create, update, or destroy Automation Platform Controller workflow job template nodes.
* **awx.awx.workflow_launch** : Run a workflow in Automation Platform Controller
* **awx.awx.workflow_node_wait** : Wait for a workflow node to finish.

## `azure.azcollection` collection

* **azure.azcollection.azure_rm_account_info** : Get Azure Account facts (output of az account show)
* **azure.azcollection.azure_rm_adapplication** : Manage Azure Active Directory application
* **azure.azcollection.azure_rm_adapplication_info** : Get Azure Active Directory application info
* **azure.azcollection.azure_rm_adgroup** : Manage Azure Active Directory group
* **azure.azcollection.azure_rm_adgroup_info** : Get Azure Active Directory group info
* **azure.azcollection.azure_rm_adpassword** : Manage application password
* **azure.azcollection.azure_rm_adpassword_info** : Get application password info
* **azure.azcollection.azure_rm_adserviceprincipal** : Manage Azure Active Directory service principal
* **azure.azcollection.azure_rm_adserviceprincipal_info** : Get Azure Active Directory service principal info
* **azure.azcollection.azure_rm_aduser** : Modify an Azure Active Directory user
* **azure.azcollection.azure_rm_aduser_info** : Get Azure Active Directory user info
* **azure.azcollection.azure_rm_aks** : Manage a managed Azure Container Service (AKS) instance
* **azure.azcollection.azure_rm_aks_info** : Get Azure Kubernetes Service facts
* **azure.azcollection.azure_rm_aksagentpool** : Manage node pools in Kubernetes kubernetes cluster
* **azure.azcollection.azure_rm_aksagentpool_info** : Show the details for a node pool in the managed Kubernetes cluster
* **azure.azcollection.azure_rm_aksagentpoolversion_info** : Gets a list of supported versions for the specified agent pool
* **azure.azcollection.azure_rm_aksupgrade_info** : Get the upgrade versions available for a AKS instance
* **azure.azcollection.azure_rm_aksversion_info** : Get available kubernetes versions supported by Azure Kubernetes Service
* **azure.azcollection.azure_rm_apimanagement** : Manage Azure api instances
* **azure.azcollection.azure_rm_apimanagement_info** : Get the infomation of the API Instance
* **azure.azcollection.azure_rm_apimanagementservice** : Manage Azure ApiManagementService instance
* **azure.azcollection.azure_rm_apimanagementservice_info** : Get ApiManagementService info
* **azure.azcollection.azure_rm_appgateway** : Manage Application Gateway instance
* **azure.azcollection.azure_rm_appgateway_info** : Retrieve Application Gateway instance facts
* **azure.azcollection.azure_rm_applicationsecuritygroup** : Manage Azure Application Security Group
* **azure.azcollection.azure_rm_applicationsecuritygroup_info** : Get Azure Application Security Group facts
* **azure.azcollection.azure_rm_appserviceplan** : Manage App Service Plan
* **azure.azcollection.azure_rm_appserviceplan_info** : Get azure app service plan facts
* **azure.azcollection.azure_rm_automationaccount** : Manage Azure Automation account
* **azure.azcollection.azure_rm_automationaccount_info** : Get Azure automation account facts
* **azure.azcollection.azure_rm_automationrunbook** : Mange automation runbook
* **azure.azcollection.azure_rm_automationrunbook_info** : Get Azure automation runbook facts
* **azure.azcollection.azure_rm_autoscale** : Manage Azure autoscale setting
* **azure.azcollection.azure_rm_autoscale_info** : Get Azure Auto Scale Setting facts
* **azure.azcollection.azure_rm_availabilityset** : Manage Azure Availability Set
* **azure.azcollection.azure_rm_availabilityset_info** : Get Azure Availability Set facts
* **azure.azcollection.azure_rm_azurefirewall** : Manage Azure Firewall instance
* **azure.azcollection.azure_rm_azurefirewall_info** : Get AzureFirewall info
* **azure.azcollection.azure_rm_backupazurevm** : Back up an Azure Virtual Machine using Azure Backup
* **azure.azcollection.azure_rm_backupazurevm_info** : Back up an Azure Virtual Machine using Azure Backup Information
* **azure.azcollection.azure_rm_backuppolicy** : Manage Azure Backup Policy
* **azure.azcollection.azure_rm_backuppolicy_info** : Get Info on Azure Backup Policy
* **azure.azcollection.azure_rm_bastionhost** : Managed bastion host resource
* **azure.azcollection.azure_rm_bastionhost_info** : Get Azure bastion host info
* **azure.azcollection.azure_rm_batchaccount** : Manages a Batch Account on Azure
* **azure.azcollection.azure_rm_cdnendpoint** : Manage a Azure CDN endpoint
* **azure.azcollection.azure_rm_cdnendpoint_info** : Get Azure CDN endpoint facts
* **azure.azcollection.azure_rm_cdnprofile** : Manage a Azure CDN profile
* **azure.azcollection.azure_rm_cdnprofile_info** : Get Azure CDN profile facts
* **azure.azcollection.azure_rm_cognitivesearch** : Manage Azure Cognitive Search service
* **azure.azcollection.azure_rm_cognitivesearch_info** : Get Azure Cognitive Search service info
* **azure.azcollection.azure_rm_containerinstance** : Manage an Azure Container Instance
* **azure.azcollection.azure_rm_containerinstance_info** : Get Azure Container Instance facts
* **azure.azcollection.azure_rm_containerregistry** : Manage an Azure Container Registry
* **azure.azcollection.azure_rm_containerregistry_info** : Get Azure Container Registry facts
* **azure.azcollection.azure_rm_containerregistryreplication** : Manage Replication instance.
* **azure.azcollection.azure_rm_containerregistryreplication_info** : Get Replication facts.
* **azure.azcollection.azure_rm_containerregistrytag** : Import or delete tags in Azure Container Registry
* **azure.azcollection.azure_rm_containerregistrytag_info** : Get Azure Container Registry tag facts
* **azure.azcollection.azure_rm_containerregistrywebhook** : Manage Webhook instance.
* **azure.azcollection.azure_rm_containerregistrywebhook_info** : Get Webhook facts.
* **azure.azcollection.azure_rm_cosmosdbaccount** : Manage Azure Database Account instance
* **azure.azcollection.azure_rm_cosmosdbaccount_info** : Get Azure Cosmos DB Account facts
* **azure.azcollection.azure_rm_datafactory** : Managed data factory
* **azure.azcollection.azure_rm_datafactory_info** : Get data factory facts
* **azure.azcollection.azure_rm_datalakestore** : Manage Azure data lake store
* **azure.azcollection.azure_rm_datalakestore_info** : Get Azure Data Lake Store info
* **azure.azcollection.azure_rm_ddosprotectionplan** : Manage DDoS protection plan
* **azure.azcollection.azure_rm_ddosprotectionplan_info** : Get Azure DDoS protection plan
* **azure.azcollection.azure_rm_deployment** : Create or destroy Azure Resource Manager template deployments
* **azure.azcollection.azure_rm_deployment_info** : Get Azure Deployment facts
* **azure.azcollection.azure_rm_devtestlab** : Manage Azure DevTest Lab instance
* **azure.azcollection.azure_rm_devtestlab_info** : Get Azure DevTest Lab facts
* **azure.azcollection.azure_rm_devtestlabarmtemplate_info** : Get Azure DevTest Lab ARM Template facts
* **azure.azcollection.azure_rm_devtestlabartifact_info** : Get Azure DevTest Lab Artifact facts
* **azure.azcollection.azure_rm_devtestlabartifactsource** : Manage Azure DevTest Labs Artifacts Source instance
* **azure.azcollection.azure_rm_devtestlabartifactsource_info** : Get Azure DevTest Lab Artifact Source facts
* **azure.azcollection.azure_rm_devtestlabcustomimage** : Manage Azure DevTest Lab Custom Image instance
* **azure.azcollection.azure_rm_devtestlabcustomimage_info** : Get Azure DevTest Lab Custom Image facts
* **azure.azcollection.azure_rm_devtestlabenvironment** : Manage Azure DevTest Lab Environment instance
* **azure.azcollection.azure_rm_devtestlabenvironment_info** : Get Azure Environment facts
* **azure.azcollection.azure_rm_devtestlabpolicy** : Manage Azure Policy instance
* **azure.azcollection.azure_rm_devtestlabpolicy_info** : Get Azure DTL Policy facts
* **azure.azcollection.azure_rm_devtestlabschedule** : Manage Azure DevTest Lab Schedule instance
* **azure.azcollection.azure_rm_devtestlabschedule_info** : Get Azure Schedule facts
* **azure.azcollection.azure_rm_devtestlabvirtualmachine** : Manage Azure DevTest Lab Virtual Machine instance
* **azure.azcollection.azure_rm_devtestlabvirtualmachine_info** : Get Azure DevTest Lab Virtual Machine facts
* **azure.azcollection.azure_rm_devtestlabvirtualnetwork** : Manage Azure DevTest Lab Virtual Network instance
* **azure.azcollection.azure_rm_devtestlabvirtualnetwork_info** : Get Azure DevTest Lab Virtual Network facts
* **azure.azcollection.azure_rm_diskencryptionset** : Create, delete and update Disk encryption set
* **azure.azcollection.azure_rm_diskencryptionset_info** : Get disk encryption set facts
* **azure.azcollection.azure_rm_dnsrecordset** : Create, delete and update DNS record sets and records
* **azure.azcollection.azure_rm_dnsrecordset_info** : Get DNS Record Set facts
* **azure.azcollection.azure_rm_dnszone** : Manage Azure DNS zones
* **azure.azcollection.azure_rm_dnszone_info** : Get DNS zone facts
* **azure.azcollection.azure_rm_eventhub** : Manage Event Hub
* **azure.azcollection.azure_rm_eventhub_info** : Get Azure Event Hub
* **azure.azcollection.azure_rm_expressroute** : Manage Express Route Circuits
* **azure.azcollection.azure_rm_expressroute_info** : Get Azure Express Route
* **azure.azcollection.azure_rm_firewallpolicy** : Create, delete or update specified firewall policy.
* **azure.azcollection.azure_rm_firewallpolicy_info** : Get firewall policy facts
* **azure.azcollection.azure_rm_functionapp** : Manage Azure Function Apps
* **azure.azcollection.azure_rm_functionapp_info** : Get Azure Function App facts
* **azure.azcollection.azure_rm_gallery** : Manage Azure Shared Image Gallery instance
* **azure.azcollection.azure_rm_gallery_info** : Get Azure Shared Image Gallery info
* **azure.azcollection.azure_rm_galleryimage** : Manage Azure SIG Image instance
* **azure.azcollection.azure_rm_galleryimage_info** : Get Azure SIG Image info
* **azure.azcollection.azure_rm_galleryimageversion** : Manage Azure SIG Image Version instance
* **azure.azcollection.azure_rm_galleryimageversion_info** : Get Azure SIG Image Version info
* **azure.azcollection.azure_rm_hdinsightcluster** : Manage Azure HDInsight Cluster instance
* **azure.azcollection.azure_rm_hdinsightcluster_info** : Get Azure HDInsight Cluster facts
* **azure.azcollection.azure_rm_hostgroup** : Create, delete and update a dedicated host group
* **azure.azcollection.azure_rm_hostgroup_info** : Get host group facts
* **azure.azcollection.azure_rm_image** : Manage Azure image
* **azure.azcollection.azure_rm_image_info** : Get facts about azure custom images
* **azure.azcollection.azure_rm_iotdevice** : Manage Azure IoT hub device
* **azure.azcollection.azure_rm_iotdevice_info** : Facts of Azure IoT hub device
* **azure.azcollection.azure_rm_iotdevicemodule** : Manage Azure IoT hub device module
* **azure.azcollection.azure_rm_iothubconsumergroup** : Manage Azure IoT hub
* **azure.azcollection.azure_rm_iothub_info** : Get IoT Hub facts
* **azure.azcollection.azure_rm_ipgroup** : Create, delete and update IP group
* **azure.azcollection.azure_rm_ipgroup_info** : Get IP group facts
* **azure.azcollection.azure_rm_keyvault** : Manage Key Vault instance
* **azure.azcollection.azure_rm_keyvault_info** : Get Azure Key Vault facts
* **azure.azcollection.azure_rm_keyvaultkey** : Use Azure KeyVault keys
* **azure.azcollection.azure_rm_keyvaultkey_info** : Get Azure Key Vault key facts
* **azure.azcollection.azure_rm_keyvaultsecret** : Use Azure KeyVault Secrets
* **azure.azcollection.azure_rm_keyvaultsecret_info** : Get Azure Key Vault secret facts
* **azure.azcollection.azure_rm_loadbalancer** : Manage Azure load balancers
* **azure.azcollection.azure_rm_loadbalancer_info** : Get load balancer facts
* **azure.azcollection.azure_rm_lock_info** : Manage Azure locks
* **azure.azcollection.azure_rm_loganalyticsworkspace** : Manage Azure Log Analytics workspaces
* **azure.azcollection.azure_rm_loganalyticsworkspace_info** : Get facts of Azure Log Analytics workspaces
* **azure.azcollection.azure_rm_manageddisk** : Manage Azure Manage Disks
* **azure.azcollection.azure_rm_manageddisk_info** : Get managed disk facts
* **azure.azcollection.azure_rm_managementgroup** : Manage Azure ManagementGroup instance
* **azure.azcollection.azure_rm_managementgroup_info** : Get Azure Management Group facts
* **azure.azcollection.azure_rm_mysqlconfiguration** : Manage Configuration instance
* **azure.azcollection.azure_rm_mariadbconfiguration_info** : Get Azure MariaDB Configuration facts
* **azure.azcollection.azure_rm_mariadbdatabase** : Manage MariaDB Database instance
* **azure.azcollection.azure_rm_mariadbdatabase_info** : Get Azure MariaDB Database facts
* **azure.azcollection.azure_rm_mariadbfirewallrule** : Manage MariaDB firewall rule instance
* **azure.azcollection.azure_rm_mariadbfirewallrule_info** : Get Azure MariaDB Firewall Rule facts
* **azure.azcollection.azure_rm_mariadbserver** : Manage MariaDB Server instance
* **azure.azcollection.azure_rm_mariadbserver_info** : Get Azure MariaDB Server facts
* **azure.azcollection.azure_rm_monitordiagnosticsetting** : Create, update, or manage Azure Monitor diagnostic settings.
* **azure.azcollection.azure_rm_monitordiagnosticsetting_info** : Get Azure Monitor diagnostic setting facts.
* **azure.azcollection.azure_rm_monitorlogprofile** : Manage Azure Monitor log profile
* **azure.azcollection.azure_rm_mysqlconfiguration_info** : Get Azure MySQL Configuration facts
* **azure.azcollection.azure_rm_mysqldatabase** : Manage MySQL Database instance
* **azure.azcollection.azure_rm_mysqldatabase_info** : Get Azure MySQL Database facts
* **azure.azcollection.azure_rm_mysqlfirewallrule** : Manage MySQL firewall rule instance
* **azure.azcollection.azure_rm_mysqlfirewallrule_info** : Get Azure MySQL Firewall Rule facts
* **azure.azcollection.azure_rm_mysqlserver** : Manage MySQL Server instance
* **azure.azcollection.azure_rm_mysqlserver_info** : Get Azure MySQL Server facts
* **azure.azcollection.azure_rm_natgateway** : Manage Azure NAT Gateway instance
* **azure.azcollection.azure_rm_natgateway_info** : Retrieve NAT Gateway instance facts
* **azure.azcollection.azure_rm_networkinterface** : Manage Azure network interfaces
* **azure.azcollection.azure_rm_networkinterface_info** : Get network interface facts
* **azure.azcollection.azure_rm_notificationhub** : Manage Notification Hub
* **azure.azcollection.azure_rm_notificationhub_info** : Get Azure Notification Hub
* **azure.azcollection.azure_rm_openshiftmanagedcluster** : Manage Azure Red Hat OpenShift Managed Cluster instance
* **azure.azcollection.azure_rm_openshiftmanagedcluster_info** : Get Info onf Azure Red Hat OpenShift Managed Cluster
* **azure.azcollection.azure_rm_postgresqlconfiguration** : Manage Azure PostgreSQL Configuration
* **azure.azcollection.azure_rm_postgresqlconfiguration_info** : Get Azure PostgreSQL Configuration facts
* **azure.azcollection.azure_rm_postgresqldatabase** : Manage PostgreSQL Database instance
* **azure.azcollection.azure_rm_postgresqldatabase_info** : Get Azure PostgreSQL Database facts
* **azure.azcollection.azure_rm_postgresqlfirewallrule** : Manage PostgreSQL firewall rule instance
* **azure.azcollection.azure_rm_postgresqlfirewallrule_info** : Get Azure PostgreSQL Firewall Rule facts
* **azure.azcollection.azure_rm_postgresqlserver** : Manage PostgreSQL Server instance
* **azure.azcollection.azure_rm_postgresqlserver_info** : Get Azure PostgreSQL Server facts
* **azure.azcollection.azure_rm_privatednsrecordset** : Create, delete and update Private DNS record sets and records
* **azure.azcollection.azure_rm_privatednsrecordset_info** : Get Private DNS Record Set facts
* **azure.azcollection.azure_rm_privatednszone** : Manage Azure private DNS zones
* **azure.azcollection.azure_rm_privatednszone_info** : Get private DNS zone facts
* **azure.azcollection.azure_rm_privatednszonelink** : Create, delete and update Virtual network link for Private DNS zone
* **azure.azcollection.azure_rm_privatednszonelink_info** : Get Virtual Network link facts for private DNS zone
* **azure.azcollection.azure_rm_privateendpoint** : Manage Azure private endpoint
* **azure.azcollection.azure_rm_privateendpoint_info** : Get private endpoints info
* **azure.azcollection.azure_rm_privateendpointconnection** : Managed private endpoint connection
* **azure.azcollection.azure_rm_privatelinkservice_info** : Get private endpoint connection info
* **azure.azcollection.azure_rm_privateendpointdnszonegroup** : Create, update, or manage private endpoint DNS zone groups.
* **azure.azcollection.azure_rm_privateendpointdnszonegroup_info** : Get private endpoint DNS zone group info.
* **azure.azcollection.azure_rm_privatelinkservice** : Managed private link service resource
* **azure.azcollection.azure_rm_proximityplacementgroup** : Create, delete and update proximity placement group
* **azure.azcollection.azure_rm_proximityplacementgroup_info** : Get proximity placement group facts
* **azure.azcollection.azure_rm_publicipaddress** : Manage Azure Public IP Addresses
* **azure.azcollection.azure_rm_publicipaddress_info** : Get public IP facts
* **azure.azcollection.azure_rm_recoveryservicesvault** : Create and Delete Azure Recovery Services vault
* **azure.azcollection.azure_rm_recoveryservicesvault_info** : Get Azure Recovery Services vault Details
* **azure.azcollection.azure_rm_rediscache** : Manage Azure Cache for Redis instance
* **azure.azcollection.azure_rm_rediscache_info** : Get Azure Cache for Redis instance facts
* **azure.azcollection.azure_rm_rediscachefirewallrule** : Manage Azure Cache for Redis Firewall rules
* **azure.azcollection.azure_rm_registrationassignment** : Manage Azure RegistrationAssignment instance
* **azure.azcollection.azure_rm_registrationassignment_info** : Get RegistrationAssignment info
* **azure.azcollection.azure_rm_registrationdefinition** : Manage Azure RegistrationDefinition instance
* **azure.azcollection.azure_rm_registrationdefinition_info** : Get RegistrationDefinition info
* **azure.azcollection.azure_rm_resource** : Create any Azure resource
* **azure.azcollection.azure_rm_resource_info** : Generic facts of Azure resources
* **azure.azcollection.azure_rm_resourcegroup** : Manage Azure resource groups
* **azure.azcollection.azure_rm_resourcegroup_info** : Get resource group facts
* **azure.azcollection.azure_rm_roleassignment** : Manage Azure Role Assignment
* **azure.azcollection.azure_rm_roleassignment_info** : Gets Azure Role Assignment facts
* **azure.azcollection.azure_rm_roledefinition** : Manage Azure Role Definition
* **azure.azcollection.azure_rm_roledefinition_info** : Get Azure Role Definition facts
* **azure.azcollection.azure_rm_route** : Manage Azure route resource
* **azure.azcollection.azure_rm_route_info** : Get Route info
* **azure.azcollection.azure_rm_routetable** : Manage Azure route table resource
* **azure.azcollection.azure_rm_routetable_info** : Get route table facts
* **azure.azcollection.azure_rm_securitygroup** : Manage Azure network security groups
* **azure.azcollection.azure_rm_securitygroup_info** : Get security group facts
* **azure.azcollection.azure_rm_servicebustopic** : Manage Azure Service Bus
* **azure.azcollection.azure_rm_servicebus_info** : Get servicebus facts
* **azure.azcollection.azure_rm_servicebusqueue** : Manage Azure Service Bus queue
* **azure.azcollection.azure_rm_servicebussaspolicy** : Manage Azure Service Bus SAS policy
* **azure.azcollection.azure_rm_servicebustopicsubscription** : Manage Azure Service Bus subscription
* **azure.azcollection.azure_rm_snapshot** : Manage Azure Snapshot instance.
* **azure.azcollection.azure_rm_sqldatabase** : Manage SQL Database instance
* **azure.azcollection.azure_rm_sqldatabase_info** : Get Azure SQL Database facts
* **azure.azcollection.azure_rm_sqlfirewallrule** : Manage Firewall Rule instance
* **azure.azcollection.azure_rm_sqlfirewallrule_info** : Get Azure SQL Firewall Rule facts
* **azure.azcollection.azure_rm_sqlserver** : Manage SQL Server instance
* **azure.azcollection.azure_rm_sqlserver_info** : Get SQL Server facts
* **azure.azcollection.azure_rm_storageaccount** : Manage Azure storage accounts
* **azure.azcollection.azure_rm_storageaccount_info** : Get storage account facts
* **azure.azcollection.azure_rm_storageblob** : Manage blob containers and blob objects
* **azure.azcollection.azure_rm_storageshare** : Manage Azure storage file share
* **azure.azcollection.azure_rm_storageshare_info** : Get Azure storage file share info
* **azure.azcollection.azure_rm_subnet** : Manage Azure subnets
* **azure.azcollection.azure_rm_subnet_info** : Get Azure Subnet facts
* **azure.azcollection.azure_rm_subscription_info** : Get Azure Subscription facts
* **azure.azcollection.azure_rm_trafficmanager** : Manage a Traffic Manager profile.
* **azure.azcollection.azure_rm_trafficmanagerendpoint** : Manage Azure Traffic Manager endpoint
* **azure.azcollection.azure_rm_trafficmanagerendpoint_info** : Get Azure Traffic Manager endpoint facts
* **azure.azcollection.azure_rm_trafficmanagerprofile** : Manage Azure Traffic Manager profile
* **azure.azcollection.azure_rm_trafficmanagerprofile_info** : Get Azure Traffic Manager profile facts
* **azure.azcollection.azure_rm_virtualhubconnection** : Manage Azure VirtualHub instance
* **azure.azcollection.azure_rm_virtualhubconnection_info** : Get VirtualHub info
* **azure.azcollection.azure_rm_virtualmachine** : Manage Azure virtual machines
* **azure.azcollection.azure_rm_virtualmachine_info** : Get virtual machine facts
* **azure.azcollection.azure_rm_virtualmachineextension** : Managed Azure Virtual Machine extension
* **azure.azcollection.azure_rm_virtualmachineextension_info** : Get Azure Virtual Machine Extension facts
* **azure.azcollection.azure_rm_virtualmachineimage_info** : Get virtual machine image facts
* **azure.azcollection.azure_rm_virtualmachinescaleset** : Manage Azure virtual machine scale sets
* **azure.azcollection.azure_rm_virtualmachinescaleset_info** : Get Virtual Machine Scale Set facts
* **azure.azcollection.azure_rm_virtualmachinescalesetextension** : Manage Azure Virtual Machine Scale Set (VMSS) extensions
* **azure.azcollection.azure_rm_virtualmachinescalesetextension_info** : Get Azure Virtual Machine Scale Set Extension facts
* **azure.azcollection.azure_rm_virtualmachinescalesetinstance_info** : Get Azure Virtual Machine Scale Set Instance facts
* **azure.azcollection.azure_rm_virtualmachinesize_info** : Get facts for virtual machine sizes
* **azure.azcollection.azure_rm_virtualnetwork** : Manage Azure virtual networks
* **azure.azcollection.azure_rm_virtualnetwork_info** : Get virtual network facts
* **azure.azcollection.azure_rm_virtualnetworkgateway** : Manage Azure virtual network gateways
* **azure.azcollection.azure_rm_virtualnetworkpeering** : Manage Azure Virtual Network Peering
* **azure.azcollection.azure_rm_virtualnetworkpeering_info** : Get facts of Azure Virtual Network Peering
* **azure.azcollection.azure_rm_virtualwan** : Manage Azure VirtualWan instance
* **azure.azcollection.azure_rm_virtualwan_info** : Get VirtualWan info
* **azure.azcollection.azure_rm_vmbackuppolicy** : Create or Delete Azure VM Backup Policy
* **azure.azcollection.azure_rm_vmbackuppolicy_info** : Fetch Backup Policy Details
* **azure.azcollection.azure_rm_vpnsite** : Manage Azure VpnSite instance
* **azure.azcollection.azure_rm_vpnsite_info** : Get VpnSite info
* **azure.azcollection.azure_rm_vpnsitelink_info** : Get VpnSiteLink info
* **azure.azcollection.azure_rm_webapp** : Manage Web App instances
* **azure.azcollection.azure_rm_webapp_info** : Get Azure web app facts
* **azure.azcollection.azure_rm_webappaccessrestriction** : Manage web app network access restrictions
* **azure.azcollection.azure_rm_webappaccessrestriction_info** : Retrieve web app network access restriction facts
* **azure.azcollection.azure_rm_webappslot** : Manage Azure Web App slot
* **azure.azcollection.azure_rm_webappvnetconnection** : Manage web app virtual network connection
* **azure.azcollection.azure_rm_webappvnetconnection_info** : Get Azure web app virtual network connection facts

## `check_point.mgmt` collection

* **check_point.mgmt.cp_mgmt_access_layer** : Manages access-layer objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_access_layer_facts** : Get access-layer objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_access_role** : Manages access-role objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_access_role_facts** : Get access-role objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_access_rule** : Manages access-rule objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_access_rule_facts** : Get access-rule objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_access_rules** : Manages access-rules objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_access_section** : Manages access-section objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_add_api_key** : Add API key for administrator, to enable login with it. For the key to be valid publish is needed.
* **check_point.mgmt.cp_mgmt_add_data_center_object** : Imports a Data Center Object from a Data Center Server.&lt;br&gt; Data Center Object represents an object in the cloud environment.
* **check_point.mgmt.cp_mgmt_add_domain** : Create new object
* **check_point.mgmt.cp_mgmt_add_nat_rule** : Create new object.
* **check_point.mgmt.cp_mgmt_add_rules_batch** : Creates new rules in batch. Use this API to achieve optimum performance when adding more than one rule.
* **check_point.mgmt.cp_mgmt_address_range** : Manages address-range objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_address_range_facts** : Get address-range objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_administrator** : Manages administrator objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_administrator_facts** : Get administrator objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_application_site** : Manages application-site objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_application_site_category** : Manages application-site-category objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_application_site_category_facts** : Get application-site-category objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_application_site_facts** : Get application-site objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_application_site_group** : Manages application-site-group objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_application_site_group_facts** : Get application-site-group objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_approve_session** : Workflow feature - Approve and Publish the session.
* **check_point.mgmt.cp_mgmt_assign_global_assignment** : assign global assignment on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_check_network_feed** : Check if a target can reach or parse a network feed; can work with an existing feed object or with a new one (by providing all relevant feed parameters).
* **check_point.mgmt.cp_mgmt_check_threat_ioc_feed** : Check if a target can reach or parse a threat IOC feed; can work with an existing feed object or with a new one (by providing all relevant feed parameters).
* **check_point.mgmt.cp_mgmt_cluster_members_facts** : Retrieve all existing cluster members in domain.
* **check_point.mgmt.cp_mgmt_connect_cloud_services** : Securely connect the Management Server to Check Point&#39;s Infinity Portal. &lt;br&gt;This is a preliminary operation so that the management server can use various Check Point cloud-based security services hosted in the Infinity Portal.
* **check_point.mgmt.cp_mgmt_data_center_object_facts** : Get data-center-object objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_delete_api_key** : Delete the API key. For the key to be invalid publish is needed.
* **check_point.mgmt.cp_mgmt_delete_nat_rule** : Delete existing object using object name or uid.
* **check_point.mgmt.cp_mgmt_delete_rules_batch** : Delete rules in batch from the same layer. Use this API to achieve optimum performance when removing more than one rule.
* **check_point.mgmt.cp_mgmt_discard** : All changes done by user are discarded and removed from database.
* **check_point.mgmt.cp_mgmt_disconnect_cloud_services** : Disconnect the Management Server from Check Point&#39;s Infinity Portal.
* **check_point.mgmt.cp_mgmt_dns_domain** : Manages dns-domain objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_dns_domain_facts** : Get dns-domain objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_domain_facts** : Get domain objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_domain_permissions_profile** : Manages domain-permissions-profile objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_domain_permissions_profile_facts** : Get domain-permissions-profile objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_dynamic_object** : Manages dynamic-object objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_dynamic_object_facts** : Get dynamic-object objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_exception_group** : Manages exception-group objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_exception_group_facts** : Get exception-group objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_get_platform** : Get actual platform (Hardware, Version, OS) from gateway, cluster or Check Point host.
* **check_point.mgmt.cp_mgmt_global_assignment** : Manages global-assignment objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_global_assignment_facts** : Get global-assignment objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_group** : Manages group objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_group_facts** : Get group objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_group_with_exclusion** : Manages group-with-exclusion objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_group_with_exclusion_facts** : Get group-with-exclusion objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_host** : Manages host objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_host_facts** : Get host objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_https_section** : Manages https-section objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_identity_tag** : Manages identity-tag objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_identity_tag_facts** : Get identity-tag objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_idp_administrator_group** : Manages idp-administrator-group objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_idp_administrator_group_facts** : Get idp-administrator-group objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_idp_to_domain_assignment_facts** : Get idp-to-domain-assignment objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_install_database** : Copies the user database and network objects information to specified targets.
* **check_point.mgmt.cp_mgmt_install_lsm_policy** : Executes the lsm-install-policy on a given list of targets. Install the LSM policy that defined on the attached LSM profile on the targets devices.
* **check_point.mgmt.cp_mgmt_install_lsm_settings** : Executes the lsm-install-settings on a given list of targets. Install the provisioning settings that defined on the object on the targets devices.
* **check_point.mgmt.cp_mgmt_install_policy** : install policy on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_install_software_package** : Installs the software package on target machines.
* **check_point.mgmt.cp_mgmt_interoperable_device** : Manages interoperable-device objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_interoperable_device_facts** : Get interoperable-device objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_lsm_cluster** : Manages lsm-cluster objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_lsm_cluster_facts** : Get lsm-cluster objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_lsm_cluster_profile_facts** : Get lsm-cluster-profile objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_lsm_gateway** : Manages lsm-gateway objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_lsm_gateway_facts** : Get lsm-gateway objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_lsm_gateway_profile_facts** : Get lsm-gateway-profile objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_lsm_run_script** : Executes the lsm-run-script on a given list of targets. Run the given script on the targets devices.
* **check_point.mgmt.cp_mgmt_md_permissions_profile** : Manages md-permissions-profile objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_md_permissions_profile_facts** : Get md-permissions-profile objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_mds** : Manages mds objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_mds_facts** : Get Multi-Domain Server (mds) objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_multicast_address_range** : Manages multicast-address-range objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_multicast_address_range_facts** : Get multicast-address-range objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_nat_rule_facts** : Get nat-rule objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_nat_section** : Manages nat-section objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_network** : Manages network objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_network_facts** : Get network objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_network_feed** : Manages network-feed objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_network_feed_facts** : Get network-feed objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_objects_facts** : Get objects objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_package** : Manages package objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_package_facts** : Get package objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_provisioning_profile_facts** : Get provisioning-profile objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_publish** : All the changes done by this user will be seen by all users only after publish is called.
* **check_point.mgmt.cp_mgmt_put_file** : put file on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_reject_session** : Workflow feature - Return the session to the submitter administrator.
* **check_point.mgmt.cp_mgmt_repository_script** : Manages repository-script objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_repository_script_facts** : Get repository-script objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_reset_sic** : Reset Secure Internal Communication (SIC). To complete the reset operation need also to reset the device in the Check Point Configuration Tool (by running cpconfig in Clish or Expert mode). Communication will not be possible until you reset and re-initialize the device properly.
* **check_point.mgmt.cp_mgmt_run_ips_update** : Runs IPS database update. If &#34;package-path&#34; is not provided server will try to get the latest package from the User Center.
* **check_point.mgmt.cp_mgmt_run_script** : Executes the script on a given list of targets.
* **check_point.mgmt.cp_mgmt_security_zone** : Manages security-zone objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_security_zone_facts** : Get security-zone objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_dce_rpc** : Manages service-dce-rpc objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_dce_rpc_facts** : Get service-dce-rpc objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_group** : Manages service-group objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_group_facts** : Get service-group objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_icmp** : Manages service-icmp objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_icmp6** : Manages service-icmp6 objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_icmp6_facts** : Get service-icmp6 objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_icmp_facts** : Get service-icmp objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_other** : Manages service-other objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_other_facts** : Get service-other objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_rpc** : Manages service-rpc objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_rpc_facts** : Get service-rpc objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_sctp** : Manages service-sctp objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_sctp_facts** : Get service-sctp objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_tcp** : Manages service-tcp objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_tcp_facts** : Get service-tcp objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_udp** : Manages service-udp objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_service_udp_facts** : Get service-udp objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_session_facts** : Get session objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_threat_protection_override** : Edit existing object using object name or uid.
* **check_point.mgmt.cp_mgmt_set_global_properties** : Edit Global Properties.
* **check_point.mgmt.cp_mgmt_set_idp_default_assignment** : Set default Identity Provider assignment to be use for Management server administrator access.
* **check_point.mgmt.cp_mgmt_set_idp_to_domain_assignment** : Set Identity Provider assignment to domain, to allow administrator login to that domain using that identity provider, if there is no Identity Provider assigned to the domain the &#39;idp-default-assignment&#39; will be used. This command only available  for Multi-Domain server.
* **check_point.mgmt.cp_mgmt_set_session** : Edit user&#39;s current session.
* **check_point.mgmt.cp_mgmt_set_threat_advanced_settings** : Edit Threat Prevention&#39;s Blades&#39; Settings.
* **check_point.mgmt.cp_mgmt_show_nat_section** : Retrieve existing object using object name or uid.
* **check_point.mgmt.cp_mgmt_show_cloud_services** : Show the connection status of the Management Server to Check Point&#39;s Infinity Portal.
* **check_point.mgmt.cp_mgmt_show_global_properties** : Retrieve Global Properties.
* **check_point.mgmt.cp_mgmt_show_https_section** : Retrieve existing HTTPS Inspection section using section name or uid and layer name.
* **check_point.mgmt.cp_mgmt_show_idp_default_assignment** : Retrieve default Identity Provider assignment that used for Management server administrator access.
* **check_point.mgmt.cp_mgmt_show_logs** : Showing logs according to the given filter.
* **check_point.mgmt.cp_mgmt_show_servers_and_processes** : Shows the status of all processes in the current machine (Multi-Domain Server and all Domain Management / Log Servers). &lt;br&gt;This command is available only on Multi-Domain Server.
* **check_point.mgmt.cp_mgmt_show_software_package_details** : Gets the software package information from the cloud.
* **check_point.mgmt.cp_mgmt_show_task** : Show task progress and details.
* **check_point.mgmt.cp_mgmt_show_tasks** : Retrieve all tasks and show their progress and details.
* **check_point.mgmt.cp_mgmt_show_threat_advanced_settings** : Show Threat Prevention&#39;s Blades&#39; Settings.
* **check_point.mgmt.cp_mgmt_simple_cluster** : Manages simple-cluster objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_simple_cluster_facts** : Get simple-cluster objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_simple_gateway** : Manages simple-gateway objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_simple_gateway_facts** : Get simple-gateway objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_smtp_server** : Manages smtp-server objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_smtp_server_facts** : Get smtp-server objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_submit_session** : Workflow feature - Submit the session for approval.
* **check_point.mgmt.cp_mgmt_tag** : Manages tag objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_tag_facts** : Get tag objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_test_sic_status** : Test SIC Status reflects the state of the gateway after it has received the certificate issued by the ICA. If the SIC status is Unknown then there is no connection between the gateway and the Security Management Server. If the SIC status is No Communication, an error message will appear. It may contain specific instructions on how to fix the situation.
* **check_point.mgmt.cp_mgmt_threat_exception** : Manages threat-exception objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_threat_exception_facts** : Get threat-exception objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_threat_indicator** : Manages threat-indicator objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_threat_indicator_facts** : Get threat-indicator objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_threat_layer** : Manages threat-layer objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_threat_layer_facts** : Get threat-layer objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_threat_profile** : Manages threat-profile objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_threat_profile_facts** : Get threat-profile objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_threat_rule** : Manages threat-rule objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_threat_rule_facts** : Get threat-rule objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_time** : Manages time objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_time_facts** : Get time objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_trusted_client** : Manages trusted-client objects on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_trusted_client_facts** : Get trusted-client objects facts on Checkpoint over Web Services API
* **check_point.mgmt.cp_mgmt_uninstall_software_package** : Uninstalls the software package from target machines.
* **check_point.mgmt.cp_mgmt_update_provisioned_satellites** : Executes the update-provisioned-satellites on center gateways of VPN communities.
* **check_point.mgmt.cp_mgmt_verify_policy** : Verifies the policy of the selected package.
* **check_point.mgmt.cp_mgmt_verify_software_package** : Verifies the software package on target machines.
* **check_point.mgmt.cp_mgmt_vpn_community_meshed** : Manages vpn-community-meshed objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_vpn_community_meshed_facts** : Get vpn-community-meshed objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_vpn_community_star** : Manages vpn-community-star objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_vpn_community_star_facts** : Get vpn-community-star objects facts on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_wildcard** : Manages wildcard objects on Check Point over Web Services API
* **check_point.mgmt.cp_mgmt_wildcard_facts** : Get wildcard objects facts on Check Point over Web Services API

## `chocolatey.chocolatey` collection

* **chocolatey.chocolatey.win_chocolatey** : Manage packages using chocolatey
* **chocolatey.chocolatey.win_chocolatey_config** : Manages Chocolatey config settings
* **chocolatey.chocolatey.win_chocolatey_facts** : Create a facts collection for Chocolatey
* **chocolatey.chocolatey.win_chocolatey_feature** : Manages Chocolatey features
* **chocolatey.chocolatey.win_chocolatey_source** : Manages Chocolatey sources

## `cisco.aci` collection

* **cisco.aci.aci_aaa_custom_privilege** : Manage AAA RBAC Custom Privileges (aaa:RbacClassPriv)
* **cisco.aci.aci_aaa_domain** : Manage AAA domains (aaa:Domain)
* **cisco.aci.aci_aaa_role** : Manage AAA roles (aaa:Role)
* **cisco.aci.aci_aaa_ssh_auth** : Manage AAA SSH auth (aaaSshAuth) objects.
* **cisco.aci.aci_aaa_user** : Manage AAA users (aaa:User)
* **cisco.aci.aci_aaa_user_certificate** : Manage AAA user certificates (aaa:UserCert)
* **cisco.aci.aci_aaa_user_domain** : Manage AAA user domains (aaa:UserDomain)
* **cisco.aci.aci_aaa_user_role** : Manage AAA user roles (aaa:UserRole)
* **cisco.aci.aci_access_port_block_to_access_port** : Manage port blocks of Fabric interface policy leaf profile interface selectors (infra:HPortS, infra:PortBlk)
* **cisco.aci.aci_access_port_to_interface_policy_leaf_profile** : Manage Fabric interface policy leaf profile interface selectors (infra:HPortS, infra:RsAccBaseGrp, infra:PortBlk)
* **cisco.aci.aci_access_sub_port_block_to_access_port** : Manage sub port blocks of Fabric interface policy leaf profile interface selectors (infra:HPortS, infra:SubPortBlk)
* **cisco.aci.aci_aep** : Manage attachable Access Entity Profile (AEP) objects (infra:AttEntityP, infra:ProvAcc)
* **cisco.aci.aci_aep_to_domain** : Bind AEPs to Physical or Virtual Domains (infra:RsDomP)
* **cisco.aci.aci_aep_to_epg** : Bind EPG to AEP (infra:RsFuncToEpg).
* **cisco.aci.aci_ap** : Manage top level Application Profile (AP) objects (fv:Ap)
* **cisco.aci.aci_bd** : Manage Bridge Domains (BD) objects (fv:BD)
* **cisco.aci.aci_bd_dhcp_label** : Manage DHCP Labels (dhcp:Lbl)
* **cisco.aci.aci_bd_subnet** : Manage Subnets (fv:Subnet)
* **cisco.aci.aci_bd_to_l3out** : Bind Bridge Domain to L3 Out (fv:RsBDToOut)
* **cisco.aci.aci_bgp_rr_asn** : Manage BGP Route Reflector ASN.
* **cisco.aci.aci_bgp_rr_node** : Manage BGP Route Reflector objects.
* **cisco.aci.aci_static_binding_to_epg** : Bind static paths to EPGs (fv:RsPathAtt)
* **cisco.aci.aci_cloud_ap** : Manage Cloud Application Profile (AP) (cloud:App)
* **cisco.aci.aci_cloud_aws_provider** : Manage Cloud AWS Provider (cloud:AwsProvider)
* **cisco.aci.aci_cloud_bgp_asn** : Manage Cloud APIC BGP Autonomous System Profile (cloud:BgpAsP)
* **cisco.aci.aci_cloud_cidr** : Manage CIDR under Cloud Context Profile (cloud:Cidr)
* **cisco.aci.aci_cloud_ctx_profile** : Manage Cloud Context Profile (cloud:CtxProfile)
* **cisco.aci.aci_cloud_epg** : Manage Cloud EPG (cloud:EPg)
* **cisco.aci.aci_cloud_epg_selector** : Manage Cloud Endpoint Selector (cloud:EPSelector)
* **cisco.aci.aci_cloud_external_epg** : Manage Cloud External EPG (cloud:ExtEPg)
* **cisco.aci.aci_cloud_external_epg_selector** : Manage Cloud Endpoint Selector for External EPGs (cloud:ExtEPSelector)
* **cisco.aci.aci_cloud_provider** : Query Cloud Provider information (cloud:ProvP)
* **cisco.aci.aci_cloud_region** : Manage Cloud Providers Region (cloud:Region)
* **cisco.aci.aci_cloud_subnet** : Manage Cloud Subnet (cloud:Subnet)
* **cisco.aci.aci_cloud_vpn_gateway** : Manage cloudRouterP in Cloud Context Profile (cloud:cloudRouterP)
* **cisco.aci.aci_cloud_zone** : Manage Cloud Availability Zone (cloud:Zone)
* **cisco.aci.aci_config_rollback** : Provides rollback and rollback preview functionality (config:ImportP)
* **cisco.aci.aci_config_snapshot** : Manage Config Snapshots (config:Snapshot, config:ExportP)
* **cisco.aci.aci_contract** : Manage contract resources (vz:BrCP)
* **cisco.aci.aci_contract_export** : Manage contract interfaces (vz:CPIf)
* **cisco.aci.aci_contract_subject** : Manage initial Contract Subjects (vz:Subj)
* **cisco.aci.aci_contract_subject_to_filter** : Bind Contract Subjects to Filters (vz:RsSubjFiltAtt)
* **cisco.aci.aci_contract_subject_to_service_graph** : Bind contract subject to service graph (vz:RsSubjGraphAtt).
* **cisco.aci.aci_dhcp_relay** : Manage DHCP relay policies.
* **cisco.aci.aci_dhcp_relay_provider** : Manage DHCP relay policy providers.
* **cisco.aci.aci_dns_domain** : Manage DNS Provider (dnsDomain) objects.
* **cisco.aci.aci_dns_profile** : Manage DNS Profile (dnsProfile) objects.
* **cisco.aci.aci_dns_provider** : Manage DNS Provider (dnsProv) objects.
* **cisco.aci.aci_domain** : Manage physical, virtual, bridged, routed or FC domain profiles (phys:DomP, vmm:DomP, l2ext:DomP, l3ext:DomP, fc:DomP)
* **cisco.aci.aci_domain_to_encap_pool** : Bind Domain to Encap Pools (infra:RsVlanNs)
* **cisco.aci.aci_domain_to_vlan_pool** : Bind Domain to VLAN Pools (infra:RsVlanNs)
* **cisco.aci.aci_encap_pool** : Manage encap pools (fvns:VlanInstP, fvns:VxlanInstP, fvns:VsanInstP)
* **cisco.aci.aci_encap_pool_range** : Manage encap ranges assigned to pools (fvns:EncapBlk, fvns:VsanEncapBlk)
* **cisco.aci.aci_epg** : Manage End Point Groups (EPG) objects (fv:AEPg)
* **cisco.aci.aci_epg_monitoring_policy** : Manage monitoring policies (mon:EPGPol)
* **cisco.aci.aci_epg_to_contract** : Bind EPGs to Contracts (fv:RsCons, fv:RsProv)
* **cisco.aci.aci_epg_to_contract_interface** : Bind EPGs to Consumed Contracts Interface (fv:RsConsIf).
* **cisco.aci.aci_epg_to_contract_master** : Manage End Point Group (EPG) contract master relationships (fv:RsSecInherited)
* **cisco.aci.aci_epg_to_domain** : Bind EPGs to Domains (fv:RsDomAtt)
* **cisco.aci.aci_esg** : Manage Endpoint Security Groups (ESGs) objects (fv:ESg)
* **cisco.aci.aci_esg_contract_master** : Manage ESG contract master relationships (fv:RsSecInherited)
* **cisco.aci.aci_esg_epg_selector** : Manage ESG - EPG Selectors (fv:fvEPgSelector)
* **cisco.aci.aci_esg_ip_subnet_selector** : Manage ESG IP Subnet selector(fv:EPSelector)
* **cisco.aci.aci_esg_tag_selector** : Manage ESG Tag Selectors (fv:TagSelector)
* **cisco.aci.aci_fabric_leaf_profile** : Manage fabric leaf profiles (fabric:LeafP).
* **cisco.aci.aci_fabric_leaf_switch_assoc** : Manage leaf switch bindings to profiles and policy groups (fabric:LeafS and fabric:RsLeNodePGrp).
* **cisco.aci.aci_fabric_node** : Manage Fabric Node Members (fabric:NodeIdentP)
* **cisco.aci.aci_fabric_pod_policy_group** : Manage Fabric Pod Policy Groups (fabric:PodPGrp)
* **cisco.aci.aci_fabric_scheduler** : This modules creates ACI schedulers.
* **cisco.aci.aci_fabric_spine_profile** : Manage fabric spine profiles (fabric:SpineP).
* **cisco.aci.aci_fabric_spine_switch_assoc** : Manage spine switch bindings to profiles and policy groups (fabric:SpineS and fabric:RsSpNodePGrp).
* **cisco.aci.aci_fabric_switch_block** : Manage switch blocks (fabric:NodeBlk).
* **cisco.aci.aci_fabric_switch_policy_group** : Manage Fabric Switch Policy Group objects.
* **cisco.aci.aci_filter** : Manages top level filter objects (vz:Filter)
* **cisco.aci.aci_filter_entry** : Manage filter entries (vz:Entry)
* **cisco.aci.aci_firmware_group** : This module creates a firmware group
* **cisco.aci.aci_firmware_group_node** : This modules adds and remove nodes from the firmware group
* **cisco.aci.aci_firmware_policy** : This creates a firmware policy
* **cisco.aci.aci_firmware_source** : Manage firmware image sources (firmware:OSource)
* **cisco.aci.aci_interface_blacklist** : Enabling or Disabling physical interfaces.
* **cisco.aci.aci_interface_description** : Setting and removing description on physical interfaces.
* **cisco.aci.aci_interface_policy_cdp** : Manage CDP interface policies (cdp:IfPol)
* **cisco.aci.aci_interface_policy_fc** : Manage Fibre Channel interface policies (fc:IfPol)
* **cisco.aci.aci_interface_policy_l2** : Manage Layer 2 interface policies (l2:IfPol)
* **cisco.aci.aci_interface_policy_leaf_breakout_port_group** : Manage fabric interface policy leaf breakout port group (infra:BrkoutPortGrp)
* **cisco.aci.aci_interface_policy_leaf_policy_group** : Manage fabric interface policy leaf policy groups (infra:AccBndlGrp, infra:AccPortGrp)
* **cisco.aci.aci_interface_policy_leaf_profile** : Manage fabric interface policy leaf profiles (infra:AccPortP)
* **cisco.aci.aci_interface_policy_leaf_profile_fex_policy_group** : Manage leaf interface profiles fex policy group (infra:FexBndlGrp)
* **cisco.aci.aci_interface_policy_link_level** : Manage Link Level interface policies (fabric:HIfPol)
* **cisco.aci.aci_interface_policy_lldp** : Manage LLDP interface policies (lldp:IfPol)
* **cisco.aci.aci_interface_policy_mcp** : Manage MCP interface policies (mcp:IfPol)
* **cisco.aci.aci_interface_policy_ospf** : Manage OSPF interface policies (ospf:IfPol)
* **cisco.aci.aci_interface_policy_port_channel** : Manage port channel interface policies (lacp:LagPol)
* **cisco.aci.aci_interface_policy_port_security** : Manage port security (l2:PortSecurityPol)
* **cisco.aci.aci_interface_selector_to_switch_policy_leaf_profile** : Bind interface selector profiles to switch policy leaf profiles (infra:RsAccPortP)
* **cisco.aci.aci_l2out** : Manage Layer2 Out (L2Out) objects.
* **cisco.aci.aci_l2out_extepg** : Manage External Network Instance (L2Out External EPG) objects (l2extInstP).
* **cisco.aci.aci_l2out_extepg_to_contract** : Bind Contracts to L2 External End Point Groups (EPGs)
* **cisco.aci.aci_l2out_logical_interface_path** : Manage Layer 2 Outside (L2Out) logical interface path (l2extRsPathL2OutAtt)
* **cisco.aci.aci_l2out_logical_interface_profile** : Manage Layer 2 Outside (L2Out) interface profiles (l2ext:LIfP)
* **cisco.aci.aci_l2out_logical_node_profile** : Manage Layer 2 Outside (L2Out) logical node profiles (l2ext:LNodeP)
* **cisco.aci.aci_l3out** : Manage Layer 3 Outside (L3Out) objects (l3ext:Out)
* **cisco.aci.aci_l3out_bgp_peer** : Manage Layer 3 Outside (L3Out) BGP Peers (bgp:PeerP)
* **cisco.aci.aci_l3out_extepg** : Manage External Network Instance Profile (ExtEpg) objects (l3extInstP:instP)
* **cisco.aci.aci_l3out_extepg_to_contract** : Bind Contracts to External End Point Groups (EPGs)
* **cisco.aci.aci_l3out_extsubnet** : Manage External Subnet objects (l3extSubnet:extsubnet)
* **cisco.aci.aci_l3out_interface** : Manage Layer 3 Outside (L3Out) interfaces (l3ext:RsPathL3OutAtt)
* **cisco.aci.aci_l3out_interface_secondary_ip** : Manage Layer 3 Outside (L3Out) interface secondary IP addresses (l3ext:Ip).
* **cisco.aci.aci_l3out_logical_interface_profile** : Manage Layer 3 Outside (L3Out) logical interface profiles (l3ext:LIfP)
* **cisco.aci.aci_l3out_logical_interface_profile_ospf_policy** : Manage Layer 3 Outside (L3Out) logical interface profile (l3ext:LIfP) OSPF policy (ospfIfP)
* **cisco.aci.aci_l3out_logical_interface_vpc_member** : Manage Member Node objects (l3ext:Member)
* **cisco.aci.aci_l3out_logical_node** : Manage Layer 3 Outside (L3Out) logical node profile nodes (l3ext:RsNodeL3OutAtt)
* **cisco.aci.aci_l3out_logical_node_profile** : Manage Layer 3 Outside (L3Out) logical node profiles (l3extLNodeP:lnodep)
* **cisco.aci.aci_l3out_route_tag_policy** : Manage route tag policies (l3ext:RouteTagPol)
* **cisco.aci.aci_l3out_static_routes** : Manage Static routes object (l3ext:ipRouteP)
* **cisco.aci.aci_l3out_static_routes_nexthop** : Manage nexthops for static routes (ip:NexthopP)
* **cisco.aci.aci_maintenance_group** : This creates an ACI maintenance group
* **cisco.aci.aci_maintenance_group_node** : Manage maintenance group nodes
* **cisco.aci.aci_maintenance_policy** : Manage firmware maintenance policies
* **cisco.aci.aci_node_mgmt_epg** : In band or Out of band management EPGs
* **cisco.aci.aci_ntp_policy** : Manage NTP policies.
* **cisco.aci.aci_ntp_server** : Manage NTP servers.
* **cisco.aci.aci_rest** : Direct access to the Cisco APIC REST API
* **cisco.aci.aci_snmp_client** : Manage SNMP clients (snmp:ClientP).
* **cisco.aci.aci_snmp_client_group** : Manage SNMP client groups (snmp:ClientGrpP).
* **cisco.aci.aci_snmp_community_policy** : Manage SNMP community policies (snmp:CommunityP).
* **cisco.aci.aci_snmp_policy** : Manage Syslog groups (snmp:Pol).
* **cisco.aci.aci_snmp_user** : Manage SNMP v3 Users (snmp:UserP).
* **cisco.aci.aci_static_node_mgmt_address** : In band or Out of band management IP address
* **cisco.aci.aci_switch_leaf_selector** : Bind leaf selectors to switch policy leaf profiles (infra:LeafS, infra:NodeBlk, infra:RsAccNodePGrep)
* **cisco.aci.aci_switch_policy_leaf_profile** : Manage switch policy leaf profiles (infra:NodeP)
* **cisco.aci.aci_switch_policy_vpc_protection_group** : Manage switch policy explicit vPC protection groups (fabric:ExplicitGEp, fabric:NodePEp).
* **cisco.aci.aci_syslog_group** : Manage Syslog groups (syslog:Group, syslog:Console, syslog:File and syslog:Prof).
* **cisco.aci.aci_syslog_remote_dest** : Manage Syslog Remote Destinations (syslog:RemoteDest).
* **cisco.aci.aci_syslog_source** : Manage Syslog Source objects (syslog:Src)
* **cisco.aci.aci_system** : Query the ACI system information (top:System)
* **cisco.aci.aci_taboo_contract** : Manage taboo contracts (vz:BrCP)
* **cisco.aci.aci_tag** : Tagging of ACI objects
* **cisco.aci.aci_tenant** : Manage tenants (fv:Tenant)
* **cisco.aci.aci_tenant_action_rule_profile** : Manage action rule profiles (rtctrl:AttrP)
* **cisco.aci.aci_tenant_ep_retention_policy** : Manage End Point (EP) retention protocol policies (fv:EpRetPol)
* **cisco.aci.aci_tenant_span_dst_group** : Manage SPAN destination groups (span:DestGrp)
* **cisco.aci.aci_tenant_span_src_group** : Manage SPAN source groups (span:SrcGrp)
* **cisco.aci.aci_tenant_span_src_group_src** : Manage SPAN source group sources (span:Src)
* **cisco.aci.aci_tenant_span_src_group_to_dst_group** : Bind SPAN source groups to destination groups (span:SpanLbl)
* **cisco.aci.aci_vlan_pool** : Manage VLAN pools (fvns:VlanInstP)
* **cisco.aci.aci_vlan_pool_encap_block** : Manage encap blocks assigned to VLAN pools (fvns:EncapBlk)
* **cisco.aci.aci_vmm_controller** : Manage VMM Controller for virtual domains profiles (vmm:CtrlrP)
* **cisco.aci.aci_vmm_credential** : Manage virtual domain credential profiles (vmm:UsrAccP)
* **cisco.aci.aci_vmm_uplink** : Manage VMM uplinks (vmm:UplinkP)
* **cisco.aci.aci_vmm_uplink_container** : Manage VMM uplink containers (vmm:UplinkPCont)
* **cisco.aci.aci_vmm_vswitch_policy** : Manage vSwitch policy for VMware virtual domains profiles (vmm:DomP)
* **cisco.aci.aci_vrf** : Manage contexts or VRFs (fv:Ctx)
* **cisco.aci.aci_vzany_to_contract** : Attach contracts to vzAny (vz:RsAnyToProv, vz:RsAnyToCons, vz:RsAnyToConsIf)

## `cisco.asa` collection

* **cisco.asa.asa_acls** : Access-Lists resource module
* **cisco.asa.asa_command** : Run arbitrary commands on Cisco ASA devices
* **cisco.asa.asa_config** : Manage configuration sections on Cisco ASA devices
* **cisco.asa.asa_facts** : Collect facts from remote devices running Cisco ASA
* **cisco.asa.asa_ogs** : Object Group resource module

## `cisco.dnac` collection

* **cisco.dnac.app_policy_default_info** : Information module for App Policy Default
* **cisco.dnac.app_policy_info** : Information module for App Policy
* **cisco.dnac.app_policy_intent_create** : Resource module for App Policy Intent Create
* **cisco.dnac.app_policy_queuing_profile** : Resource module for App Policy Queuing Profile
* **cisco.dnac.app_policy_queuing_profile_count_info** : Information module for App Policy Queuing Profile Count
* **cisco.dnac.app_policy_queuing_profile_info** : Information module for App Policy Queuing Profile
* **cisco.dnac.application_sets** : Resource module for Application Sets
* **cisco.dnac.application_sets_count_info** : Information module for Application Sets Count
* **cisco.dnac.application_sets_info** : Information module for Application Sets
* **cisco.dnac.applications** : Resource module for Applications
* **cisco.dnac.applications_count_info** : Information module for Applications Count
* **cisco.dnac.applications_health_info** : Information module for Applications Health
* **cisco.dnac.applications_info** : Information module for Applications
* **cisco.dnac.assign_device_to_site** : Resource module for Assign Device To Site
* **cisco.dnac.associate_site_to_network_profile** : Resource module for Associate Site To Network Profile
* **cisco.dnac.authentication_import_certificate** : Resource module for Authentication Import Certificate
* **cisco.dnac.authentication_import_certificate_p12** : Resource module for Authentication Import Certificate P12
* **cisco.dnac.buildings_planned_access_points_info** : Information module for Buildings Planned Access Points
* **cisco.dnac.business_sda_hostonboarding_ssid_ippool** : Resource module for Business Sda Hostonboarding Ssid Ippool
* **cisco.dnac.business_sda_hostonboarding_ssid_ippool_info** : Information module for Business Sda Hostonboarding Ssid Ippool
* **cisco.dnac.business_sda_virtual_network_summary_info** : Information module for Business Sda Virtual Network Summary
* **cisco.dnac.business_sda_wireless_controller_create** : Resource module for Business Sda Wireless Controller Create
* **cisco.dnac.business_sda_wireless_controller_delete** : Resource module for Business Sda Wireless Controller Delete
* **cisco.dnac.cli_credential** : Resource module for Cli Credential
* **cisco.dnac.client_detail_info** : Information module for Client Detail
* **cisco.dnac.client_enrichment_details_info** : Information module for Client Enrichment Details
* **cisco.dnac.client_health_info** : Information module for Client Health
* **cisco.dnac.client_proximity_info** : Information module for Client Proximity
* **cisco.dnac.command_runner_run_command** : Resource module for Command Runner Run Command
* **cisco.dnac.compliance_check_run** : Resource module for Compliance Check Run
* **cisco.dnac.compliance_device_by_id_info** : Information module for Compliance Device By Id
* **cisco.dnac.compliance_device_details_count_info** : Information module for Compliance Device Details Count
* **cisco.dnac.compliance_device_details_info** : Information module for Compliance Device Details
* **cisco.dnac.compliance_device_info** : Information module for Compliance Device
* **cisco.dnac.compliance_device_status_count_info** : Information module for Compliance Device Status Count
* **cisco.dnac.configuration_template** : Resource module for Configuration Template
* **cisco.dnac.configuration_template_clone** : Resource module for Configuration Template Clone
* **cisco.dnac.configuration_template_create** : Resource module for Configuration Template Create
* **cisco.dnac.configuration_template_deploy** : Resource module for Configuration Template Deploy
* **cisco.dnac.configuration_template_deploy_status_info** : Information module for Configuration Template Deploy Status
* **cisco.dnac.configuration_template_deploy_v2** : Resource module for Configuration Template Deploy V2
* **cisco.dnac.configuration_template_export_project** : Resource module for Configuration Template Export Project
* **cisco.dnac.configuration_template_export_template** : Resource module for Configuration Template Export Template
* **cisco.dnac.configuration_template_import_project** : Resource module for Configuration Template Import Project
* **cisco.dnac.configuration_template_import_template** : Resource module for Configuration Template Import Template
* **cisco.dnac.configuration_template_info** : Information module for Configuration Template
* **cisco.dnac.configuration_template_project** : Resource module for Configuration Template Project
* **cisco.dnac.configuration_template_project_info** : Information module for Configuration Template Project
* **cisco.dnac.configuration_template_version_create** : Resource module for Configuration Template Version Create
* **cisco.dnac.configuration_template_version_info** : Information module for Configuration Template Version
* **cisco.dnac.device_configurations_export** : Resource module for Device Configurations Export
* **cisco.dnac.device_credential_create** : Resource module for Device Credential Create
* **cisco.dnac.device_credential_delete** : Resource module for Device Credential Delete
* **cisco.dnac.device_credential_info** : Information module for Device Credential
* **cisco.dnac.device_credential_update** : Resource module for Device Credential Update
* **cisco.dnac.device_details_info** : Information module for Device Details
* **cisco.dnac.device_enrichment_details_info** : Information module for Device Enrichment Details
* **cisco.dnac.device_family_identifiers_details_info** : Information module for Device Family Identifiers Details
* **cisco.dnac.device_health_info** : Information module for Device Health
* **cisco.dnac.device_interface_by_ip_info** : Information module for Device Interface By Ip
* **cisco.dnac.device_interface_count_info** : Information module for Device Interface Count
* **cisco.dnac.device_interface_info** : Information module for Device Interface
* **cisco.dnac.device_interface_isis_info** : Information module for Device Interface Isis
* **cisco.dnac.device_interface_ospf_info** : Information module for Device Interface Ospf
* **cisco.dnac.device_replacement** : Resource module for Device Replacement
* **cisco.dnac.device_replacement_count_info** : Information module for Device Replacement Count
* **cisco.dnac.device_replacement_deploy** : Resource module for Device Replacement Deploy
* **cisco.dnac.device_replacement_info** : Information module for Device Replacement
* **cisco.dnac.disassociate_site_to_network_profile** : Resource module for Disassociate Site To Network Profile
* **cisco.dnac.disasterrecovery_system_operationstatus_info** : Information module for Disasterrecovery System Operationstatus
* **cisco.dnac.disasterrecovery_system_status_info** : Information module for Disasterrecovery System Status
* **cisco.dnac.discovery** : Resource module for Discovery
* **cisco.dnac.discovery_count_info** : Information module for Discovery Count
* **cisco.dnac.discovery_device_count_info** : Information module for Discovery Device Count
* **cisco.dnac.discovery_device_info** : Information module for Discovery Device
* **cisco.dnac.discovery_device_range_info** : Information module for Discovery Device Range
* **cisco.dnac.discovery_info** : Information module for Discovery
* **cisco.dnac.discovery_job_info** : Information module for Discovery Job
* **cisco.dnac.discovery_range_delete** : Resource module for Discovery Range Delete
* **cisco.dnac.discovery_range_info** : Information module for Discovery Range
* **cisco.dnac.discovery_summary_info** : Information module for Discovery Summary
* **cisco.dnac.dna_command_runner_keywords_info** : Information module for Dna Command Runner Keywords
* **cisco.dnac.dnacaap_management_execution_status_info** : Information module for Dnacaap Management Execution Status
* **cisco.dnac.endpoint_analytics_profiling_rules** : Resource module for Endpoint Analytics Profiling Rules
* **cisco.dnac.endpoint_analytics_profiling_rules_info** : Information module for Endpoint Analytics Profiling Rules
* **cisco.dnac.event_api_status_info** : Information module for Event Api Status
* **cisco.dnac.event_artifact_count_info** : Information module for Event Artifact Count
* **cisco.dnac.event_artifact_info** : Information module for Event Artifact
* **cisco.dnac.event_config_connector_types_info** : Information module for Event Config Connector Types
* **cisco.dnac.event_count_info** : Information module for Event Count
* **cisco.dnac.event_email_config_create** : Resource module for Event Email Config Create
* **cisco.dnac.event_email_config_update** : Resource module for Event Email Config Update
* **cisco.dnac.event_info** : Information module for Event
* **cisco.dnac.event_series_audit_logs_info** : Information module for Event Series Audit Logs
* **cisco.dnac.event_series_audit_logs_parent_records_info** : Information module for Event Series Audit Logs Parent Records
* **cisco.dnac.event_series_audit_logs_summary_info** : Information module for Event Series Audit Logs Summary
* **cisco.dnac.event_series_count_info** : Information module for Event Series Count
* **cisco.dnac.event_series_info** : Information module for Event Series
* **cisco.dnac.event_subscription** : Resource module for Event Subscription
* **cisco.dnac.event_subscription_count_info** : Information module for Event Subscription Count
* **cisco.dnac.event_subscription_details_email_info** : Information module for Event Subscription Details Email
* **cisco.dnac.event_subscription_details_rest_info** : Information module for Event Subscription Details Rest
* **cisco.dnac.event_subscription_details_syslog_info** : Information module for Event Subscription Details Syslog
* **cisco.dnac.event_subscription_email** : Resource module for Event Subscription Email
* **cisco.dnac.event_subscription_email_info** : Information module for Event Subscription Email
* **cisco.dnac.event_subscription_info** : Information module for Event Subscription
* **cisco.dnac.event_subscription_rest** : Resource module for Event Subscription Rest
* **cisco.dnac.event_subscription_rest_info** : Information module for Event Subscription Rest
* **cisco.dnac.event_subscription_syslog** : Resource module for Event Subscription Syslog
* **cisco.dnac.event_subscription_syslog_info** : Information module for Event Subscription Syslog
* **cisco.dnac.event_webhook_create** : Resource module for Event Webhook Create
* **cisco.dnac.event_webhook_update** : Resource module for Event Webhook Update
* **cisco.dnac.file_import** : Resource module for File Import
* **cisco.dnac.file_info** : Information module for File
* **cisco.dnac.file_namespace_files_info** : Information module for File Namespace Files
* **cisco.dnac.file_namespaces_info** : Information module for File Namespaces
* **cisco.dnac.global_credential_delete** : Resource module for Global Credential Delete
* **cisco.dnac.global_credential_info** : Information module for Global Credential
* **cisco.dnac.global_credential_update** : Resource module for Global Credential Update
* **cisco.dnac.global_pool** : Resource module for Global Pool
* **cisco.dnac.global_pool_info** : Information module for Global Pool
* **cisco.dnac.golden_image_create** : Resource module for Golden Image Create
* **cisco.dnac.golden_tag_image_delete** : Resource module for Golden Tag Image Delete
* **cisco.dnac.golden_tag_image_details_info** : Information module for Golden Tag Image Details
* **cisco.dnac.http_read_credential** : Resource module for Http Read Credential
* **cisco.dnac.http_write_credential** : Resource module for Http Write Credential
* **cisco.dnac.interface_info** : Information module for Interface
* **cisco.dnac.interface_network_device_detail_info** : Information module for Interface Network Device Detail
* **cisco.dnac.interface_network_device_info** : Information module for Interface Network Device
* **cisco.dnac.interface_network_device_range_info** : Information module for Interface Network Device Range
* **cisco.dnac.interface_operation_create** : Resource module for Interface Operation Create
* **cisco.dnac.interface_update** : Resource module for Interface Update
* **cisco.dnac.issues_enrichment_details_info** : Information module for Issues Enrichment Details
* **cisco.dnac.issues_info** : Information module for Issues
* **cisco.dnac.itsm_cmdb_sync_status_info** : Information module for Itsm Cmdb Sync Status
* **cisco.dnac.itsm_integration_events_failed_info** : Information module for Itsm Integration Events Failed
* **cisco.dnac.itsm_integration_events_retry** : Resource module for Itsm Integration Events Retry
* **cisco.dnac.lan_automation_count_info** : Information module for Lan Automation Count
* **cisco.dnac.lan_automation_create** : Resource module for Lan Automation Create
* **cisco.dnac.lan_automation_delete** : Resource module for Lan Automation Delete
* **cisco.dnac.lan_automation_log_info** : Information module for Lan Automation Log
* **cisco.dnac.lan_automation_status_info** : Information module for Lan Automation Status
* **cisco.dnac.license_device_count_info** : Information module for License Device Count
* **cisco.dnac.license_device_deregistration** : Resource module for License Device Deregistration
* **cisco.dnac.license_device_license_details_info** : Information module for License Device License Details
* **cisco.dnac.license_device_license_summary_info** : Information module for License Device License Summary
* **cisco.dnac.license_device_registration** : Resource module for License Device Registration
* **cisco.dnac.license_smart_account_details_info** : Information module for License Smart Account Details
* **cisco.dnac.license_term_details_info** : Information module for License Term Details
* **cisco.dnac.license_usage_details_info** : Information module for License Usage Details
* **cisco.dnac.license_virtual_account_change** : Resource module for License Virtual Account Change
* **cisco.dnac.license_virtual_account_details_info** : Information module for License Virtual Account Details
* **cisco.dnac.netconf_credential** : Resource module for Netconf Credential
* **cisco.dnac.network_create** : Resource module for Network Create
* **cisco.dnac.network_device** : Resource module for Network Device
* **cisco.dnac.network_device_by_ip_info** : Information module for Network Device By Ip
* **cisco.dnac.network_device_by_serial_number_info** : Information module for Network Device By Serial Number
* **cisco.dnac.network_device_chassis_details_info** : Information module for Network Device Chassis Details
* **cisco.dnac.network_device_config_count_info** : Information module for Network Device Config Count
* **cisco.dnac.network_device_config_info** : Information module for Network Device Config
* **cisco.dnac.network_device_count_info** : Information module for Network Device Count
* **cisco.dnac.network_device_custom_prompt** : Resource module for Network Device Custom Prompt
* **cisco.dnac.network_device_custom_prompt_info** : Information module for Network Device Custom Prompt
* **cisco.dnac.network_device_equipment_info** : Information module for Network Device Equipment
* **cisco.dnac.network_device_export** : Resource module for Network Device Export
* **cisco.dnac.network_device_functional_capability_info** : Information module for Network Device Functional Capability
* **cisco.dnac.network_device_global_polling_interval_info** : Information module for Network Device Global Polling Interval
* **cisco.dnac.network_device_info** : Information module for Network Device
* **cisco.dnac.network_device_interface_neighbor_info** : Information module for Network Device Interface Neighbor
* **cisco.dnac.network_device_interface_poe_info** : Information module for Network Device Interface Poe
* **cisco.dnac.network_device_inventory_insight_link_mismatch_info** : Information module for Network Device Inventory Insight Link Mismatch
* **cisco.dnac.network_device_lexicographically_sorted_info** : Information module for Network Device Lexicographically Sorted
* **cisco.dnac.network_device_linecard_details_info** : Information module for Network Device Linecard Details
* **cisco.dnac.network_device_meraki_organization_info** : Information module for Network Device Meraki Organization
* **cisco.dnac.network_device_module_count_info** : Information module for Network Device Module Count
* **cisco.dnac.network_device_module_info** : Information module for Network Device Module
* **cisco.dnac.network_device_poe_info** : Information module for Network Device Poe
* **cisco.dnac.network_device_polling_interval_info** : Information module for Network Device Polling Interval
* **cisco.dnac.network_device_range_info** : Information module for Network Device Range
* **cisco.dnac.network_device_register_for_wsa_info** : Information module for Network Device Register For Wsa
* **cisco.dnac.network_device_stack_details_info** : Information module for Network Device Stack Details
* **cisco.dnac.network_device_summary_info** : Information module for Network Device Summary
* **cisco.dnac.network_device_supervisor_card_details_info** : Information module for Network Device Supervisor Card Details
* **cisco.dnac.network_device_sync** : Resource module for Network Device Sync
* **cisco.dnac.network_device_update_role** : Resource module for Network Device Update Role
* **cisco.dnac.network_device_vlan_info** : Information module for Network Device Vlan
* **cisco.dnac.network_device_wireless_lan_info** : Information module for Network Device Wireless Lan
* **cisco.dnac.network_device_with_snmp_v3_des_info** : Information module for Network Device With Snmp V3 Des
* **cisco.dnac.network_info** : Information module for Network
* **cisco.dnac.network_update** : Resource module for Network Update
* **cisco.dnac.nfv_profile** : Resource module for Nfv Profile
* **cisco.dnac.nfv_profile_info** : Information module for Nfv Profile
* **cisco.dnac.nfv_provision** : Resource module for Nfv Provision
* **cisco.dnac.nfv_provision_detail_info** : Information module for Nfv Provision Detail
* **cisco.dnac.nfv_provision_details** : Resource module for Nfv Provision Details
* **cisco.dnac.path_trace** : Resource module for Path Trace
* **cisco.dnac.path_trace_info** : Information module for Path Trace
* **cisco.dnac.planned_access_points_info** : Information module for Planned Access Points
* **cisco.dnac.platform_nodes_configuration_summary_info** : Information module for Platform Nodes Configuration Summary
* **cisco.dnac.platform_release_summary_info** : Information module for Platform Release Summary
* **cisco.dnac.pnp_device** : Resource module for Pnp Device
* **cisco.dnac.pnp_device_authorize** : Resource module for Pnp Device Authorize
* **cisco.dnac.pnp_device_claim** : Resource module for Pnp Device Claim
* **cisco.dnac.pnp_device_claim_to_site** : Resource module for Pnp Device Claim To Site
* **cisco.dnac.pnp_device_config_preview** : Resource module for Pnp Device Config Preview
* **cisco.dnac.pnp_device_count_info** : Information module for Pnp Device Count
* **cisco.dnac.pnp_device_history_info** : Information module for Pnp Device History
* **cisco.dnac.pnp_device_import** : Resource module for Pnp Device Import
* **cisco.dnac.pnp_device_info** : Information module for Pnp Device
* **cisco.dnac.pnp_device_reset** : Resource module for Pnp Device Reset
* **cisco.dnac.pnp_device_unclaim** : Resource module for Pnp Device Unclaim
* **cisco.dnac.pnp_global_settings** : Resource module for Pnp Global Settings
* **cisco.dnac.pnp_global_settings_info** : Information module for Pnp Global Settings
* **cisco.dnac.pnp_intent** : Resource module for Site and PnP related functions
* **cisco.dnac.pnp_server_profile_update** : Resource module for Pnp Server Profile Update
* **cisco.dnac.pnp_smart_account_domains_info** : Information module for Pnp Smart Account Domains
* **cisco.dnac.pnp_virtual_account_add** : Resource module for Pnp Virtual Account Add
* **cisco.dnac.pnp_virtual_account_deregister** : Resource module for Pnp Virtual Account Deregister
* **cisco.dnac.pnp_virtual_account_devices_sync** : Resource module for Pnp Virtual Account Devices Sync
* **cisco.dnac.pnp_virtual_account_sync_result_info** : Information module for Pnp Virtual Account Sync Result
* **cisco.dnac.pnp_virtual_accounts_info** : Information module for Pnp Virtual Accounts
* **cisco.dnac.pnp_workflow** : Resource module for Pnp Workflow
* **cisco.dnac.pnp_workflow_count_info** : Information module for Pnp Workflow Count
* **cisco.dnac.pnp_workflow_info** : Information module for Pnp Workflow
* **cisco.dnac.profiling_rules_count_info** : Information module for Profiling Rules Count
* **cisco.dnac.profiling_rules_in_bulk_create** : Resource module for Profiling Rules In Bulk Create
* **cisco.dnac.projects_details_info** : Information module for Projects Details
* **cisco.dnac.qos_device_interface** : Resource module for Qos Device Interface
* **cisco.dnac.qos_device_interface_info** : Information module for Qos Device Interface
* **cisco.dnac.qos_device_interface_info_count_info** : Information module for Qos Device Interface Info Count
* **cisco.dnac.reports** : Resource module for Reports
* **cisco.dnac.reports_executions_info** : Information module for Reports Executions
* **cisco.dnac.reports_info** : Information module for Reports
* **cisco.dnac.reports_view_group_info** : Information module for Reports View Group
* **cisco.dnac.reports_view_group_view_info** : Information module for Reports View Group View
* **cisco.dnac.reserve_ip_subpool** : Resource module for Reserve Ip Subpool
* **cisco.dnac.reserve_ip_subpool_create** : Resource module for Reserve Ip Subpool Create
* **cisco.dnac.reserve_ip_subpool_delete** : Resource module for Reserve Ip Subpool Delete
* **cisco.dnac.reserve_ip_subpool_info** : Information module for Reserve Ip Subpool
* **cisco.dnac.reserve_ip_subpool_update** : Resource module for Reserve Ip Subpool Update
* **cisco.dnac.sda_count_info** : Information module for Sda Count
* **cisco.dnac.sda_device_info** : Information module for Sda Device
* **cisco.dnac.sda_device_role_info** : Information module for Sda Device Role
* **cisco.dnac.sda_fabric** : Resource module for Sda Fabric
* **cisco.dnac.sda_fabric_authentication_profile** : Resource module for Sda Fabric Authentication Profile
* **cisco.dnac.sda_fabric_authentication_profile_info** : Information module for Sda Fabric Authentication Profile
* **cisco.dnac.sda_fabric_border_device** : Resource module for Sda Fabric Border Device
* **cisco.dnac.sda_fabric_border_device_info** : Information module for Sda Fabric Border Device
* **cisco.dnac.sda_fabric_control_plane_device** : Resource module for Sda Fabric Control Plane Device
* **cisco.dnac.sda_fabric_control_plane_device_info** : Information module for Sda Fabric Control Plane Device
* **cisco.dnac.sda_fabric_edge_device** : Resource module for Sda Fabric Edge Device
* **cisco.dnac.sda_fabric_edge_device_info** : Information module for Sda Fabric Edge Device
* **cisco.dnac.sda_fabric_info** : Information module for Sda Fabric
* **cisco.dnac.sda_fabric_site** : Resource module for Sda Fabric Site
* **cisco.dnac.sda_fabric_site_info** : Information module for Sda Fabric Site
* **cisco.dnac.sda_multicast** : Resource module for Sda Multicast
* **cisco.dnac.sda_multicast_info** : Information module for Sda Multicast
* **cisco.dnac.sda_port_assignment_for_access_point** : Resource module for Sda Port Assignment For Access Point
* **cisco.dnac.sda_port_assignment_for_access_point_info** : Information module for Sda Port Assignment For Access Point
* **cisco.dnac.sda_port_assignment_for_user_device** : Resource module for Sda Port Assignment For User Device
* **cisco.dnac.sda_port_assignment_for_user_device_info** : Information module for Sda Port Assignment For User Device
* **cisco.dnac.sda_provision_device** : Resource module for Sda Provision Device
* **cisco.dnac.sda_provision_device_info** : Information module for Sda Provision Device
* **cisco.dnac.sda_virtual_network** : Resource module for Sda Virtual Network
* **cisco.dnac.sda_virtual_network_info** : Information module for Sda Virtual Network
* **cisco.dnac.sda_virtual_network_ip_pool** : Resource module for Sda Virtual Network Ip Pool
* **cisco.dnac.sda_virtual_network_ip_pool_info** : Information module for Sda Virtual Network Ip Pool
* **cisco.dnac.sda_virtual_network_v2** : Resource module for Sda Virtual Network V2
* **cisco.dnac.sda_virtual_network_v2_info** : Information module for Sda Virtual Network V2
* **cisco.dnac.security_advisories_devices_info** : Information module for Security Advisories Devices
* **cisco.dnac.security_advisories_ids_per_device_info** : Information module for Security Advisories Ids Per Device
* **cisco.dnac.security_advisories_info** : Information module for Security Advisories
* **cisco.dnac.security_advisories_per_device_info** : Information module for Security Advisories Per Device
* **cisco.dnac.security_advisories_summary_info** : Information module for Security Advisories Summary
* **cisco.dnac.sensor** : Resource module for Sensor
* **cisco.dnac.sensor_info** : Information module for Sensor
* **cisco.dnac.sensor_test_run** : Resource module for Sensor Test Run
* **cisco.dnac.sensor_test_template_duplicate** : Resource module for Sensor Test Template Duplicate
* **cisco.dnac.sensor_test_template_edit** : Resource module for Sensor Test Template Edit
* **cisco.dnac.service_provider_create** : Resource module for Service Provider Create
* **cisco.dnac.service_provider_info** : Information module for Service Provider
* **cisco.dnac.service_provider_profile_delete** : Resource module for Service Provider Profile Delete
* **cisco.dnac.service_provider_update** : Resource module for Service Provider Update
* **cisco.dnac.site_assign_credential** : Resource module for Site Assign Credential
* **cisco.dnac.site_assign_device** : Resource module for Site Assign Device
* **cisco.dnac.site_count_info** : Information module for Site Count
* **cisco.dnac.site_create** : Resource module for Site Create
* **cisco.dnac.site_delete** : Resource module for Site Delete
* **cisco.dnac.site_design_floormap** : Resource module for Site Design Floormap
* **cisco.dnac.site_design_floormap_info** : Information module for Site Design Floormap
* **cisco.dnac.site_health_info** : Information module for Site Health
* **cisco.dnac.site_info** : Information module for Site
* **cisco.dnac.site_intent** : Resource module for Site operations
* **cisco.dnac.site_membership_info** : Information module for Site Membership
* **cisco.dnac.site_update** : Resource module for Site Update
* **cisco.dnac.snmp_properties** : Resource module for Snmp Properties
* **cisco.dnac.snmp_properties_info** : Information module for Snmp Properties
* **cisco.dnac.snmpv2_read_community_credential** : Resource module for Snmpv2 Read Community Credential
* **cisco.dnac.snmpv2_write_community_credential** : Resource module for Snmpv2 Write Community Credential
* **cisco.dnac.snmpv3_credential** : Resource module for Snmpv3 Credential
* **cisco.dnac.swim_image_details_info** : Information module for Swim Image Details
* **cisco.dnac.swim_import_local** : Resource module for Swim Import Local
* **cisco.dnac.swim_import_via_url** : Resource module for Swim Import Via Url
* **cisco.dnac.swim_intent** : Intent module for SWIM related functions
* **cisco.dnac.swim_trigger_activation** : Resource module for Swim Trigger Activation
* **cisco.dnac.swim_trigger_distribution** : Resource module for Swim Trigger Distribution
* **cisco.dnac.syslog_config_create** : Resource module for Syslog Config Create
* **cisco.dnac.syslog_config_update** : Resource module for Syslog Config Update
* **cisco.dnac.system_health_count_info** : Information module for System Health Count
* **cisco.dnac.system_health_info** : Information module for System Health
* **cisco.dnac.system_performance_historical_info** : Information module for System Performance Historical
* **cisco.dnac.system_performance_info** : Information module for System Performance
* **cisco.dnac.tag** : Resource module for Tag
* **cisco.dnac.tag_count_info** : Information module for Tag Count
* **cisco.dnac.tag_info** : Information module for Tag
* **cisco.dnac.tag_member** : Resource module for Tag Member
* **cisco.dnac.tag_member_count_info** : Information module for Tag Member Count
* **cisco.dnac.tag_member_info** : Information module for Tag Member
* **cisco.dnac.tag_member_type_info** : Information module for Tag Member Type
* **cisco.dnac.tag_membership** : Resource module for Tag Membership
* **cisco.dnac.task_count_info** : Information module for Task Count
* **cisco.dnac.task_info** : Information module for Task
* **cisco.dnac.task_operation_info** : Information module for Task Operation
* **cisco.dnac.task_tree_info** : Information module for Task Tree
* **cisco.dnac.template_intent** : Resource module for Template functions
* **cisco.dnac.template_preview** : Resource module for Template Preview
* **cisco.dnac.templates_details_info** : Information module for Templates Details
* **cisco.dnac.threat_detail** : Resource module for Threat Detail
* **cisco.dnac.threat_detail_count** : Resource module for Threat Detail Count
* **cisco.dnac.threat_summary** : Resource module for Threat Summary
* **cisco.dnac.topology_layer_2_info** : Information module for Topology Layer 2
* **cisco.dnac.topology_layer_3_info** : Information module for Topology Layer 3
* **cisco.dnac.topology_network_health_info** : Information module for Topology Network Health
* **cisco.dnac.topology_physical_info** : Information module for Topology Physical
* **cisco.dnac.topology_site_info** : Information module for Topology Site
* **cisco.dnac.topology_vlan_details_info** : Information module for Topology Vlan Details
* **cisco.dnac.transit_peer_network** : Resource module for Transit Peer Network
* **cisco.dnac.transit_peer_network_info** : Information module for Transit Peer Network
* **cisco.dnac.user_enrichment_details_info** : Information module for User Enrichment Details
* **cisco.dnac.wireless_dynamic_interface** : Resource module for Wireless Dynamic Interface
* **cisco.dnac.wireless_dynamic_interface_info** : Information module for Wireless Dynamic Interface
* **cisco.dnac.wireless_enterprise_ssid** : Resource module for Wireless Enterprise Ssid
* **cisco.dnac.wireless_enterprise_ssid_info** : Information module for Wireless Enterprise Ssid
* **cisco.dnac.wireless_profile** : Resource module for Wireless Profile
* **cisco.dnac.wireless_profile_info** : Information module for Wireless Profile
* **cisco.dnac.wireless_provision_access_point** : Resource module for Wireless Provision Access Point
* **cisco.dnac.wireless_provision_device_create** : Resource module for Wireless Provision Device Create
* **cisco.dnac.wireless_provision_device_update** : Resource module for Wireless Provision Device Update
* **cisco.dnac.wireless_provision_ssid_create_provision** : Resource module for Wireless Provision Ssid Create Provision
* **cisco.dnac.wireless_provision_ssid_delete_reprovision** : Resource module for Wireless Provision Ssid Delete Reprovision
* **cisco.dnac.wireless_psk_override** : Resource module for Wireless Psk Override
* **cisco.dnac.wireless_rf_profile** : Resource module for Wireless Rf Profile
* **cisco.dnac.wireless_rf_profile_info** : Information module for Wireless Rf Profile
* **cisco.dnac.wireless_sensor_test_results_info** : Information module for Wireless Sensor Test Results

## `cisco.intersight` collection

* **cisco.intersight.intersight_boot_order_policy** : Boot Order policy configuration for Cisco Intersight
* **cisco.intersight.intersight_imc_access_policy** : IMC Access Policy configuration for Cisco Intersight
* **cisco.intersight.intersight_info** : Gather information about Intersight
* **cisco.intersight.intersight_local_user_policy** : Local User Policy configuration for Cisco Intersight
* **cisco.intersight.intersight_ntp_policy** : NTP policy configuration for Cisco Intersight
* **cisco.intersight.intersight_rest_api** : REST API configuration for Cisco Intersight
* **cisco.intersight.intersight_server_profile** : Server Profile configuration for Cisco Intersight
* **cisco.intersight.intersight_target_claim** : Target claim configuraiton for Cisco Intersight
* **cisco.intersight.intersight_virtual_media_policy** : Virtual Media policy configuration for Cisco Intersight

## `cisco.ios` collection

* **cisco.ios.ios_acl_interfaces** : Resource module to configure ACL interfaces.
* **cisco.ios.ios_acls** : Resource module to configure ACLs.
* **cisco.ios.ios_banner** : Module to configure multiline banners.
* **cisco.ios.ios_bgp_address_family** : Resource module to configure BGP Address family.
* **cisco.ios.ios_bgp_global** : Resource module to configure BGP.
* **cisco.ios.ios_command** : Module to run commands on remote devices.
* **cisco.ios.ios_config** : Module to manage configuration sections.
* **cisco.ios.ios_facts** : Module to collect facts from remote devices.
* **cisco.ios.ios_hostname** : Resource module to configure hostname.
* **cisco.ios.ios_interfaces** : Resource module to configure interfaces.
* **cisco.ios.ios_l2_interfaces** : Resource Module to configure L2 interfaces.
* **cisco.ios.ios_l3_interfaces** : Resource module to configure L3 interfaces.
* **cisco.ios.ios_lacp** : Resource module to configure LACP.
* **cisco.ios.ios_lacp_interfaces** : Resource module to configure LACP interfaces.
* **cisco.ios.ios_lag_interfaces** : Resource module to configure LAG interfaces.
* **cisco.ios.ios_lldp_global** : Resource module to configure LLDP.
* **cisco.ios.ios_lldp_interfaces** : Resource module to configure LLDP interfaces.
* **cisco.ios.ios_logging_global** : Resource module to configure logging.
* **cisco.ios.ios_ntp_global** : Resource module to configure NTP.
* **cisco.ios.ios_ospf_interfaces** : Resource module to configure OSPF interfaces.
* **cisco.ios.ios_ospfv2** : Resource module to configure OSPFv2.
* **cisco.ios.ios_ospfv3** : Resource module to configure OSPFv3.
* **cisco.ios.ios_ping** : Tests reachability using ping from IOS switch.
* **cisco.ios.ios_prefix_lists** : Resource module to configure prefix lists.
* **cisco.ios.ios_route_maps** : Resource module to configure route maps.
* **cisco.ios.ios_snmp_server** : Resource module to configure snmp server.
* **cisco.ios.ios_static_routes** : Resource module to configure static routes.
* **cisco.ios.ios_system** : Module to manage the system attributes.
* **cisco.ios.ios_user** : Module to manage the aggregates of local users.
* **cisco.ios.ios_vlans** : Resource module to configure VLANs.
* **cisco.ios.ios_vrf** : Module to configure VRF definitions.

## `cisco.iosxr` collection

* **cisco.iosxr.iosxr_acl_interfaces** : Resource module to configure ACL interfaces.
* **cisco.iosxr.iosxr_acls** : Resource module to configure ACLs.
* **cisco.iosxr.iosxr_banner** : Module to configure multiline banners.
* **cisco.iosxr.iosxr_bgp_address_family** : Resource module to configure BGP Address family.
* **cisco.iosxr.iosxr_bgp_global** : Resource module to configure BGP.
* **cisco.iosxr.iosxr_bgp_neighbor_address_family** : Resource module to configure BGP Neighbor Address family.
* **cisco.iosxr.iosxr_command** : Module to run commands on remote devices.
* **cisco.iosxr.iosxr_config** : Module to manage configuration sections.
* **cisco.iosxr.iosxr_facts** : Module to collect facts from remote devices.
* **cisco.iosxr.iosxr_hostname** : Resource module to configure hostname.
* **cisco.iosxr.iosxr_interfaces** : Resource module to configure interfaces.
* **cisco.iosxr.iosxr_l2_interfaces** : Resource Module to configure L2 interfaces.
* **cisco.iosxr.iosxr_l3_interfaces** : Resource module to configure L3 interfaces.
* **cisco.iosxr.iosxr_lacp** : Resource module to configure LACP.
* **cisco.iosxr.iosxr_lacp_interfaces** : Resource module to configure LACP interfaces.
* **cisco.iosxr.iosxr_lag_interfaces** : Resource module to configure LAG interfaces.
* **cisco.iosxr.iosxr_lldp_global** : Resource module to configure LLDP.
* **cisco.iosxr.iosxr_lldp_interfaces** : Resource module to configure LLDP interfaces.
* **cisco.iosxr.iosxr_logging_global** : Resource module to configure logging.
* **cisco.iosxr.iosxr_netconf** : Configures NetConf sub-system service on Cisco IOS-XR devices
* **cisco.iosxr.iosxr_ntp_global** : Resource module to configure NTP.
* **cisco.iosxr.iosxr_ospf_interfaces** : Resource module to configure OSPF interfaces.
* **cisco.iosxr.iosxr_ospfv2** : Resource module to configure OSPFv2.
* **cisco.iosxr.iosxr_ospfv3** : Resource module to configure OSPFv3.
* **cisco.iosxr.iosxr_ping** : Tests reachability using ping from IOSXR switch.
* **cisco.iosxr.iosxr_prefix_lists** : Resource module to configure prefix lists.
* **cisco.iosxr.iosxr_snmp_server** : Resource module to configure snmp server.
* **cisco.iosxr.iosxr_static_routes** : Resource module to configure static routes.
* **cisco.iosxr.iosxr_system** : Module to manage the system attributes.
* **cisco.iosxr.iosxr_user** : Module to manage the aggregates of local users.

## `cisco.ise` collection

* **cisco.ise.aci_bindings_info** : Information module for ACI Bindings
* **cisco.ise.aci_settings** : Resource module for ACI Settings
* **cisco.ise.aci_settings_info** : Information module for ACI Settings
* **cisco.ise.aci_test_connectivity** : Resource module for ACI Test Connectivity
* **cisco.ise.active_directory** : Resource module for Active Directory
* **cisco.ise.active_directory_add_groups** : Resource module for Active Directory Add Groups
* **cisco.ise.active_directory_groups_by_domain_info** : Information module for Active Directory Groups By Domain
* **cisco.ise.active_directory_info** : Information module for Active Directory
* **cisco.ise.active_directory_is_user_member_of_group_info** : Information module for Active Directory Is User Member Of Group
* **cisco.ise.active_directory_join_domain** : Resource module for Active Directory Join Domain
* **cisco.ise.active_directory_join_domain_with_all_nodes** : Resource module for Active Directory Join Domain With All Nodes
* **cisco.ise.active_directory_leave_domain** : Resource module for Active Directory Leave Domain
* **cisco.ise.active_directory_leave_domain_with_all_nodes** : Resource module for Active Directory Leave Domain With All Nodes
* **cisco.ise.active_directory_trusted_domains_info** : Information module for Active Directory Trusted Domains
* **cisco.ise.active_directory_user_groups_info** : Information module for Active Directory User Groups
* **cisco.ise.admin_user_info** : Information module for Admin User
* **cisco.ise.allowed_protocols** : Resource module for Allowed Protocols
* **cisco.ise.allowed_protocols_info** : Information module for Allowed Protocols
* **cisco.ise.anc_endpoint_apply** : Resource module for ANC Endpoint Apply
* **cisco.ise.anc_endpoint_bulk_monitor_status_info** : Information module for ANC Endpoint Bulk Monitor Status
* **cisco.ise.anc_endpoint_bulk_request** : Resource module for ANC Endpoint Bulk Request
* **cisco.ise.anc_endpoint_clear** : Resource module for ANC Endpoint Clear
* **cisco.ise.anc_endpoint_info** : Information module for ANC Endpoint
* **cisco.ise.anc_policy** : Resource module for ANC Policy
* **cisco.ise.anc_policy_bulk_monitor_status_info** : Information module for ANC Policy Bulk Monitor Status
* **cisco.ise.anc_policy_bulk_request** : Resource module for ANC Policy Bulk Request
* **cisco.ise.anc_policy_info** : Information module for ANC Policy
* **cisco.ise.authorization_profile** : Resource module for Authorization Profile
* **cisco.ise.authorization_profile_info** : Information module for Authorization Profile
* **cisco.ise.backup_cancel** : Resource module for Backup Cancel
* **cisco.ise.backup_config** : Resource module for Backup Config
* **cisco.ise.backup_last_status_info** : Information module for Backup Last Status
* **cisco.ise.backup_restore** : Resource module for Backup RESTore
* **cisco.ise.backup_schedule_config** : Resource module for Backup Schedule Config
* **cisco.ise.backup_schedule_config_update** : Resource module for Backup Schedule Config Update
* **cisco.ise.bind_signed_certificate** : Resource module for Bind Signed Certificate
* **cisco.ise.byod_portal** : Resource module for BYOD Portal
* **cisco.ise.byod_portal_info** : Information module for BYOD Portal
* **cisco.ise.certificate_profile** : Resource module for Certificate Profile
* **cisco.ise.certificate_profile_info** : Information module for Certificate Profile
* **cisco.ise.certificate_template_info** : Information module for Certificate Template
* **cisco.ise.csr_delete** : Resource module for CSR Delete
* **cisco.ise.csr_export_info** : Information module for CSR Export
* **cisco.ise.csr_generate** : Resource module for CSR Generate
* **cisco.ise.csr_generate_intermediate_ca** : Resource module for CSR Generate Intermediate CA
* **cisco.ise.csr_info** : Information module for CSR
* **cisco.ise.deployment_info** : Information module for Deployment
* **cisco.ise.device_administration_authentication_reset_hitcount** : Resource module for Device Administration Authentication Reset Hitcount
* **cisco.ise.device_administration_authentication_rules** : Resource module for Device Administration Authentication Rules
* **cisco.ise.device_administration_authentication_rules_info** : Information module for Device Administration Authentication Rules
* **cisco.ise.device_administration_authorization_reset_hitcount** : Resource module for Device Administration Authorization Reset Hitcount
* **cisco.ise.device_administration_authorization_rules** : Resource module for Device Administration Authorization Rules
* **cisco.ise.device_administration_authorization_rules_info** : Information module for Device Administration Authorization Rules
* **cisco.ise.device_administration_command_set_info** : Information module for Device Administration Command Set
* **cisco.ise.device_administration_conditions** : Resource module for Device Administration Conditions
* **cisco.ise.device_administration_conditions_for_authentication_rule_info** : Information module for Device Administration Conditions For Authentication Rule
* **cisco.ise.device_administration_conditions_for_authorization_rule_info** : Information module for Device Administration Conditions For Authorization Rule
* **cisco.ise.device_administration_conditions_for_policy_set_info** : Information module for Device Administration Conditions For Policy Set
* **cisco.ise.device_administration_conditions_info** : Information module for Device Administration Conditions
* **cisco.ise.device_administration_dictionary_attributes_authentication_info** : Information module for Device Administration Dictionary Attributes Authentication
* **cisco.ise.device_administration_dictionary_attributes_authorization_info** : Information module for Device Administration Dictionary Attributes Authorization
* **cisco.ise.device_administration_dictionary_attributes_policy_set_info** : Information module for Device Administration Dictionary Attributes Policy Set
* **cisco.ise.device_administration_global_exception_rules** : Resource module for Device Administration Global Exception Rules
* **cisco.ise.device_administration_global_exception_rules_info** : Information module for Device Administration Global Exception Rules
* **cisco.ise.device_administration_global_exception_rules_reset_hitcount** : Resource module for Device Administration Global Exception Rules Reset Hitcount
* **cisco.ise.device_administration_identity_stores_info** : Information module for Device Administration Identity Stores
* **cisco.ise.device_administration_local_exception_rules** : Resource module for Device Administration Local Exception Rules
* **cisco.ise.device_administration_local_exception_rules_info** : Information module for Device Administration Local Exception Rules
* **cisco.ise.device_administration_local_exception_rules_reset_hitcount** : Resource module for Device Administration Local Exception Rules Reset Hitcount
* **cisco.ise.device_administration_network_conditions** : Resource module for Device Administration Network Conditions
* **cisco.ise.device_administration_network_conditions_info** : Information module for Device Administration Network Conditions
* **cisco.ise.device_administration_policy_set** : Resource module for Device Administration Policy Set
* **cisco.ise.device_administration_policy_set_info** : Information module for Device Administration Policy Set
* **cisco.ise.device_administration_policy_set_reset_hitcount** : Resource module for Device Administration Policy Set Reset Hitcount
* **cisco.ise.device_administration_profiles_info** : Information module for Device Administration Profiles
* **cisco.ise.device_administration_service_names_info** : Information module for Device Administration Service Names
* **cisco.ise.device_administration_time_date_conditions** : Resource module for Device Administration Time Date Conditions
* **cisco.ise.device_administration_time_date_conditions_info** : Information module for Device Administration Time Date Conditions
* **cisco.ise.downloadable_acl** : Resource module for Downloadable ACL
* **cisco.ise.downloadable_acl_info** : Information module for Downloadable ACL
* **cisco.ise.egress_matrix_cell** : Resource module for Egress Matrix Cell
* **cisco.ise.egress_matrix_cell_bulk_monitor_status_info** : Information module for Egress Matrix Cell Bulk Monitor Status
* **cisco.ise.egress_matrix_cell_bulk_request** : Resource module for Egress Matrix Cell Bulk Request
* **cisco.ise.egress_matrix_cell_clear_all** : Resource module for Egress Matrix Cell Clear All
* **cisco.ise.egress_matrix_cell_clone** : Resource module for Egress Matrix Cell Clone
* **cisco.ise.egress_matrix_cell_info** : Information module for Egress Matrix Cell
* **cisco.ise.egress_matrix_cell_set_all_status** : Resource module for Egress Matrix Cell Set All Status
* **cisco.ise.endpoint** : Resource module for Endpoint
* **cisco.ise.endpoint_bulk_monitor_status_info** : Information module for Endpoint Bulk Monitor Status
* **cisco.ise.endpoint_bulk_request** : Resource module for Endpoint Bulk Request
* **cisco.ise.endpoint_certificate** : Resource module for Endpoint Certificate
* **cisco.ise.endpoint_deregister** : Resource module for Endpoint Deregister
* **cisco.ise.endpoint_get_rejected_endpoints_info** : Information module for Endpoint Get Rejected Endpoints
* **cisco.ise.endpoint_group** : Resource module for Endpoint Group
* **cisco.ise.endpoint_group_info** : Information module for Endpoint Group
* **cisco.ise.endpoint_info** : Information module for Endpoint
* **cisco.ise.endpoint_register** : Resource module for Endpoint Register
* **cisco.ise.endpoint_release_rejected_endpoint** : Resource module for Endpoint Release Rejected Endpoint
* **cisco.ise.external_radius_server** : Resource module for External RADIUS Server
* **cisco.ise.external_radius_server_info** : Information module for External RADIUS Server
* **cisco.ise.filter_policy** : Resource module for Filter Policy
* **cisco.ise.filter_policy_info** : Information module for Filter Policy
* **cisco.ise.guest_location_info** : Information module for Guest Location
* **cisco.ise.guest_smtp_notification_settings** : Resource module for Guest SMTP Notification Settings
* **cisco.ise.guest_smtp_notification_settings_info** : Information module for Guest SMTP Notification Settings
* **cisco.ise.guest_ssid** : Resource module for Guest SSID
* **cisco.ise.guest_ssid_info** : Information module for Guest SSID
* **cisco.ise.guest_type** : Resource module for Guest Type
* **cisco.ise.guest_type_email** : Resource module for Guest Type Email
* **cisco.ise.guest_type_info** : Information module for Guest Type
* **cisco.ise.guest_type_sms** : Resource module for Guest Type SMS
* **cisco.ise.guest_user** : Resource module for Guest User
* **cisco.ise.guest_user_approve** : Resource module for Guest User Approve
* **cisco.ise.guest_user_bulk_monitor_status_info** : Information module for Guest User Bulk Monitor Status
* **cisco.ise.guest_user_bulk_request** : Resource module for Guest User Bulk Request
* **cisco.ise.guest_user_change_sponsor_password** : Resource module for Guest User Change Sponsor Password
* **cisco.ise.guest_user_deny** : Resource module for Guest User Deny
* **cisco.ise.guest_user_email** : Resource module for Guest User Email
* **cisco.ise.guest_user_info** : Information module for Guest User
* **cisco.ise.guest_user_reinstate** : Resource module for Guest User Reinstate
* **cisco.ise.guest_user_reset_password** : Resource module for Guest User Reset Password
* **cisco.ise.guest_user_sms** : Resource module for Guest User SMS
* **cisco.ise.guest_user_suspend** : Resource module for Guest User Suspend
* **cisco.ise.hotpatch_info** : Information module for Hotpatch
* **cisco.ise.hotpatch_install** : Resource module for Hotpatch Install
* **cisco.ise.hotpatch_rollback** : Resource module for Hotpatch Rollback
* **cisco.ise.hotspot_portal** : Resource module for Hotspot Portal
* **cisco.ise.hotspot_portal_info** : Information module for Hotspot Portal
* **cisco.ise.id_store_sequence** : Resource module for Id Store Sequence
* **cisco.ise.id_store_sequence_info** : Information module for Id Store Sequence
* **cisco.ise.identity_group** : Resource module for Identity Group
* **cisco.ise.identity_group_info** : Information module for Identity Group
* **cisco.ise.internal_user** : Resource module for Internal User
* **cisco.ise.internal_user_info** : Information module for Internal User
* **cisco.ise.ise_root_ca_regenerate** : Resource module for Ise Root CA Regenerate
* **cisco.ise.licensing_connection_type_info** : Information module for Licensing Connection Type
* **cisco.ise.licensing_eval_license_info** : Information module for Licensing Eval License
* **cisco.ise.licensing_feature_to_tier_mapping_info** : Information module for Licensing Feature To Tier Mapping
* **cisco.ise.licensing_registration_create** : Resource module for Licensing Registration Create
* **cisco.ise.licensing_registration_info** : Information module for Licensing Registration
* **cisco.ise.licensing_smart_state_create** : Resource module for Licensing Smart State Create
* **cisco.ise.licensing_smart_state_info** : Information module for Licensing Smart State
* **cisco.ise.licensing_tier_state_create** : Resource module for Licensing Tier State Create
* **cisco.ise.licensing_tier_state_info** : Information module for Licensing Tier State
* **cisco.ise.mnt_account_status_info** : Information module for MNT Account Status
* **cisco.ise.mnt_athentication_status_info** : Information module for Mnt Athentication Status
* **cisco.ise.mnt_authentication_status_info** : Information module for MNT Authentication Status
* **cisco.ise.mnt_failure_reasons_info** : Information module for MNT Failure Reasons
* **cisco.ise.mnt_session_active_count_info** : Information module for MNT Session Active Count
* **cisco.ise.mnt_session_active_list_info** : Information module for MNT Session Active List
* **cisco.ise.mnt_session_auth_list_info** : Information module for MNT Session Auth List
* **cisco.ise.mnt_session_by_ip_info** : Information module for MNT Session By Ip
* **cisco.ise.mnt_session_by_mac_info** : Information module for MNT Session By Mac
* **cisco.ise.mnt_session_by_nas_ip_info** : Information module for MNT Session By Nas Ip
* **cisco.ise.mnt_session_by_username_info** : Information module for MNT Session By Username
* **cisco.ise.mnt_session_delete_all** : Resource module for MNT Session Delete All
* **cisco.ise.mnt_session_disconnect_info** : Information module for MNT Session Disconnect
* **cisco.ise.mnt_session_posture_count_info** : Information module for MNT Session Posture Count
* **cisco.ise.mnt_session_profiler_count_info** : Information module for MNT Session Profiler Count
* **cisco.ise.mnt_session_reauthentication_info** : Information module for MNT Session Reauthentication
* **cisco.ise.mnt_sessions_by_session_id_info** : Information module for MNT Sessions By Session Id
* **cisco.ise.mnt_version_info** : Information module for MNT Version
* **cisco.ise.my_device_portal** : Resource module for My Device Portal
* **cisco.ise.my_device_portal_info** : Information module for My Device Portal
* **cisco.ise.native_supplicant_profile** : Resource module for Native Supplicant Profile
* **cisco.ise.native_supplicant_profile_info** : Information module for Native Supplicant Profile
* **cisco.ise.network_access_authentication_rules** : Resource module for Network Access Authentication Rules
* **cisco.ise.network_access_authentication_rules_info** : Information module for Network Access Authentication Rules
* **cisco.ise.network_access_authentication_rules_reset_hitcount** : Resource module for Network Access Authentication Rules Reset Hitcount
* **cisco.ise.network_access_authorization_rules** : Resource module for Network Access Authorization Rules
* **cisco.ise.network_access_authorization_rules_info** : Information module for Network Access Authorization Rules
* **cisco.ise.network_access_authorization_rules_reset_hitcount** : Resource module for Network Access Authorization Rules Reset Hitcount
* **cisco.ise.network_access_conditions** : Resource module for Network Access Conditions
* **cisco.ise.network_access_conditions_for_authentication_rule_info** : Information module for Network Access Conditions For Authentication Rule
* **cisco.ise.network_access_conditions_for_authorization_rule_info** : Information module for Network Access Conditions For Authorization Rule
* **cisco.ise.network_access_conditions_for_policy_set_info** : Information module for Network Access Conditions For Policy Set
* **cisco.ise.network_access_conditions_info** : Information module for Network Access Conditions
* **cisco.ise.network_access_dictionary** : Resource module for Network Access Dictionary
* **cisco.ise.network_access_dictionary_attribute** : Resource module for Network Access Dictionary Attribute
* **cisco.ise.network_access_dictionary_attribute_info** : Information module for Network Access Dictionary Attribute
* **cisco.ise.network_access_dictionary_attributes_authentication_info** : Information module for Network Access Dictionary Attributes Authentication
* **cisco.ise.network_access_dictionary_attributes_authorization_info** : Information module for Network Access Dictionary Attributes Authorization
* **cisco.ise.network_access_dictionary_attributes_policy_set_info** : Information module for Network Access Dictionary Attributes Policy Set
* **cisco.ise.network_access_dictionary_info** : Information module for Network Access Dictionary
* **cisco.ise.network_access_global_exception_rules** : Resource module for Network Access Global Exception Rules
* **cisco.ise.network_access_global_exception_rules_info** : Information module for Network Access Global Exception Rules
* **cisco.ise.network_access_global_exception_rules_reset_hitcount** : Resource module for Network Access Global Exception Rules Reset Hitcount
* **cisco.ise.network_access_identity_stores_info** : Information module for Network Access Identity Stores
* **cisco.ise.network_access_local_exception_rules** : Resource module for Network Access Local Exception Rules
* **cisco.ise.network_access_local_exception_rules_info** : Information module for Network Access Local Exception Rules
* **cisco.ise.network_access_local_exception_rules_reset_hitcounts** : Resource module for Network Access Local Exception Rules Reset Hitcounts
* **cisco.ise.network_access_network_condition** : Resource module for Network Access Network Condition
* **cisco.ise.network_access_network_condition_info** : Information module for Network Access Network Condition
* **cisco.ise.network_access_policy_set** : Resource module for Network Access Policy Set
* **cisco.ise.network_access_policy_set_info** : Information module for Network Access Policy Set
* **cisco.ise.network_access_policy_set_reset_hitcount** : Resource module for Network Access Policy Set Reset Hitcount
* **cisco.ise.network_access_profiles_info** : Information module for Network Access Profiles
* **cisco.ise.network_access_security_groups_info** : Information module for Network Access Security Groups
* **cisco.ise.network_access_service_name_info** : Information module for Network Access Service Name
* **cisco.ise.network_access_time_date_conditions** : Resource module for Network Access Time Date Conditions
* **cisco.ise.network_access_time_date_conditions_info** : Information module for Network Access Time Date Conditions
* **cisco.ise.network_device** : Resource module for Network Device
* **cisco.ise.network_device_bulk_monitor_status_info** : Information module for Network Device Bulk Monitor Status
* **cisco.ise.network_device_bulk_request** : Resource module for Network Device Bulk Request
* **cisco.ise.network_device_group** : Resource module for Network Device Group
* **cisco.ise.network_device_group_info** : Information module for Network Device Group
* **cisco.ise.network_device_info** : Information module for Network Device
* **cisco.ise.node_deployment** : Resource module for Node Deployment
* **cisco.ise.node_deployment_info** : Information module for Node Deployment
* **cisco.ise.node_deployment_sync** : Resource module for Node Deployment Sync
* **cisco.ise.node_group** : Resource module for Node Group
* **cisco.ise.node_group_info** : Information module for Node Group
* **cisco.ise.node_group_node_create** : Resource module for Node Group Node Create
* **cisco.ise.node_group_node_delete** : Resource module for Node Group Node Delete
* **cisco.ise.node_group_node_info** : Information module for Node Group Node
* **cisco.ise.node_info** : Information module for Node
* **cisco.ise.node_primary_to_standalone** : Resource module for Node Primary To Standalone
* **cisco.ise.node_promotion** : Resource module for Node Promotion
* **cisco.ise.node_replication_status_info** : Information module for Node Replication Status
* **cisco.ise.node_secondary_to_primary** : Resource module for Node Secondary To Primary
* **cisco.ise.node_services_interfaces_info** : Information module for Node Services Interfaces
* **cisco.ise.node_services_profiler_probe_config** : Resource module for Node Services Profiler Probe Config
* **cisco.ise.node_services_profiler_probe_config_info** : Information module for Node Services Profiler Probe Config
* **cisco.ise.node_services_sxp_interfaces** : Resource module for Node Services SXP Interfaces
* **cisco.ise.node_services_sxp_interfaces_info** : Information module for Node Services SXP Interfaces
* **cisco.ise.node_standalone_to_primary** : Resource module for Node Standalone To Primary
* **cisco.ise.node_sync** : Resource module for Node Sync
* **cisco.ise.pan_ha** : Resource module for Pan Ha
* **cisco.ise.pan_ha_info** : Information module for Pan Ha
* **cisco.ise.pan_ha_update** : Resource module for Pan Ha Update
* **cisco.ise.patch_info** : Information module for Patch
* **cisco.ise.patch_install** : Resource module for Patch Install
* **cisco.ise.patch_rollback** : Resource module for Patch Rollback
* **cisco.ise.personas_check_standalone** : Ensure the node is in standalone mode
* **cisco.ise.personas_export_certs** : Export certificate into primary node
* **cisco.ise.personas_promote_primary** : Promote a node as the primary node
* **cisco.ise.personas_register_node** : Register a node to the primary
* **cisco.ise.personas_update_roles_services** : Update the roles and services of a node
* **cisco.ise.portal_global_setting** : Resource module for Portal Global Setting
* **cisco.ise.portal_global_setting_info** : Information module for Portal Global Setting
* **cisco.ise.portal_info** : Information module for Portal
* **cisco.ise.portal_theme** : Resource module for Portal Theme
* **cisco.ise.portal_theme_info** : Information module for Portal Theme
* **cisco.ise.profiler_profile_info** : Information module for Profiler Profile
* **cisco.ise.proxy_connection_settings** : Resource module for Proxy Connection Settings
* **cisco.ise.proxy_connection_settings_info** : Information module for Proxy Connection Settings
* **cisco.ise.px_grid_node_approve** : Resource module for Px Grid Node Approve
* **cisco.ise.px_grid_node_delete** : Resource module for Px Grid Node Delete
* **cisco.ise.px_grid_node_info** : Information module for Px Grid Node
* **cisco.ise.px_grid_settings_auto_approve** : Resource module for Px Grid Settings Auto Approve
* **cisco.ise.pxgrid_access_secret** : Resource module for pxGrid Access Secret
* **cisco.ise.pxgrid_account_activate** : Resource module for pxGrid Account Activate
* **cisco.ise.pxgrid_account_create** : Resource module for pxGrid Account Create
* **cisco.ise.pxgrid_authorization** : Resource module for pxGrid Authorization
* **cisco.ise.pxgrid_bindings_info** : Information module for pxGrid Bindings Info
* **cisco.ise.pxgrid_egress_matrices_info** : Information module for pxGrid Egress Matrices Info
* **cisco.ise.pxgrid_egress_policies_info** : Information module for pxGrid Egress Policies Info
* **cisco.ise.pxgrid_endpoint_by_mac_info** : Information module for pxGrid Endpoint By Mac Info
* **cisco.ise.pxgrid_endpoints_by_os_type_info** : Information module for pxGrid Endpoints By Os Type Info
* **cisco.ise.pxgrid_endpoints_by_type_info** : Information module for pxGrid Endpoints By Type Info
* **cisco.ise.pxgrid_endpoints_info** : Information module for pxGrid Endpoints Info
* **cisco.ise.pxgrid_failures_info** : Information module for pxGrid Failures
* **cisco.ise.pxgrid_healths_info** : Information module for pxGrid Healths Info
* **cisco.ise.pxgrid_node_approve** : Resource module for pxGrid Node Approve
* **cisco.ise.pxgrid_node_delete** : Resource module for pxGrid Node Delete
* **cisco.ise.pxgrid_node_info** : Information module for pxGrid Node
* **cisco.ise.pxgrid_performances_info** : Information module for pxGrid Performances Info
* **cisco.ise.pxgrid_profiles_info** : Information module for pxGrid Profiles Info
* **cisco.ise.pxgrid_security_group_acls_info** : Information module for pxGrid Security Group ACLs Info
* **cisco.ise.pxgrid_security_groups_info** : Information module for pxGrid Security Groups Info
* **cisco.ise.pxgrid_service_lookup** : Resource module for pxGrid Service Lookup
* **cisco.ise.pxgrid_service_register** : Resource module for pxGrid Service Register
* **cisco.ise.pxgrid_service_reregister** : Resource module for pxGrid Service Reregister
* **cisco.ise.pxgrid_service_unregister** : Resource module for pxGrid Service Unregister
* **cisco.ise.pxgrid_session_by_ip_info** : Information module for pxGrid Session By Ip Info
* **cisco.ise.pxgrid_session_by_mac_info** : Information module for pxGrid Session By Mac Info
* **cisco.ise.pxgrid_session_for_recovery_info** : Information module for pxGrid Session For Recovery Info
* **cisco.ise.pxgrid_sessions_info** : Information module for pxGrid Sessions Info
* **cisco.ise.pxgrid_settings_auto_approve** : Resource module for pxGrid Settings Auto Approve
* **cisco.ise.pxgrid_user_group_by_username_info** : Information module for pxGrid User Group By Username Info
* **cisco.ise.pxgrid_user_groups_info** : Information module for pxGrid User Groups Info
* **cisco.ise.radius_server_sequence** : Resource module for RADIUS Server Sequence
* **cisco.ise.radius_server_sequence_info** : Information module for RADIUS Server Sequence
* **cisco.ise.renew_certificate** : Resource module for Renew Certificate
* **cisco.ise.repository** : Resource module for Repository
* **cisco.ise.repository_files_info** : Information module for Repository Files
* **cisco.ise.repository_info** : Information module for Repository
* **cisco.ise.resource_version_info** : Information module for Resource Version
* **cisco.ise.rest_id_store** : Resource module for REST Id Store
* **cisco.ise.rest_id_store_info** : Information module for REST Id Store
* **cisco.ise.self_registered_portal** : Resource module for Self Registered Portal
* **cisco.ise.self_registered_portal_info** : Information module for Self Registered Portal
* **cisco.ise.selfsigned_certificate_generate** : Resource module for Selfsigned Certificate Generate
* **cisco.ise.session_service_node_info** : Information module for Session Service Node
* **cisco.ise.sg_acl** : Resource module for SGACL
* **cisco.ise.sg_acl_bulk_monitor_status_info** : Information module for SGACL Bulk Monitor Status
* **cisco.ise.sg_acl_bulk_request** : Resource module for SGACL Bulk Request
* **cisco.ise.sg_acl_info** : Information module for SGACL
* **cisco.ise.sg_mapping** : Resource module for SG Mapping
* **cisco.ise.sg_mapping_bulk_monitor_status_info** : Information module for SG Mapping Bulk Monitor Status
* **cisco.ise.sg_mapping_bulk_request** : Resource module for SG Mapping Bulk Request
* **cisco.ise.sg_mapping_deploy** : Resource module for SG Mapping Deploy
* **cisco.ise.sg_mapping_deploy_all** : Resource module for SG Mapping Deploy All
* **cisco.ise.sg_mapping_deploy_status_info** : Information module for SG Mapping Deploy Status
* **cisco.ise.sg_mapping_group** : Resource module for SG Mapping Group
* **cisco.ise.sg_mapping_group_bulk_monitor_status_info** : Information module for SG Mapping Group Bulk Monitor Status
* **cisco.ise.sg_mapping_group_bulk_request** : Resource module for SG Mapping Group Bulk Request
* **cisco.ise.sg_mapping_group_deploy** : Resource module for SG Mapping Group Deploy
* **cisco.ise.sg_mapping_group_deploy_all** : Resource module for SG Mapping Group Deploy All
* **cisco.ise.sg_mapping_group_deploy_status_info** : Information module for SG Mapping Group Deploy Status
* **cisco.ise.sg_mapping_group_info** : Information module for SG Mapping Group
* **cisco.ise.sg_mapping_info** : Information module for SG Mapping
* **cisco.ise.sg_to_vn_to_vlan** : Resource module for SG To VN To VLAN
* **cisco.ise.sg_to_vn_to_vlan_bulk_monitor_status_info** : Information module for SG To VN To VLAN Bulk Monitor Status
* **cisco.ise.sg_to_vn_to_vlan_bulk_request** : Resource module for SG To VN To VLAN Bulk Request
* **cisco.ise.sg_to_vn_to_vlan_info** : Information module for SG To VN To VLAN
* **cisco.ise.sgt** : Resource module for SGt
* **cisco.ise.sgt_bulk_monitor_status_info** : Information module for SGt Bulk Monitor Status
* **cisco.ise.sgt_bulk_request** : Resource module for SGt Bulk Request
* **cisco.ise.sgt_info** : Information module for SGt
* **cisco.ise.sms_provider_info** : Information module for SMS Provider
* **cisco.ise.sponsor_group** : Resource module for Sponsor Group
* **cisco.ise.sponsor_group_info** : Information module for Sponsor Group
* **cisco.ise.sponsor_group_member_info** : Information module for Sponsor Group Member
* **cisco.ise.sponsor_portal** : Resource module for Sponsor Portal
* **cisco.ise.sponsor_portal_info** : Information module for Sponsor Portal
* **cisco.ise.sponsored_guest_portal** : Resource module for Sponsored Guest Portal
* **cisco.ise.sponsored_guest_portal_info** : Information module for Sponsored Guest Portal
* **cisco.ise.support_bundle** : Resource module for Support Bundle
* **cisco.ise.support_bundle_download** : Resource module for Support Bundle Download
* **cisco.ise.support_bundle_status_info** : Information module for Support Bundle Status
* **cisco.ise.sxp_connections** : Resource module for SXP Connections
* **cisco.ise.sxp_connections_bulk_monitor_status_info** : Information module for SXP Connections Bulk Monitor Status
* **cisco.ise.sxp_connections_bulk_request** : Resource module for SXP Connections Bulk Request
* **cisco.ise.sxp_connections_info** : Information module for SXP Connections
* **cisco.ise.sxp_local_bindings** : Resource module for SXP Local Bindings
* **cisco.ise.sxp_local_bindings_bulk_monitor_status_info** : Information module for SXP Local Bindings Bulk Monitor Status
* **cisco.ise.sxp_local_bindings_bulk_request** : Resource module for SXP Local Bindings Bulk Request
* **cisco.ise.sxp_local_bindings_info** : Information module for SXP Local Bindings
* **cisco.ise.sxp_vpns** : Resource module for SXP VPNs
* **cisco.ise.sxp_vpns_bulk_monitor_status_info** : Information module for SXP VPNs Bulk Monitor Status
* **cisco.ise.sxp_vpns_bulk_request** : Resource module for SXP VPNs Bulk Request
* **cisco.ise.sxp_vpns_info** : Information module for SXP VPNs
* **cisco.ise.system_certificate** : Resource module for System Certificate
* **cisco.ise.system_certificate_create** : Resource module for System Certificate Create
* **cisco.ise.system_certificate_export_info** : Information module for System Certificate Export Info
* **cisco.ise.system_certificate_import** : Resource module for System Certificate Import
* **cisco.ise.system_certificate_info** : Information module for System Certificate
* **cisco.ise.system_config_version_info** : Information module for System Config Version
* **cisco.ise.tacacs_command_sets** : Resource module for TACACS Command Sets
* **cisco.ise.tacacs_command_sets_info** : Information module for TACACS Command Sets
* **cisco.ise.tacacs_external_servers** : Resource module for TACACS External Servers
* **cisco.ise.tacacs_external_servers_info** : Information module for TACACS External Servers
* **cisco.ise.tacacs_profile** : Resource module for TACACS Profile
* **cisco.ise.tacacs_profile_info** : Information module for TACACS Profile
* **cisco.ise.tacacs_server_sequence** : Resource module for TACACS Server Sequence
* **cisco.ise.tacacs_server_sequence_info** : Information module for TACACS Server Sequence
* **cisco.ise.tasks_info** : Information module for Tasks
* **cisco.ise.telemetry_info** : Information module for Telemetry Info
* **cisco.ise.threat_vulnerabilities_clear** : Resource module for Threat Vulnerabilities Clear
* **cisco.ise.transport_gateway_settings** : Resource module for Transport Gateway Settings
* **cisco.ise.transport_gateway_settings_info** : Information module for Transport Gateway Settings
* **cisco.ise.trusted_certificate** : Resource module for Trusted Certificate
* **cisco.ise.trusted_certificate_export_info** : Information module for Trusted Certificate Export
* **cisco.ise.trusted_certificate_import** : Resource module for Trusted Certificate Import
* **cisco.ise.trusted_certificate_info** : Information module for Trusted Certificate
* **cisco.ise.trustsec_nbar_app** : Resource module for Trustsec NBAR App
* **cisco.ise.trustsec_nbar_app_info** : Information module for Trustsec NBAR App
* **cisco.ise.trustsec_sg_vn_mapping** : Resource module for Trustsec SG VN Mapping
* **cisco.ise.trustsec_sg_vn_mapping_bulk_create** : Resource module for Trustsec SG VN Mapping Bulk Create
* **cisco.ise.trustsec_sg_vn_mapping_bulk_delete** : Resource module for Trustsec SG VN Mapping Bulk Delete
* **cisco.ise.trustsec_sg_vn_mapping_bulk_update** : Resource module for Trustsec SG VN Mapping Bulk Update
* **cisco.ise.trustsec_sg_vn_mapping_info** : Information module for Trustsec SG VN Mapping
* **cisco.ise.trustsec_vn** : Resource module for Trustsec VN
* **cisco.ise.trustsec_vn_bulk_create** : Resource module for Trustsec VN Bulk Create
* **cisco.ise.trustsec_vn_bulk_delete** : Resource module for Trustsec VN Bulk Delete
* **cisco.ise.trustsec_vn_bulk_update** : Resource module for Trustsec VN Bulk Update
* **cisco.ise.trustsec_vn_info** : Information module for Trustsec VN
* **cisco.ise.trustsec_vn_vlan_mapping** : Resource module for Trustsec VN VLAN Mapping
* **cisco.ise.trustsec_vn_vlan_mapping_bulk_create** : Resource module for Trustsec VN VLAN Mapping Bulk Create
* **cisco.ise.trustsec_vn_vlan_mapping_bulk_delete** : Resource module for Trustsec VN VLAN Mapping Bulk Delete
* **cisco.ise.trustsec_vn_vlan_mapping_bulk_update** : Resource module for Trustsec VN VLAN Mapping Bulk Update
* **cisco.ise.trustsec_vn_vlan_mapping_info** : Information module for Trustsec VN VLAN Mapping

## `cisco.meraki` collection

* **cisco.meraki.meraki_action_batch** : Manage Action Batch jobs within the Meraki Dashboard.
* **cisco.meraki.meraki_admin** : Manage administrators in the Meraki cloud
* **cisco.meraki.meraki_alert** : Manage alerts in the Meraki cloud
* **cisco.meraki.meraki_config_template** : Manage configuration templates in the Meraki cloud
* **cisco.meraki.meraki_device** : Manage devices in the Meraki cloud
* **cisco.meraki.meraki_firewalled_services** : Edit firewall policies for administrative network services
* **cisco.meraki.meraki_management_interface** : Configure Meraki management interfaces
* **cisco.meraki.meraki_mr_l3_firewall** : Manage MR access point layer 3 firewalls in the Meraki cloud
* **cisco.meraki.meraki_mr_l7_firewall** : Manage MR access point layer 7 firewalls in the Meraki cloud
* **cisco.meraki.meraki_mr_radio** : Manage device radio settings for Meraki wireless networks
* **cisco.meraki.meraki_mr_rf_profile** : Manage RF profiles for Meraki wireless networks
* **cisco.meraki.meraki_mr_settings** : Manage general settings for Meraki wireless networks
* **cisco.meraki.meraki_mr_ssid** : Manage wireless SSIDs in the Meraki cloud
* **cisco.meraki.meraki_ms_access_list** : Manage access lists for Meraki switches in the Meraki cloud
* **cisco.meraki.meraki_ms_access_policies** : Manage Switch Access Policies in the Meraki cloud
* **cisco.meraki.meraki_ms_stack_l3_interface** : Manage routed interfaces on MS switches
* **cisco.meraki.meraki_ms_link_aggregation** : Manage link aggregations on MS switches
* **cisco.meraki.meraki_ms_ospf** : Manage OSPF configuration on MS switches
* **cisco.meraki.meraki_ms_stack** : Modify switch stacking configuration in Meraki.
* **cisco.meraki.meraki_ms_storm_control** : Manage storm control configuration on a switch in the Meraki cloud
* **cisco.meraki.meraki_ms_switchport** : Manage switchports on a switch in the Meraki cloud
* **cisco.meraki.meraki_mx_content_filtering** : Edit Meraki MX content filtering policies
* **cisco.meraki.meraki_mx_intrusion_prevention** : Manage intrustion prevention in the Meraki cloud
* **cisco.meraki.meraki_mx_l2_interface** : Configure MX layer 2 interfaces
* **cisco.meraki.meraki_mx_l3_firewall** : Manage MX appliance layer 3 firewalls in the Meraki cloud
* **cisco.meraki.meraki_mx_l7_firewall** : Manage MX appliance layer 7 firewalls in the Meraki cloud
* **cisco.meraki.meraki_mx_malware** : Manage Malware Protection in the Meraki cloud
* **cisco.meraki.meraki_mx_nat** : Manage NAT rules in Meraki cloud
* **cisco.meraki.meraki_mx_network_vlan_settings** : Manage VLAN settings for Meraki Networks
* **cisco.meraki.meraki_mx_site_to_site_firewall** : Manage MX appliance firewall rules for site-to-site VPNs
* **cisco.meraki.meraki_mx_site_to_site_vpn** : Manage AutoVPN connections in Meraki
* **cisco.meraki.meraki_mx_static_route** : Manage static routes in the Meraki cloud
* **cisco.meraki.meraki_mx_third_party_vpn_peers** : Manage third party (IPSec) VPN peers for MX devices
* **cisco.meraki.meraki_mx_uplink_bandwidth** : Manage uplinks on Meraki MX appliances
* **cisco.meraki.meraki_mx_vlan** : Manage VLANs in the Meraki cloud
* **cisco.meraki.meraki_network** : Manage networks in the Meraki cloud
* **cisco.meraki.meraki_network_settings** : Manage the settings of networks in the Meraki cloud
* **cisco.meraki.meraki_snmp** : Manage organizations in the Meraki cloud
* **cisco.meraki.meraki_syslog** : Manage syslog server settings in the Meraki cloud.
* **cisco.meraki.meraki_webhook** : Manage webhooks configured in the Meraki cloud
* **cisco.meraki.meraki_webhook_payload_template** : Manage webhook payload templates for a network in the Meraki cloud

## `cisco.mso` collection

* **cisco.mso.mso_backup** : Manages backups
* **cisco.mso.mso_backup_schedule** : Manages backup schedules
* **cisco.mso.mso_dhcp_option_policy** : Manage DHCP Option policies.
* **cisco.mso.mso_dhcp_option_policy_option** : Manage DHCP options in a DHCP Option policy.
* **cisco.mso.mso_dhcp_relay_policy** : Manage DHCP Relay policies.
* **cisco.mso.mso_dhcp_relay_policy_provider** : Manage DHCP providers in a DHCP Relay policy.
* **cisco.mso.mso_label** : Manage labels
* **cisco.mso.mso_remote_location** : Manages remote locations
* **cisco.mso.mso_rest** : Direct access to the Cisco MSO REST API
* **cisco.mso.mso_role** : Manage roles
* **cisco.mso.mso_schema** : Manage schemas
* **cisco.mso.mso_schema_clone** : Clone schemas
* **cisco.mso.mso_schema_site** : Manage sites in schemas
* **cisco.mso.mso_schema_site_anp** : Manage site-local Application Network Profiles (ANPs) in schema template
* **cisco.mso.mso_schema_site_anp_epg** : Manage site-local Endpoint Groups (EPGs) in schema template
* **cisco.mso.mso_schema_site_anp_epg_domain** : Manage site-local EPG domains in schema template
* **cisco.mso.mso_schema_site_anp_epg_selector** : Manage site-local EPG selector in schema templates
* **cisco.mso.mso_schema_site_anp_epg_staticleaf** : Manage site-local EPG static leafs in schema template
* **cisco.mso.mso_schema_site_anp_epg_staticport** : Manage site-local EPG static ports in schema template
* **cisco.mso.mso_schema_site_anp_epg_subnet** : Manage site-local EPG subnets in schema template
* **cisco.mso.mso_schema_site_bd** : Manage site-local Bridge Domains (BDs) in schema template
* **cisco.mso.mso_schema_site_bd_l3out** : Manage site-local BD l3out&#39;s in schema template
* **cisco.mso.mso_schema_site_bd_subnet** : Manage site-local BD subnets in schema template
* **cisco.mso.mso_schema_site_external_epg** : Manage External EPG in schema of sites
* **cisco.mso.mso_schema_site_external_epg_selector** : Manage External EPG selector in schema of cloud sites
* **cisco.mso.mso_schema_site_l3out** : Manage site-local layer3 Out (L3Outs) in schema template
* **cisco.mso.mso_schema_site_service_graph** : Manage Service Graph in schema sites
* **cisco.mso.mso_schema_site_vrf** : Manage site-local VRFs in schema template
* **cisco.mso.mso_schema_site_vrf_region_cidr_subnet** : Manage site-local VRF regions in schema template
* **cisco.mso.mso_schema_site_vrf_region_cidr** : Manage site-local VRF region CIDRs in schema template
* **cisco.mso.mso_schema_site_vrf_region_hub_network** : Manage site-local VRF region hub network in schema template
* **cisco.mso.mso_schema_template** : Manage templates in schemas
* **cisco.mso.mso_schema_template_anp** : Manage Application Network Profiles (ANPs) in schema templates
* **cisco.mso.mso_schema_template_anp_epg** : Manage Endpoint Groups (EPGs) in schema templates
* **cisco.mso.mso_schema_template_anp_epg_contract** : Manage EPG contracts in schema templates
* **cisco.mso.mso_schema_template_anp_epg_selector** : Manage EPG selector in schema templates
* **cisco.mso.mso_schema_template_anp_epg_subnet** : Manage EPG subnets in schema templates
* **cisco.mso.mso_schema_template_bd** : Manage Bridge Domains (BDs) in schema templates
* **cisco.mso.mso_schema_template_bd_dhcp_policy** : Manage BD DHCP Policy in schema templates
* **cisco.mso.mso_schema_template_bd_subnet** : Manage BD subnets in schema templates
* **cisco.mso.mso_schema_template_clone** : Clone templates
* **cisco.mso.mso_schema_template_contract_filter** : Manage contract filters in schema templates
* **cisco.mso.mso_schema_template_contract_service_graph** : Manage the service graph association with a contract in schema template
* **cisco.mso.mso_schema_template_deploy** : Deploy schema templates to sites
* **cisco.mso.mso_schema_template_deploy_status** : Check query of objects before deployment to site
* **cisco.mso.mso_schema_template_external_epg** : Manage external EPGs in schema templates
* **cisco.mso.mso_schema_template_external_epg_contract** : Manage Extrnal EPG contracts in schema templates
* **cisco.mso.mso_schema_template_external_epg_selector** : Manage External EPG selector in schema templates
* **cisco.mso.mso_schema_template_external_epg_subnet** : Manage External EPG subnets in schema templates
* **cisco.mso.mso_schema_template_filter_entry** : Manage filter entries in schema templates
* **cisco.mso.mso_schema_template_l3out** : Manage l3outs in schema templates
* **cisco.mso.mso_schema_template_migrate** : Migrate Bridge Domains (BDs) and EPGs between templates
* **cisco.mso.mso_schema_template_service_graph** : Manage Service Graph in schema templates
* **cisco.mso.mso_schema_template_vrf** : Manage VRFs in schema templates
* **cisco.mso.mso_schema_template_vrf_contract** : Manage vrf contracts in schema templates
* **cisco.mso.mso_schema_validate** : Validate the schema before deploying it to site
* **cisco.mso.mso_service_node_type** : Manage Service Node Types
* **cisco.mso.mso_site** : Manage sites
* **cisco.mso.mso_tenant** : Manage tenants
* **cisco.mso.mso_tenant_site** : Manage tenants with cloud sites.
* **cisco.mso.mso_user** : Manage users
* **cisco.mso.mso_version** : Get version of MSO
* **cisco.mso.ndo_schema_template_deploy** : Deploy schema templates to sites for NDO v3.7 and higher

## `cisco.nso` collection

* **cisco.nso.nso_action** : Executes Cisco NSO actions and verifies output.
* **cisco.nso.nso_config** : Manage Cisco NSO configuration and service synchronization.
* **cisco.nso.nso_query** : Query data from Cisco NSO.
* **cisco.nso.nso_show** : Displays data from Cisco NSO.
* **cisco.nso.nso_verify** : Verifies Cisco NSO configuration.

## `cisco.nxos` collection

* **cisco.nxos.nxos_aaa_server** : Manages AAA server global configuration.
* **cisco.nxos.nxos_aaa_server_host** : Manages AAA server host-specific configuration.
* **cisco.nxos.nxos_acl_interfaces** : ACL interfaces resource module
* **cisco.nxos.nxos_acls** : ACLs resource module
* **cisco.nxos.nxos_banner** : Manage multiline banners on Cisco NXOS devices
* **cisco.nxos.nxos_bfd_global** : Bidirectional Forwarding Detection (BFD) global-level configuration
* **cisco.nxos.nxos_bfd_interfaces** : BFD interfaces resource module
* **cisco.nxos.nxos_bgp_address_family** : BGP Address Family resource module.
* **cisco.nxos.nxos_bgp_global** : BGP Global resource module.
* **cisco.nxos.nxos_bgp_neighbor_address_family** : BGP Neighbor Address Family resource module.
* **cisco.nxos.nxos_command** : Run arbitrary command on Cisco NXOS devices
* **cisco.nxos.nxos_config** : Manage Cisco NXOS configuration sections
* **cisco.nxos.nxos_devicealias** : Configuration of device alias for Cisco NXOS MDS Switches.
* **cisco.nxos.nxos_evpn_global** : Handles the EVPN control plane for VXLAN.
* **cisco.nxos.nxos_evpn_vni** : Manages Cisco EVPN VXLAN Network Identifier (VNI).
* **cisco.nxos.nxos_facts** : Gets facts about NX-OS switches
* **cisco.nxos.nxos_feature** : Manage features in NX-OS switches.
* **cisco.nxos.nxos_file_copy** : Copy a file to a remote NXOS device.
* **cisco.nxos.nxos_gir** : Trigger a graceful removal or insertion (GIR) of the switch.
* **cisco.nxos.nxos_gir_profile_management** : Create a maintenance-mode or normal-mode profile for GIR.
* **cisco.nxos.nxos_hostname** : Hostname resource module.
* **cisco.nxos.nxos_hsrp** : Manages HSRP configuration on NX-OS switches.
* **cisco.nxos.nxos_hsrp_interfaces** : HSRP interfaces resource module
* **cisco.nxos.nxos_igmp** : Manages IGMP global configuration.
* **cisco.nxos.nxos_igmp_interface** : Manages IGMP interface configuration.
* **cisco.nxos.nxos_igmp_snooping** : Manages IGMP snooping global configuration.
* **cisco.nxos.nxos_install_os** : Set boot options like boot, kickstart image and issu.
* **cisco.nxos.nxos_interfaces** : Interfaces resource module
* **cisco.nxos.nxos_l2_interfaces** : L2 interfaces resource module
* **cisco.nxos.nxos_l3_interfaces** : L3 interfaces resource module
* **cisco.nxos.nxos_lacp** : LACP resource module
* **cisco.nxos.nxos_lacp_interfaces** : LACP interfaces resource module
* **cisco.nxos.nxos_lag_interfaces** : LAG interfaces resource module
* **cisco.nxos.nxos_lldp_global** : LLDP resource module
* **cisco.nxos.nxos_lldp_interfaces** : LLDP interfaces resource module
* **cisco.nxos.nxos_logging_global** : Logging resource module.
* **cisco.nxos.nxos_ntp_global** : NTP Global resource module.
* **cisco.nxos.nxos_nxapi** : Manage NXAPI configuration on an NXOS device.
* **cisco.nxos.nxos_ospf_interfaces** : OSPF Interfaces Resource Module.
* **cisco.nxos.nxos_ospfv2** : OSPFv2 resource module
* **cisco.nxos.nxos_ospfv3** : OSPFv3 resource module
* **cisco.nxos.nxos_overlay_global** : Configures anycast gateway MAC of the switch.
* **cisco.nxos.nxos_pim** : Manages configuration of a PIM instance.
* **cisco.nxos.nxos_pim_interface** : Manages PIM interface configuration.
* **cisco.nxos.nxos_pim_rp_address** : Manages configuration of an PIM static RP address instance.
* **cisco.nxos.nxos_ping** : Tests reachability using ping from Nexus switch.
* **cisco.nxos.nxos_prefix_lists** : Prefix-Lists resource module.
* **cisco.nxos.nxos_reboot** : Reboot a network device.
* **cisco.nxos.nxos_rollback** : Set a checkpoint or rollback to a checkpoint.
* **cisco.nxos.nxos_route_maps** : Route Maps resource module.
* **cisco.nxos.nxos_rpm** : Install patch or feature rpms on Cisco NX-OS devices.
* **cisco.nxos.nxos_snapshot** : Manage snapshots of the running states of selected features.
* **cisco.nxos.nxos_snmp_server** : SNMP Server resource module.
* **cisco.nxos.nxos_static_routes** : Static routes resource module
* **cisco.nxos.nxos_system** : Manage the system attributes on Cisco NXOS devices
* **cisco.nxos.nxos_telemetry** : TELEMETRY resource module
* **cisco.nxos.nxos_udld** : Manages UDLD global configuration params.
* **cisco.nxos.nxos_udld_interface** : Manages UDLD interface configuration params.
* **cisco.nxos.nxos_user** : Manage the collection of local users on Nexus devices
* **cisco.nxos.nxos_vlans** : VLANs resource module
* **cisco.nxos.nxos_vpc** : Manages global VPC configuration
* **cisco.nxos.nxos_vpc_interface** : Manages interface VPC configuration
* **cisco.nxos.nxos_vrf** : Manages global VRF configuration.
* **cisco.nxos.nxos_vrf_af** : Manages VRF AF.
* **cisco.nxos.nxos_vrf_interface** : Manages interface specific VRF configuration.
* **cisco.nxos.nxos_vrrp** : Manages VRRP configuration on NX-OS switches.
* **cisco.nxos.nxos_vsan** : Configuration of vsan for Cisco NXOS MDS Switches.
* **cisco.nxos.nxos_vtp_domain** : Manages VTP domain configuration.
* **cisco.nxos.nxos_vtp_password** : Manages VTP password configuration.
* **cisco.nxos.nxos_vtp_version** : Manages VTP version configuration.
* **cisco.nxos.nxos_vxlan_vtep** : Manages VXLAN Network Virtualization Endpoint (NVE).
* **cisco.nxos.nxos_vxlan_vtep_vni** : Creates a Virtual Network Identifier member (VNI)
* **cisco.nxos.nxos_zone_zoneset** : Configuration of zone/zoneset for Cisco NXOS MDS Switches.

## `cisco.ucs` collection

* **cisco.ucs.ucs_disk_group_policy** : Configures disk group policies on Cisco UCS Manager
* **cisco.ucs.ucs_dns_server** : Configure DNS servers on Cisco UCS Manager
* **cisco.ucs.ucs_graphics_card_policy** : Manages UCS Graphics Card Policies on UCS Manager
* **cisco.ucs.ucs_ip_pool** : Configures IP address pools on Cisco UCS Manager
* **cisco.ucs.ucs_lan_connectivity** : Configures LAN Connectivity Policies on Cisco UCS Manager
* **cisco.ucs.ucs_mac_pool** : Configures MAC address pools on Cisco UCS Manager
* **cisco.ucs.ucs_managed_objects** : Configures Managed Objects on Cisco UCS Manager
* **cisco.ucs.ucs_ntp_server** : Configures NTP server on Cisco UCS Manager
* **cisco.ucs.ucs_org** : Manages UCS Organizations for UCS Manager
* **cisco.ucs.ucs_query** : Queries UCS Manager objects by class or distinguished name
* **cisco.ucs.ucs_san_connectivity** : Configures SAN Connectivity Policies on Cisco UCS Manager
* **cisco.ucs.ucs_scrub_policy** : Manages UCS Scrub Policies on UCS Manager
* **cisco.ucs.ucs_serial_over_lan_policy** : Manages UCS Serial Over Lan Policies on UCS Manager
* **cisco.ucs.ucs_server_maintenance** : Creates Server Maintenance Policy on Cisco UCS Manager
* **cisco.ucs.ucs_service_profile_association** : Configures Service Profile Association on Cisco UCS Manager
* **cisco.ucs.ucs_service_profile_from_template** : Configures Service Profiles from templates on Cisco UCS Manager
* **cisco.ucs.ucs_service_profile_template** : Configures Service Profile Templates on Cisco UCS Manager
* **cisco.ucs.ucs_sp_vnic_order** : Configures vNIC order for service profiles and templates on Cisco UCS Manager
* **cisco.ucs.ucs_storage_profile** : Configures storage profiles on Cisco UCS Manager
* **cisco.ucs.ucs_system_qos** : Configures system QoS settings
* **cisco.ucs.ucs_timezone** : Configures timezone on Cisco UCS Manager
* **cisco.ucs.ucs_uuid_pool** : Configures server UUID pools on Cisco UCS Manager
* **cisco.ucs.ucs_vhba_template** : Configures vHBA templates on Cisco UCS Manager
* **cisco.ucs.ucs_vlan_find** : Find VLANs on Cisco UCS Manager
* **cisco.ucs.ucs_vlan_to_group** : Add VLANs to a VLAN Group. Requires VLAN and VLAN Group to already be created on UCS prior to running module.
* **cisco.ucs.ucs_vlans** : Configures VLANs on Cisco UCS Manager
* **cisco.ucs.ucs_vnic_template** : Configures vNIC templates on Cisco UCS Manager
* **cisco.ucs.ucs_vsans** : Configures VSANs on Cisco UCS Manager
* **cisco.ucs.ucs_wwn_pool** : Configures WWNN or WWPN pools on Cisco UCS Manager

## `cloud.common` collection

* **cloud.common.turbo_demo** : A demo module for ansible_module.turbo
* **cloud.common.turbo_fail** : A short module which honor additional args when calling fail_json
* **cloud.common.turbo_import** : A demo module to test import logic for turbo mode

## `cloudscale_ch.cloud` collection

* **cloudscale_ch.cloud.custom_image** : Manage custom images on the cloudscale.ch IaaS service
* **cloudscale_ch.cloud.floating_ip** : Manages floating IPs on the cloudscale.ch IaaS service
* **cloudscale_ch.cloud.network** : Manages networks on the cloudscale.ch IaaS service
* **cloudscale_ch.cloud.objects_user** : Manages objects users on the cloudscale.ch IaaS service
* **cloudscale_ch.cloud.server** : Manages servers on the cloudscale.ch IaaS service
* **cloudscale_ch.cloud.server_group** : Manages server groups on the cloudscale.ch IaaS service
* **cloudscale_ch.cloud.subnet** : Manages subnets on the cloudscale.ch IaaS service
* **cloudscale_ch.cloud.volume** : Manages volumes on the cloudscale.ch IaaS service.

## `community.aws` collection

* **community.aws.accessanalyzer_validate_policy_info** : Performs validation of IAM policies
* **community.aws.acm_certificate** : Upload and delete certificates in the AWS Certificate Manager service
* **community.aws.acm_certificate_info** : Retrieve certificate information from AWS Certificate Manager service
* **community.aws.api_gateway** : Manage AWS API Gateway APIs
* **community.aws.api_gateway_domain** : Manage AWS API Gateway custom domains
* **community.aws.application_autoscaling_policy** : Manage Application Auto Scaling Scaling Policies
* **community.aws.autoscaling_complete_lifecycle_action** : Completes the lifecycle action of an instance
* **community.aws.autoscaling_instance_refresh** : Start or cancel an EC2 Auto Scaling Group (ASG) instance refresh in AWS
* **community.aws.autoscaling_instance_refresh_info** : Gather information about EC2 Auto Scaling Group (ASG) Instance Refreshes in AWS
* **community.aws.autoscaling_launch_config** : Create or delete AWS Autoscaling Launch Configurations
* **community.aws.autoscaling_launch_config_find** : Find AWS Autoscaling Launch Configurations
* **community.aws.autoscaling_launch_config_info** : Gather information about AWS Autoscaling Launch Configurations
* **community.aws.autoscaling_lifecycle_hook** : Create, delete or update AWS ASG Lifecycle Hooks
* **community.aws.autoscaling_policy** : Create or delete AWS scaling policies for Autoscaling groups
* **community.aws.autoscaling_scheduled_action** : Create, modify and delete ASG scheduled scaling actions
* **community.aws.aws_region_info** : Gather information about AWS regions
* **community.aws.batch_compute_environment** : Manage AWS Batch Compute Environments
* **community.aws.batch_job_definition** : Manage AWS Batch Job Definitions
* **community.aws.batch_job_queue** : Manage AWS Batch Job Queues
* **community.aws.cloudformation_exports_info** : Read a value from CloudFormation Exports
* **community.aws.cloudformation_stack_set** : Manage groups of CloudFormation stacks
* **community.aws.cloudfront_distribution** : Create, update and delete AWS CloudFront distributions
* **community.aws.cloudfront_distribution_info** : Obtain facts about an AWS CloudFront distribution
* **community.aws.cloudfront_invalidation** : create invalidations for AWS CloudFront distributions
* **community.aws.cloudfront_origin_access_identity** : Create, update and delete origin access identities for a CloudFront distribution
* **community.aws.cloudfront_response_headers_policy** : Create, update and delete response headers policies to be used in a Cloudfront distribution
* **community.aws.codebuild_project** : Create or delete an AWS CodeBuild project
* **community.aws.codecommit_repository** : Manage repositories in AWS CodeCommit
* **community.aws.codepipeline** : Create or delete AWS CodePipelines
* **community.aws.config_aggregation_authorization** : Manage cross-account AWS Config authorizations
* **community.aws.config_aggregator** : Manage AWS Config aggregations across multiple accounts
* **community.aws.config_delivery_channel** : Manage AWS Config delivery channels
* **community.aws.config_recorder** : Manage AWS Config Recorders
* **community.aws.config_rule** : Manage AWS Config rule resources
* **community.aws.data_pipeline** : Create and manage AWS Datapipelines
* **community.aws.directconnect_confirm_connection** : Confirms the creation of a hosted DirectConnect connection
* **community.aws.directconnect_connection** : Creates, deletes, modifies a DirectConnect connection
* **community.aws.directconnect_gateway** : Manage AWS Direct Connect gateway
* **community.aws.directconnect_link_aggregation_group** : Manage Direct Connect LAG bundles
* **community.aws.directconnect_virtual_interface** : Manage Direct Connect virtual interfaces
* **community.aws.dms_endpoint** : Creates or destroys a data migration services endpoint
* **community.aws.dms_replication_subnet_group** : creates or destroys a data migration services subnet group
* **community.aws.dynamodb_table** : Create, update or delete AWS Dynamo DB tables
* **community.aws.dynamodb_ttl** : Set TTL for a given DynamoDB table
* **community.aws.ec2_ami_copy** : copies AMI between AWS regions, return new image id
* **community.aws.ec2_customer_gateway** : Manage an AWS customer gateway
* **community.aws.ec2_customer_gateway_info** : Gather information about customer gateways in AWS
* **community.aws.ec2_launch_template** : Manage EC2 launch templates
* **community.aws.ec2_placement_group** : Create or delete an EC2 Placement Group
* **community.aws.ec2_placement_group_info** : List EC2 Placement Group(s) details
* **community.aws.ec2_snapshot_copy** : Copies an EC2 snapshot and returns the new Snapshot ID
* **community.aws.ec2_transit_gateway** : Create and delete AWS Transit Gateways
* **community.aws.ec2_transit_gateway_info** : Gather information about ec2 transit gateways in AWS
* **community.aws.ec2_transit_gateway_vpc_attachment** : Create and delete AWS Transit Gateway VPC attachments
* **community.aws.ec2_transit_gateway_vpc_attachment_info** : describes AWS Transit Gateway VPC attachments
* **community.aws.ec2_vpc_egress_igw** : Manage an AWS VPC Egress Only Internet gateway
* **community.aws.ec2_vpc_nacl** : create and delete Network ACLs
* **community.aws.ec2_vpc_nacl_info** : Gather information about Network ACLs in an AWS VPC
* **community.aws.ec2_vpc_peer** : create, delete, accept, and reject VPC peering connections between two VPCs.
* **community.aws.ec2_vpc_peering_info** : Retrieves AWS VPC Peering details using AWS methods.
* **community.aws.ec2_vpc_vgw** : Create and delete AWS VPN Virtual Gateways
* **community.aws.ec2_vpc_vgw_info** : Gather information about virtual gateways in AWS
* **community.aws.ec2_vpc_vpn** : Create, modify, and delete EC2 VPN connections
* **community.aws.ec2_vpc_vpn_info** : Gather information about VPN Connections in AWS.
* **community.aws.ec2_win_password** : Gets the default administrator password for EC2 Windows instances
* **community.aws.ecs_attribute** : manage ecs attributes
* **community.aws.ecs_cluster** : Create or terminate ECS clusters.
* **community.aws.ecs_ecr** : Manage Elastic Container Registry repositories
* **community.aws.ecs_service** : Create, terminate, start or stop a service in ECS
* **community.aws.ecs_service_info** : List or describe services in ECS
* **community.aws.ecs_tag** : create and remove tags on Amazon ECS resources
* **community.aws.ecs_task** : Run, start or stop a task in ECS
* **community.aws.ecs_taskdefinition** : register a task definition in ecs
* **community.aws.ecs_taskdefinition_info** : Describe a task definition in ECS
* **community.aws.efs** : create and maintain EFS file systems
* **community.aws.efs_info** : Get information about Amazon EFS file systems
* **community.aws.efs_tag** : create and remove tags on Amazon EFS resources
* **community.aws.eks_cluster** : Manage Elastic Kubernetes Service (EKS) Clusters
* **community.aws.eks_fargate_profile** : Manage EKS Fargate Profile
* **community.aws.elasticache** : Manage cache clusters in Amazon ElastiCache
* **community.aws.elasticache_info** : Retrieve information for AWS ElastiCache clusters
* **community.aws.elasticache_parameter_group** : Manage cache parameter groups in Amazon ElastiCache.
* **community.aws.elasticache_snapshot** : Manage cache snapshots in Amazon ElastiCache
* **community.aws.elasticache_subnet_group** : manage ElastiCache subnet groups
* **community.aws.elasticbeanstalk_app** : Create, update, and delete an Elastic Beanstalk application
* **community.aws.elb_classic_lb_info** : Gather information about EC2 Elastic Load Balancers in AWS
* **community.aws.elb_instance** : De-registers or registers instances from EC2 ELBs
* **community.aws.elb_network_lb** : Manage a Network Load Balancer
* **community.aws.elb_target** : Manage a target in a target group
* **community.aws.elb_target_group** : Manage a target group for an Application or Network load balancer
* **community.aws.elb_target_group_info** : Gather information about ELB target groups in AWS
* **community.aws.elb_target_info** : Gathers which target groups a target is associated with.
* **community.aws.glue_connection** : Manage an AWS Glue connection
* **community.aws.glue_crawler** : Manage an AWS Glue crawler
* **community.aws.glue_job** : Manage an AWS Glue job
* **community.aws.iam_access_key** : Manage AWS IAM User access keys
* **community.aws.iam_access_key_info** : fetch information about AWS IAM User access keys
* **community.aws.iam_group** : Manage AWS IAM groups
* **community.aws.iam_managed_policy** : Manage User Managed IAM policies
* **community.aws.iam_mfa_device_info** : List the MFA (Multi-Factor Authentication) devices registered for a user
* **community.aws.iam_password_policy** : Update an IAM Password Policy
* **community.aws.iam_role** : Manage AWS IAM roles
* **community.aws.iam_role_info** : Gather information on IAM roles
* **community.aws.iam_saml_federation** : Maintain IAM SAML federation configuration.
* **community.aws.iam_server_certificate** : Manage IAM server certificates for use on ELBs and CloudFront
* **community.aws.iam_server_certificate_info** : Retrieve the information of a server certificate
* **community.aws.inspector_target** : Create, Update and Delete Amazon Inspector Assessment Targets
* **community.aws.kinesis_stream** : Manage a Kinesis Stream.
* **community.aws.lightsail** : Manage instances in AWS Lightsail
* **community.aws.lightsail_static_ip** : Manage static IP addresses in AWS Lightsail
* **community.aws.msk_cluster** : Manage Amazon MSK clusters
* **community.aws.msk_config** : Manage Amazon MSK cluster configurations
* **community.aws.networkfirewall** : manage AWS Network Firewall firewalls
* **community.aws.networkfirewall_info** : describe AWS Network Firewall firewalls
* **community.aws.networkfirewall_policy** : manage AWS Network Firewall policies
* **community.aws.networkfirewall_policy_info** : describe AWS Network Firewall policies
* **community.aws.networkfirewall_rule_group** : create, delete and modify AWS Network Firewall rule groups
* **community.aws.networkfirewall_rule_group_info** : describe AWS Network Firewall rule groups
* **community.aws.opensearch** : Creates OpenSearch or ElasticSearch domain
* **community.aws.opensearch_info** : obtain information about one or more OpenSearch or ElasticSearch domain
* **community.aws.redshift** : create, delete, or modify an Amazon Redshift instance
* **community.aws.redshift_cross_region_snapshots** : Manage Redshift Cross Region Snapshots
* **community.aws.redshift_info** : Gather information about Redshift cluster(s)
* **community.aws.redshift_subnet_group** : manage Redshift cluster subnet groups
* **community.aws.s3_bucket_info** : Lists S3 buckets in AWS
* **community.aws.s3_bucket_notification** : Creates, updates or deletes S3 Bucket notifications targeting Lambda functions, SNS or SQS.
* **community.aws.s3_cors** : Manage CORS for S3 buckets in AWS
* **community.aws.s3_lifecycle** : Manage S3 bucket lifecycle rules in AWS
* **community.aws.s3_logging** : Manage logging facility of an s3 bucket in AWS
* **community.aws.s3_metrics_configuration** : Manage s3 bucket metrics configuration in AWS
* **community.aws.s3_sync** : Efficiently upload multiple files to S3
* **community.aws.s3_website** : Configure an s3 bucket as a website
* **community.aws.secretsmanager_secret** : Manage secrets stored in AWS Secrets Manager
* **community.aws.ses_identity** : Manages SES email and domain identity
* **community.aws.ses_identity_policy** : Manages SES sending authorization policies
* **community.aws.ses_rule_set** : Manages SES inbound receipt rule sets
* **community.aws.sns** : Send Amazon Simple Notification Service messages
* **community.aws.sns_topic** : Manages AWS SNS topics and subscriptions
* **community.aws.sns_topic_info** : sns_topic_info module
* **community.aws.sqs_queue** : Creates or deletes AWS SQS queues
* **community.aws.ssm_parameter** : Manage key-value pairs in AWS Systems Manager Parameter Store
* **community.aws.stepfunctions_state_machine** : Manage AWS Step Functions state machines
* **community.aws.stepfunctions_state_machine_execution** : Start or stop execution of an AWS Step Functions state machine
* **community.aws.storagegateway_info** : Fetch AWS Storage Gateway information
* **community.aws.sts_assume_role** : Assume a role using AWS Security Token Service and obtain temporary credentials
* **community.aws.sts_session_token** : Obtain a session token from the AWS Security Token Service
* **community.aws.waf_condition** : Create and delete WAF Conditions
* **community.aws.waf_info** : Retrieve information for WAF ACLs, Rules, Conditions and Filters
* **community.aws.waf_rule** : Create and delete WAF Rules
* **community.aws.wafv2_web_acl** : Create and delete WAF Web ACLs
* **community.aws.wafv2_ip_set** : wafv2_ip_set
* **community.aws.wafv2_ip_set_info** : Get information about wafv2 ip sets
* **community.aws.wafv2_web_acl_info** : wafv2_web_acl
* **community.aws.wafv2_resources_info** : wafv2_resources_info
* **community.aws.wafv2_rule_group_info** : wafv2_web_acl_info

## `community.ciscosmb` collection

* **community.ciscosmb.command** : Run commands on remote Cisco SMB devices
* **community.ciscosmb.facts** : Collect facts from remote devices running Cisco SMB

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

## `community.digitalocean` collection

* **community.digitalocean.digital_ocean_account_info** : Gather information about DigitalOcean User account
* **community.digitalocean.digital_ocean_balance_info** : Display DigitalOcean customer balance
* **community.digitalocean.digital_ocean_block_storage** : Create/destroy or attach/detach Block Storage volumes in DigitalOcean
* **community.digitalocean.digital_ocean_cdn_endpoints** : Create, update, and delete DigitalOcean CDN Endpoints
* **community.digitalocean.digital_ocean_cdn_endpoints_info** : Display DigitalOcean CDN Endpoints
* **community.digitalocean.digital_ocean_certificate** : Manage certificates in DigitalOcean
* **community.digitalocean.digital_ocean_certificate_info** : Gather information about DigitalOcean certificates
* **community.digitalocean.digital_ocean_database** : Create and delete a DigitalOcean database
* **community.digitalocean.digital_ocean_database_info** : Gather information about DigitalOcean databases
* **community.digitalocean.digital_ocean_domain** : Create/delete a DNS domain in DigitalOcean
* **community.digitalocean.digital_ocean_domain_info** : Gather information about DigitalOcean Domains
* **community.digitalocean.digital_ocean_domain_record** : Manage DigitalOcean domain records
* **community.digitalocean.digital_ocean_domain_record_info** : Gather information about DigitalOcean domain records
* **community.digitalocean.digital_ocean_droplet** : Create and delete a DigitalOcean droplet
* **community.digitalocean.digital_ocean_droplet_info** : Gather information about DigitalOcean Droplets
* **community.digitalocean.digital_ocean_firewall** : Manage cloud firewalls within DigitalOcean
* **community.digitalocean.digital_ocean_firewall_info** : Gather information about DigitalOcean firewalls
* **community.digitalocean.digital_ocean_floating_ip** : Manage DigitalOcean Floating IPs
* **community.digitalocean.digital_ocean_floating_ip_info** : DigitalOcean Floating IPs information
* **community.digitalocean.digital_ocean_image_info** : Gather information about DigitalOcean images
* **community.digitalocean.digital_ocean_kubernetes** : Create and delete a DigitalOcean Kubernetes cluster
* **community.digitalocean.digital_ocean_kubernetes_info** : Returns information about an existing DigitalOcean Kubernetes cluster
* **community.digitalocean.digital_ocean_load_balancer** : Manage DigitalOcean Load Balancers
* **community.digitalocean.digital_ocean_load_balancer_info** : Gather information about DigitalOcean load balancers
* **community.digitalocean.digital_ocean_monitoring_alerts_info** : Programmatically retrieve metrics as well as configure alert policies based on these metrics
* **community.digitalocean.digital_ocean_project** : Manage a DigitalOcean project
* **community.digitalocean.digital_ocean_project_info** : Gather information about DigitalOcean Projects
* **community.digitalocean.digital_ocean_region_info** : Gather information about DigitalOcean regions
* **community.digitalocean.digital_ocean_size_info** : Gather information about DigitalOcean Droplet sizes
* **community.digitalocean.digital_ocean_snapshot** : Create and delete DigitalOcean snapshots
* **community.digitalocean.digital_ocean_snapshot_info** : Gather information about DigitalOcean Snapshot
* **community.digitalocean.digital_ocean_spaces** : Create and remove DigitalOcean Spaces.
* **community.digitalocean.digital_ocean_spaces_info** : List DigitalOcean Spaces.
* **community.digitalocean.digital_ocean_sshkey** : Manage DigitalOcean SSH keys
* **community.digitalocean.digital_ocean_sshkey_info** : Gather information about DigitalOcean SSH keys
* **community.digitalocean.digital_ocean_tag** : Create and remove tag(s) to DigitalOcean resource.
* **community.digitalocean.digital_ocean_tag_info** : Gather information about DigitalOcean tags
* **community.digitalocean.digital_ocean_volume_info** : Gather information about DigitalOcean volumes
* **community.digitalocean.digital_ocean_vpc** : Create and delete DigitalOcean VPCs
* **community.digitalocean.digital_ocean_vpc_info** : Gather information about DigitalOcean VPCs

## `community.dns` collection

* **community.dns.hetzner_dns_record** : Add or delete a single record in Hetzner DNS service
* **community.dns.hetzner_dns_record_info** : Retrieve records in Hetzner DNS service
* **community.dns.hetzner_dns_record_set** : Add or delete record sets in Hetzner DNS service
* **community.dns.hetzner_dns_record_set_info** : Retrieve record sets in Hetzner DNS service
* **community.dns.hetzner_dns_record_sets** : Bulk synchronize DNS record sets in Hetzner DNS service
* **community.dns.hetzner_dns_zone_info** : Retrieve zone information in Hetzner DNS service
* **community.dns.hosttech_dns_record** : Add or delete a single record in Hosttech DNS service
* **community.dns.hosttech_dns_record_info** : Retrieve records in Hosttech DNS service
* **community.dns.hosttech_dns_record_set** : Add or delete record sets in Hosttech DNS service
* **community.dns.hosttech_dns_record_set_info** : Retrieve record sets in Hosttech DNS service
* **community.dns.hosttech_dns_record_sets** : Bulk synchronize DNS record sets in Hosttech DNS service
* **community.dns.hosttech_dns_zone_info** : Retrieve zone information in Hosttech DNS service
* **community.dns.wait_for_txt** : Wait for TXT entries to be available on all authoritative nameservers

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

## `community.fortios` collection

* **community.fortios.faz_device** : Add or remove device
* **community.fortios.fmgr_device** : Add or remove device from FortiManager.
* **community.fortios.fmgr_device_config** : Edit device configurations
* **community.fortios.fmgr_device_group** : Alter FortiManager device groups.
* **community.fortios.fmgr_device_provision_template** : Manages Device Provisioning Templates in FortiManager.
* **community.fortios.fmgr_fwobj_address** : Allows the management of firewall objects in FortiManager
* **community.fortios.fmgr_fwobj_ippool6** : Allows the editing of IP Pool Objects within FortiManager.
* **community.fortios.fmgr_fwobj_service** : Manages FortiManager Firewall Service Objects.
* **community.fortios.fmgr_fwobj_vip** : Manages Virtual IPs objects in FortiManager
* **community.fortios.fmgr_fwpol_ipv4** : Allows the add/delete of Firewall Policies on Packages in FortiManager.
* **community.fortios.fmgr_fwpol_package** : Manages FortiManager Firewall Policies Packages.
* **community.fortios.fmgr_ha** : Manages the High-Availability State of FortiManager Clusters and Nodes.
* **community.fortios.fmgr_provisioning** : Provision devices via FortiMananger
* **community.fortios.fmgr_query** : Query FortiManager data objects for use in Ansible workflows.
* **community.fortios.fmgr_script** : Add/Edit/Delete and execute scripts
* **community.fortios.fmgr_secprof_appctrl** : Manage application control security profiles
* **community.fortios.fmgr_secprof_av** : Manage security profile
* **community.fortios.fmgr_secprof_dns** : Manage DNS security profiles in FortiManager
* **community.fortios.fmgr_secprof_ips** : Managing IPS security profiles in FortiManager
* **community.fortios.fmgr_secprof_profile_group** : Manage security profiles within FortiManager
* **community.fortios.fmgr_secprof_proxy** : Manage proxy security profiles in FortiManager
* **community.fortios.fmgr_secprof_spam** : spam filter profile for FMG
* **community.fortios.fmgr_secprof_ssl_ssh** : Manage SSL and SSH security profiles in FortiManager
* **community.fortios.fmgr_secprof_voip** : VOIP security profiles in FMG
* **community.fortios.fmgr_secprof_waf** : FortiManager web application firewall security profile
* **community.fortios.fmgr_secprof_wanopt** : WAN optimization
* **community.fortios.fmgr_secprof_web** : Manage web filter security profiles in FortiManager

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

## `community.google` collection

* **community.google.gc_storage** : This module manages objects/buckets in Google Cloud Storage.
* **community.google.gce_eip** : Create or Destroy Global or Regional External IP addresses.
* **community.google.gce_img** : utilize GCE image resources
* **community.google.gce_instance_template** : create or destroy instance templates of Compute Engine of GCP.
* **community.google.gce_labels** : Create, Update or Destroy GCE Labels.
* **community.google.gce_lb** : create/destroy GCE load-balancer resources
* **community.google.gce_mig** : Create, Update or Destroy a Managed Instance Group (MIG).
* **community.google.gce_net** : create/destroy GCE networks and firewall rules
* **community.google.gce_pd** : utilize GCE persistent disk resources
* **community.google.gce_snapshot** : Create or destroy snapshots for GCE storage volumes
* **community.google.gce_tag** : add or remove tag(s) to/from GCE instances
* **community.google.gcpubsub** : Create and Delete Topics/Subscriptions, Publish and pull messages on PubSub
* **community.google.gcpubsub_info** : List Topics/Subscriptions and Messages from Google PubSub.

## `community.grafana` collection

* **community.grafana.grafana_dashboard** : Manage Grafana dashboards
* **community.grafana.grafana_datasource** : Manage Grafana datasources
* **community.grafana.grafana_folder** : Manage Grafana Folders
* **community.grafana.grafana_notification_channel** : Manage Grafana Notification Channels
* **community.grafana.grafana_organization** : Manage Grafana Organization
* **community.grafana.grafana_plugin** : Manage Grafana plugins via grafana-cli
* **community.grafana.grafana_team** : Manage Grafana Teams
* **community.grafana.grafana_user** : Manage Grafana User

## `community.hashi_vault` collection

* **community.hashi_vault.vault_kv1_get** : Get a secret from HashiCorp Vault&#39;s KV version 1 secret store
* **community.hashi_vault.vault_kv2_delete** : Delete one or more versions of a secret from HashiCorp Vault&#39;s KV version 2 secret store
* **community.hashi_vault.vault_kv2_get** : Get a secret from HashiCorp Vault&#39;s KV version 2 secret store
* **community.hashi_vault.vault_list** : Perform a list operation against HashiCorp Vault
* **community.hashi_vault.vault_login** : Perform a login operation against HashiCorp Vault
* **community.hashi_vault.vault_pki_generate_certificate** : Generates a new set of credentials (private key and certificate) using HashiCorp Vault PKI
* **community.hashi_vault.vault_read** : Perform a read operation against HashiCorp Vault
* **community.hashi_vault.vault_token_create** : Create a HashiCorp Vault token
* **community.hashi_vault.vault_write** : Perform a write operation against HashiCorp Vault

## `community.hrobot` collection

* **community.hrobot.boot** : Set boot configuration
* **community.hrobot.failover_ip** : Manage Hetzner&#39;s failover IPs
* **community.hrobot.failover_ip_info** : Retrieve information on Hetzner&#39;s failover IPs
* **community.hrobot.firewall_info** : Manage Hetzner&#39;s dedicated server firewall
* **community.hrobot.reset** : Reset a dedicated server
* **community.hrobot.reverse_dns** : Set or remove reverse DNS entry for IP
* **community.hrobot.server** : Update server information
* **community.hrobot.server_info** : Query information on one or more servers
* **community.hrobot.ssh_key** : Add, remove or update SSH key
* **community.hrobot.ssh_key_info** : Query information on SSH keys
* **community.hrobot.v_switch** : Manage Hetzner&#39;s vSwitch

## `community.libvirt` collection

* **community.libvirt.virt** : Manages virtual machines supported by libvirt
* **community.libvirt.virt_net** : Manage libvirt network configuration
* **community.libvirt.virt_pool** : Manage libvirt storage pools

## `community.mongodb` collection

* **community.mongodb.mongodb_balancer** : Manages the MongoDB Sharded Cluster Balancer.
* **community.mongodb.mongodb_index** : Creates or drops indexes on MongoDB collections.
* **community.mongodb.mongodb_info** : Gather information about MongoDB instance.
* **community.mongodb.mongodb_maintenance** : Enables or disables maintenance mode for a secondary member.
* **community.mongodb.mongodb_monitoring** : Manages the free monitoring feature.
* **community.mongodb.mongodb_oplog** : Resizes the MongoDB oplog.
* **community.mongodb.mongodb_parameter** : Change an administrative parameter on a MongoDB server
* **community.mongodb.mongodb_replicaset** : Initialises a MongoDB replicaset.
* **community.mongodb.mongodb_role** : Adds or removes a role from a MongoDB database
* **community.mongodb.mongodb_schema** : Manages MongoDB Document Schema Validators.
* **community.mongodb.mongodb_shard** : Add or remove shards from a MongoDB Cluster
* **community.mongodb.mongodb_shard_tag** : Manage Shard Tags.
* **community.mongodb.mongodb_shard_zone** : Manage Shard Zones.
* **community.mongodb.mongodb_shell** : Run commands via the MongoDB shell.
* **community.mongodb.mongodb_shutdown** : Cleans up all database resources and then terminates the mongod/mongos process.
* **community.mongodb.mongodb_status** : Validates the status of the replicaset.
* **community.mongodb.mongodb_stepdown** : Step down the MongoDB node from a PRIMARY state.
* **community.mongodb.mongodb_user** : Adds or removes a user from a MongoDB database

## `community.mysql` collection

* **community.mysql.mysql_db** : Add or remove MySQL databases from a remote host
* **community.mysql.mysql_info** : Gather information about MySQL servers
* **community.mysql.mysql_query** : Run MySQL queries
* **community.mysql.mysql_replication** : Manage MySQL replication
* **community.mysql.mysql_role** : Adds, removes, or updates a MySQL role
* **community.mysql.mysql_user** : Adds or removes a user from a MySQL database
* **community.mysql.mysql_variables** : Manage MySQL global variables

## `community.network` collection

* **community.network.a10_server** : Manage A10 Networks AX/SoftAX/Thunder/vThunder devices&#39; server object.
* **community.network.a10_server_axapi3** : Manage A10 Networks AX/SoftAX/Thunder/vThunder devices
* **community.network.a10_service_group** : Manage A10 Networks AX/SoftAX/Thunder/vThunder devices&#39; service groups.
* **community.network.a10_virtual_server** : Manage A10 Networks AX/SoftAX/Thunder/vThunder devices&#39; virtual servers.
* **community.network.aireos_command** : Run commands on remote devices running Cisco WLC
* **community.network.aireos_config** : Manage Cisco WLC configurations
* **community.network.apconos_command** : Run arbitrary commands on APCON devices
* **community.network.aruba_command** : Run commands on remote devices running Aruba Mobility Controller
* **community.network.aruba_config** : Manage Aruba configuration sections
* **community.network.avi_actiongroupconfig** : Module for setup of ActionGroupConfig Avi RESTful Object
* **community.network.avi_alertconfig** : Module for setup of AlertConfig Avi RESTful Object
* **community.network.avi_alertemailconfig** : Module for setup of AlertEmailConfig Avi RESTful Object
* **community.network.avi_alertscriptconfig** : Module for setup of AlertScriptConfig Avi RESTful Object
* **community.network.avi_alertsyslogconfig** : Module for setup of AlertSyslogConfig Avi RESTful Object
* **community.network.avi_analyticsprofile** : Module for setup of AnalyticsProfile Avi RESTful Object
* **community.network.avi_gslbservice_patch_member** : Avi API Module
* **community.network.avi_api_version** : Avi API Version Module
* **community.network.avi_applicationpersistenceprofile** : Module for setup of ApplicationPersistenceProfile Avi RESTful Object
* **community.network.avi_applicationprofile** : Module for setup of ApplicationProfile Avi RESTful Object
* **community.network.avi_authprofile** : Module for setup of AuthProfile Avi RESTful Object
* **community.network.avi_autoscalelaunchconfig** : Module for setup of AutoScaleLaunchConfig Avi RESTful Object
* **community.network.avi_backup** : Module for setup of Backup Avi RESTful Object
* **community.network.avi_backupconfiguration** : Module for setup of BackupConfiguration Avi RESTful Object
* **community.network.avi_certificatemanagementprofile** : Module for setup of CertificateManagementProfile Avi RESTful Object
* **community.network.avi_cloud** : Module for setup of Cloud Avi RESTful Object
* **community.network.avi_cloudconnectoruser** : Module for setup of CloudConnectorUser Avi RESTful Object
* **community.network.avi_cloudproperties** : Module for setup of CloudProperties Avi RESTful Object
* **community.network.avi_cluster** : Module for setup of Cluster Avi RESTful Object
* **community.network.avi_clusterclouddetails** : Module for setup of ClusterCloudDetails Avi RESTful Object
* **community.network.avi_controllerproperties** : Module for setup of ControllerProperties Avi RESTful Object
* **community.network.avi_customipamdnsprofile** : Module for setup of CustomIpamDnsProfile Avi RESTful Object
* **community.network.avi_dnspolicy** : Module for setup of DnsPolicy Avi RESTful Object
* **community.network.avi_errorpagebody** : Module for setup of ErrorPageBody Avi RESTful Object
* **community.network.avi_errorpageprofile** : Module for setup of ErrorPageProfile Avi RESTful Object
* **community.network.avi_gslb** : Module for setup of Gslb Avi RESTful Object
* **community.network.avi_gslbgeodbprofile** : Module for setup of GslbGeoDbProfile Avi RESTful Object
* **community.network.avi_gslbservice** : Module for setup of GslbService Avi RESTful Object
* **community.network.avi_hardwaresecuritymodulegroup** : Module for setup of HardwareSecurityModuleGroup Avi RESTful Object
* **community.network.avi_healthmonitor** : Module for setup of HealthMonitor Avi RESTful Object
* **community.network.avi_httppolicyset** : Module for setup of HTTPPolicySet Avi RESTful Object
* **community.network.avi_ipaddrgroup** : Module for setup of IpAddrGroup Avi RESTful Object
* **community.network.avi_ipamdnsproviderprofile** : Module for setup of IpamDnsProviderProfile Avi RESTful Object
* **community.network.avi_l4policyset** : Module for setup of L4PolicySet Avi RESTful Object
* **community.network.avi_microservicegroup** : Module for setup of MicroServiceGroup Avi RESTful Object
* **community.network.avi_network** : Module for setup of Network Avi RESTful Object
* **community.network.avi_networkprofile** : Module for setup of NetworkProfile Avi RESTful Object
* **community.network.avi_networksecuritypolicy** : Module for setup of NetworkSecurityPolicy Avi RESTful Object
* **community.network.avi_pkiprofile** : Module for setup of PKIProfile Avi RESTful Object
* **community.network.avi_pool** : Module for setup of Pool Avi RESTful Object
* **community.network.avi_poolgroup** : Module for setup of PoolGroup Avi RESTful Object
* **community.network.avi_poolgroupdeploymentpolicy** : Module for setup of PoolGroupDeploymentPolicy Avi RESTful Object
* **community.network.avi_prioritylabels** : Module for setup of PriorityLabels Avi RESTful Object
* **community.network.avi_role** : Module for setup of Role Avi RESTful Object
* **community.network.avi_scheduler** : Module for setup of Scheduler Avi RESTful Object
* **community.network.avi_seproperties** : Module for setup of SeProperties Avi RESTful Object
* **community.network.avi_serverautoscalepolicy** : Module for setup of ServerAutoScalePolicy Avi RESTful Object
* **community.network.avi_serviceengine** : Module for setup of ServiceEngine Avi RESTful Object
* **community.network.avi_serviceenginegroup** : Module for setup of ServiceEngineGroup Avi RESTful Object
* **community.network.avi_snmptrapprofile** : Module for setup of SnmpTrapProfile Avi RESTful Object
* **community.network.avi_sslkeyandcertificate** : Module for setup of SSLKeyAndCertificate Avi RESTful Object
* **community.network.avi_sslprofile** : Module for setup of SSLProfile Avi RESTful Object
* **community.network.avi_stringgroup** : Module for setup of StringGroup Avi RESTful Object
* **community.network.avi_systemconfiguration** : Module for setup of SystemConfiguration Avi RESTful Object
* **community.network.avi_tenant** : Module for setup of Tenant Avi RESTful Object
* **community.network.avi_trafficcloneprofile** : Module for setup of TrafficCloneProfile Avi RESTful Object
* **community.network.avi_user** : Avi User Module
* **community.network.avi_useraccount** : Avi UserAccount Module
* **community.network.avi_useraccountprofile** : Module for setup of UserAccountProfile Avi RESTful Object
* **community.network.avi_virtualservice** : Module for setup of VirtualService Avi RESTful Object
* **community.network.avi_vrfcontext** : Module for setup of VrfContext Avi RESTful Object
* **community.network.avi_vsdatascriptset** : Module for setup of VSDataScriptSet Avi RESTful Object
* **community.network.avi_vsvip** : Module for setup of VsVip Avi RESTful Object
* **community.network.avi_webhook** : Module for setup of Webhook Avi RESTful Object
* **community.network.bcf_switch** : Create and remove a bcf switch.
* **community.network.bigmon_chain** : Create and remove a bigmon inline service chain.
* **community.network.bigmon_policy** : Create and remove a bigmon out-of-band policy.
* **community.network.ce_aaa_server** : Manages AAA server global configuration on HUAWEI CloudEngine switches.
* **community.network.ce_aaa_server_host** : Manages AAA server host configuration on HUAWEI CloudEngine switches.
* **community.network.ce_acl** : Manages base ACL configuration on HUAWEI CloudEngine switches.
* **community.network.ce_acl_advance** : Manages advanced ACL configuration on HUAWEI CloudEngine switches.
* **community.network.ce_acl_interface** : Manages applying ACLs to interfaces on HUAWEI CloudEngine switches.
* **community.network.ce_bfd_global** : Manages BFD global configuration on HUAWEI CloudEngine devices.
* **community.network.ce_bfd_session** : Manages BFD session configuration on HUAWEI CloudEngine devices.
* **community.network.ce_bfd_view** : Manages BFD session view configuration on HUAWEI CloudEngine devices.
* **community.network.ce_bgp** : Manages BGP configuration on HUAWEI CloudEngine switches.
* **community.network.ce_bgp_af** : Manages BGP Address-family configuration on HUAWEI CloudEngine switches.
* **community.network.ce_bgp_neighbor** : Manages BGP peer configuration on HUAWEI CloudEngine switches.
* **community.network.ce_bgp_neighbor_af** : Manages BGP neighbor Address-family configuration on HUAWEI CloudEngine switches.
* **community.network.ce_command** : Run arbitrary command on HUAWEI CloudEngine devices.
* **community.network.ce_config** : Manage Huawei CloudEngine configuration sections.
* **community.network.ce_dldp** : Manages global DLDP configuration on HUAWEI CloudEngine switches.
* **community.network.ce_dldp_interface** : Manages interface DLDP configuration on HUAWEI CloudEngine switches.
* **community.network.ce_eth_trunk** : Manages Eth-Trunk interfaces on HUAWEI CloudEngine switches.
* **community.network.ce_evpn_bd_vni** : Manages EVPN VXLAN Network Identifier (VNI) on HUAWEI CloudEngine switches.
* **community.network.ce_evpn_bgp** : Manages BGP EVPN configuration on HUAWEI CloudEngine switches.
* **community.network.ce_evpn_bgp_rr** : Manages RR for the VXLAN Network on HUAWEI CloudEngine switches.
* **community.network.ce_evpn_global** : Manages global configuration of EVPN on HUAWEI CloudEngine switches.
* **community.network.ce_facts** : Gets facts about HUAWEI CloudEngine switches.
* **community.network.ce_file_copy** : Copy a file to a remote cloudengine device over SCP on HUAWEI CloudEngine switches.
* **community.network.ce_info_center_debug** : Manages information center debug configuration on HUAWEI CloudEngine switches.
* **community.network.ce_info_center_global** : Manages outputting logs on HUAWEI CloudEngine switches.
* **community.network.ce_info_center_log** : Manages information center log configuration on HUAWEI CloudEngine switches.
* **community.network.ce_info_center_trap** : Manages information center trap configuration on HUAWEI CloudEngine switches.
* **community.network.ce_interface** : Manages physical attributes of interfaces on HUAWEI CloudEngine switches.
* **community.network.ce_interface_ospf** : Manages configuration of an OSPF interface instanceon HUAWEI CloudEngine switches.
* **community.network.ce_ip_interface** : Manages L3 attributes for IPv4 and IPv6 interfaces on HUAWEI CloudEngine switches.
* **community.network.ce_is_is_instance** : Manages isis process id configuration on HUAWEI CloudEngine devices.
* **community.network.ce_is_is_interface** : Manages isis interface configuration on HUAWEI CloudEngine devices.
* **community.network.ce_is_is_view** : Manages isis view configuration on HUAWEI CloudEngine devices.
* **community.network.ce_lacp** : Manages Eth-Trunk interfaces on HUAWEI CloudEngine switches
* **community.network.ce_link_status** : Get interface link status on HUAWEI CloudEngine switches.
* **community.network.ce_lldp** : Manages LLDP configuration on HUAWEI CloudEngine switches.
* **community.network.ce_lldp_interface** : Manages INTERFACE LLDP configuration on HUAWEI CloudEngine switches.
* **community.network.ce_mdn_interface** : Manages MDN configuration on HUAWEI CloudEngine switches.
* **community.network.ce_mlag_config** : Manages MLAG configuration on HUAWEI CloudEngine switches.
* **community.network.ce_mlag_interface** : Manages MLAG interfaces on HUAWEI CloudEngine switches.
* **community.network.ce_mtu** : Manages MTU settings on HUAWEI CloudEngine switches.
* **community.network.ce_multicast_global** : Manages multicast global configuration on HUAWEI CloudEngine switches.
* **community.network.ce_multicast_igmp_enable** : Manages multicast igmp enable configuration on HUAWEI CloudEngine switches.
* **community.network.ce_netconf** : Run an arbitrary netconf command on HUAWEI CloudEngine switches.
* **community.network.ce_netstream_aging** : Manages timeout mode of NetStream on HUAWEI CloudEngine switches.
* **community.network.ce_netstream_export** : Manages netstream export on HUAWEI CloudEngine switches.
* **community.network.ce_netstream_global** : Manages global parameters of NetStream on HUAWEI CloudEngine switches.
* **community.network.ce_netstream_template** : Manages NetStream template configuration on HUAWEI CloudEngine switches.
* **community.network.ce_ntp** : Manages core NTP configuration on HUAWEI CloudEngine switches.
* **community.network.ce_ntp_auth** : Manages NTP authentication configuration on HUAWEI CloudEngine switches.
* **community.network.ce_ospf** : Manages configuration of an OSPF instance on HUAWEI CloudEngine switches.
* **community.network.ce_ospf_vrf** : Manages configuration of an OSPF VPN instance on HUAWEI CloudEngine switches.
* **community.network.ce_reboot** : Reboot a HUAWEI CloudEngine switches.
* **community.network.ce_rollback** : Set a checkpoint or rollback to a checkpoint on HUAWEI CloudEngine switches.
* **community.network.ce_sflow** : Manages sFlow configuration on HUAWEI CloudEngine switches.
* **community.network.ce_snmp_community** : Manages SNMP community configuration on HUAWEI CloudEngine switches.
* **community.network.ce_snmp_contact** : Manages SNMP contact configuration on HUAWEI CloudEngine switches.
* **community.network.ce_snmp_location** : Manages SNMP location configuration on HUAWEI CloudEngine switches.
* **community.network.ce_snmp_target_host** : Manages SNMP target host configuration on HUAWEI CloudEngine switches.
* **community.network.ce_snmp_traps** : Manages SNMP traps configuration on HUAWEI CloudEngine switches.
* **community.network.ce_snmp_user** : Manages SNMP user configuration on HUAWEI CloudEngine switches.
* **community.network.ce_startup** : Manages a system startup information on HUAWEI CloudEngine switches.
* **community.network.ce_static_route_bfd** : Manages static route configuration on HUAWEI CloudEngine switches.
* **community.network.ce_stp** : Manages STP configuration on HUAWEI CloudEngine switches.
* **community.network.ce_switchport** : Manages Layer 2 switchport interfaces on HUAWEI CloudEngine switches.
* **community.network.ce_vlan** : Manages VLAN resources and attributes on Huawei CloudEngine switches.
* **community.network.ce_vrf** : Manages VPN instance on HUAWEI CloudEngine switches.
* **community.network.ce_vrf_af** : Manages VPN instance address family on HUAWEI CloudEngine switches.
* **community.network.ce_vrf_interface** : Manages interface specific VPN configuration on HUAWEI CloudEngine switches.
* **community.network.ce_vrrp** : Manages VRRP interfaces on HUAWEI CloudEngine devices.
* **community.network.ce_vxlan_arp** : Manages ARP attributes of VXLAN on HUAWEI CloudEngine devices.
* **community.network.ce_vxlan_gateway** : Manages gateway for the VXLAN network on HUAWEI CloudEngine devices.
* **community.network.ce_vxlan_global** : Manages global attributes of VXLAN and bridge domain on HUAWEI CloudEngine devices.
* **community.network.ce_vxlan_tunnel** : Manages VXLAN tunnel configuration on HUAWEI CloudEngine devices.
* **community.network.ce_vxlan_vap** : Manages VXLAN virtual access point on HUAWEI CloudEngine Devices.
* **community.network.cnos_backup** : Backup the current running or startup configuration to a remote server on devices running Lenovo CNOS
* **community.network.cnos_banner** : Manage multiline banners on Lenovo CNOS devices
* **community.network.cnos_bgp** : Manage BGP resources and attributes on devices running CNOS
* **community.network.cnos_command** : Run arbitrary commands on Lenovo CNOS devices
* **community.network.cnos_conditional_command** : Execute a single command based on condition on devices running Lenovo CNOS
* **community.network.cnos_conditional_template** : Manage switch configuration using templates based on condition on devices running Lenovo CNOS
* **community.network.cnos_config** : Manage Lenovo CNOS configuration sections
* **community.network.cnos_factory** : Reset the switch startup configuration to default (factory) on devices running Lenovo CNOS.
* **community.network.cnos_facts** : Collect facts from remote devices running Lenovo CNOS
* **community.network.cnos_image** : Perform firmware upgrade/download from a remote server on devices running Lenovo CNOS
* **community.network.cnos_interface** : Manage Interface on Lenovo CNOS network devices
* **community.network.cnos_l2_interface** : Manage Layer-2 interface on Lenovo CNOS devices.
* **community.network.cnos_l3_interface** : Manage Layer-3 interfaces on Lenovo CNOS network devices.
* **community.network.cnos_linkagg** : Manage link aggregation groups on Lenovo CNOS devices
* **community.network.cnos_lldp** : Manage LLDP configuration on Lenovo CNOS network devices.
* **community.network.cnos_logging** : Manage logging on network devices
* **community.network.cnos_reload** : Perform switch restart on devices running Lenovo CNOS
* **community.network.cnos_rollback** : Roll back the running or startup configuration from a remote server on devices running Lenovo CNOS
* **community.network.cnos_save** : Save the running configuration as the startup configuration on devices running Lenovo CNOS
* **community.network.cnos_showrun** : Collect the current running configuration on devices running on CNOS
* **community.network.cnos_static_route** : Manage static IP routes on Lenovo CNOS network devices
* **community.network.cnos_system** : Manage the system attributes on Lenovo CNOS devices
* **community.network.cnos_template** : Manage switch configuration using templates on devices running Lenovo CNOS
* **community.network.cnos_user** : Manage the collection of local users on Lenovo CNOS devices
* **community.network.cnos_vlag** : Manage VLAG resources and attributes on devices running Lenovo CNOS
* **community.network.cnos_vlan** : Manage VLANs on CNOS network devices
* **community.network.cnos_vrf** : Manage VRFs on Lenovo CNOS network devices
* **community.network.cv_server_provision** : Provision server port by applying or removing template configuration to an Arista CloudVision Portal configlet that is applied to a switch.
* **community.network.dladm_etherstub** : Manage etherstubs on Solaris/illumos systems.
* **community.network.dladm_iptun** : Manage IP tunnel interfaces on Solaris/illumos systems.
* **community.network.dladm_linkprop** : Manage link properties on Solaris/illumos systems.
* **community.network.dladm_vlan** : Manage VLAN interfaces on Solaris/illumos systems.
* **community.network.dladm_vnic** : Manage VNICs on Solaris/illumos systems.
* **community.network.edgeos_command** : Run one or more commands on EdgeOS devices
* **community.network.edgeos_config** : Manage EdgeOS configuration on remote device
* **community.network.edgeos_facts** : Collect facts from remote devices running EdgeOS
* **community.network.edgeswitch_facts** : Collect facts from remote devices running Edgeswitch
* **community.network.edgeswitch_vlan** : Manage VLANs on Ubiquiti Edgeswitch network devices
* **community.network.enos_command** : Run arbitrary commands on Lenovo ENOS devices
* **community.network.enos_config** : Manage Lenovo ENOS configuration sections
* **community.network.enos_facts** : Collect facts from remote devices running Lenovo ENOS
* **community.network.eric_eccli_command** : Run commands on remote devices running ERICSSON ECCLI
* **community.network.exos_command** : Run commands on remote devices running Extreme EXOS
* **community.network.exos_config** : Manage Extreme Networks EXOS configuration sections
* **community.network.exos_facts** : Collect facts from devices running Extreme EXOS
* **community.network.exos_l2_interfaces** : Manage L2 interfaces on Extreme Networks EXOS devices.
* **community.network.exos_lldp_global** : Configure and manage Link Layer Discovery Protocol(LLDP) attributes on EXOS platforms.
* **community.network.exos_lldp_interfaces** : Manage link layer discovery protocol (LLDP) attributes of interfaces on EXOS platforms.
* **community.network.exos_vlans** : Manage VLANs on Extreme Networks EXOS devices.
* **community.network.flowadm** : Manage bandwidth resource control and priority for protocols, services and zones on Solaris/illumos systems
* **community.network.ftd_configuration** : Manages configuration on Cisco FTD devices over REST API
* **community.network.ftd_file_download** : Downloads files from Cisco FTD devices over HTTP(S)
* **community.network.ftd_file_upload** : Uploads files to Cisco FTD devices over HTTP(S)
* **community.network.ftd_install** : Installs FTD pkg image on the firewall
* **community.network.iap_start_workflow** : Start a workflow in the Itential Automation Platform
* **community.network.iap_token** : Get token for the Itential Automation Platform
* **community.network.icx_banner** : Manage multiline banners on Ruckus ICX 7000 series switches
* **community.network.icx_command** : Run arbitrary commands on remote Ruckus ICX 7000 series switches
* **community.network.icx_config** : Manage configuration sections of Ruckus ICX 7000 series switches
* **community.network.icx_copy** : Transfer files from or to remote Ruckus ICX 7000 series switches
* **community.network.icx_facts** : Collect facts from remote Ruckus ICX 7000 series switches
* **community.network.icx_interface** : Manage Interface on Ruckus ICX 7000 series switches
* **community.network.icx_l3_interface** : Manage Layer-3 interfaces on Ruckus ICX 7000 series switches
* **community.network.icx_linkagg** : Manage link aggregation groups on Ruckus ICX 7000 series switches
* **community.network.icx_lldp** : Manage LLDP configuration on Ruckus ICX 7000 series switches
* **community.network.icx_logging** : Manage logging on Ruckus ICX 7000 series switches
* **community.network.icx_ping** : Tests reachability using ping from Ruckus ICX 7000 series switches
* **community.network.icx_static_route** : Manage static IP routes on Ruckus ICX 7000 series switches
* **community.network.icx_system** : Manage the system attributes on Ruckus ICX 7000 series switches
* **community.network.icx_user** : Manage the user accounts on Ruckus ICX 7000 series switches.
* **community.network.icx_vlan** : Manage VLANs on Ruckus ICX 7000 series switches
* **community.network.ig_config** : Manage the configuration database on an Ingate SBC.
* **community.network.ig_unit_information** : Get unit information from an Ingate SBC.
* **community.network.ipadm_addr** : Manage IP addresses on an interface on Solaris/illumos systems
* **community.network.ipadm_addrprop** : Manage IP address properties on Solaris/illumos systems.
* **community.network.ipadm_if** : Manage IP interfaces  on Solaris/illumos systems.
* **community.network.ipadm_ifprop** : Manage IP interface properties on Solaris/illumos systems.
* **community.network.ipadm_prop** : Manage protocol properties on Solaris/illumos systems.
* **community.network.ironware_command** : Run arbitrary commands on Extreme IronWare devices
* **community.network.ironware_config** : Manage configuration sections on Extreme Ironware devices
* **community.network.ironware_facts** : Collect facts from devices running Extreme Ironware
* **community.network.nclu** : Configure network interfaces using NCLU
* **community.network.netact_cm_command** : Manage network configuration data in Nokia Core and Radio networks
* **community.network.netscaler_cs_action** : Manage content switching actions
* **community.network.netscaler_cs_policy** : Manage content switching policy
* **community.network.netscaler_cs_vserver** : Manage content switching vserver
* **community.network.netscaler_gslb_service** : Manage gslb service entities in Netscaler.
* **community.network.netscaler_gslb_site** : Manage gslb site entities in Netscaler.
* **community.network.netscaler_gslb_vserver** : Configure gslb vserver entities in Netscaler.
* **community.network.netscaler_lb_monitor** : Manage load balancing monitors
* **community.network.netscaler_lb_vserver** : Manage load balancing vserver configuration
* **community.network.netscaler_nitro_request** : Issue Nitro API requests to a Netscaler instance.
* **community.network.netscaler_save_config** : Save Netscaler configuration.
* **community.network.netscaler_server** : Manage server configuration
* **community.network.netscaler_service** : Manage service configuration in Netscaler
* **community.network.netscaler_servicegroup** : Manage service group configuration in Netscaler
* **community.network.netscaler_ssl_certkey** : Manage ssl certificate keys.
* **community.network.nos_command** : Run commands on remote devices running Extreme Networks NOS
* **community.network.nos_config** : Manage Extreme Networks NOS configuration sections
* **community.network.nos_facts** : Collect facts from devices running Extreme NOS
* **community.network.nuage_vspk** : Manage Nuage VSP environments
* **community.network.opx_cps** : CPS operations on networking device running Openswitch (OPX)
* **community.network.ordnance_config** : Manage Ordnance configuration sections
* **community.network.ordnance_facts** : Collect facts from Ordnance Virtual Routers over SSH
* **community.network.pn_access_list** : CLI command to create/delete access-list
* **community.network.pn_access_list_ip** : CLI command to add/remove access-list-ip
* **community.network.pn_admin_service** : CLI command to modify admin-service
* **community.network.pn_admin_session_timeout** : CLI command to modify admin-session-timeout
* **community.network.pn_admin_syslog** : CLI command to create/modify/delete admin-syslog
* **community.network.pn_connection_stats_settings** : CLI command to modify connection-stats-settings
* **community.network.pn_cpu_class** : CLI command to create/modify/delete cpu-class
* **community.network.pn_cpu_mgmt_class** : CLI command to modify cpu-mgmt-class
* **community.network.pn_dhcp_filter** : CLI command to create/modify/delete dhcp-filter
* **community.network.pn_dscp_map** : CLI command to create/delete dscp-map
* **community.network.pn_dscp_map_pri_map** : CLI command to modify dscp-map-pri-map
* **community.network.pn_fabric_local** : CLI command to modify fabric-local
* **community.network.pn_igmp_snooping** : CLI command to modify igmp-snooping
* **community.network.pn_ipv6security_raguard** : CLI command to create/modify/delete ipv6security-raguard
* **community.network.pn_ipv6security_raguard_port** : CLI command to add/remove ipv6security-raguard-port
* **community.network.pn_ipv6security_raguard_vlan** : CLI command to add/remove ipv6security-raguard-vlan
* **community.network.pn_log_audit_exception** : CLI command to create/delete an audit exception
* **community.network.pn_port_config** : CLI command to modify port-config
* **community.network.pn_port_cos_bw** : CLI command to modify port-cos-bw
* **community.network.pn_port_cos_rate_setting** : CLI command to modify port-cos-rate-setting
* **community.network.pn_prefix_list** : CLI command to create/delete prefix-list
* **community.network.pn_prefix_list_network** : CLI command to add/remove prefix-list-network
* **community.network.pn_role** : CLI command to create/delete/modify role
* **community.network.pn_snmp_community** : CLI command to create/modify/delete snmp-community
* **community.network.pn_snmp_trap_sink** : CLI command to create/delete snmp-trap-sink
* **community.network.pn_snmp_vacm** : CLI command to create/modify/delete snmp-vacm
* **community.network.pn_stp** : CLI command to modify stp
* **community.network.pn_stp_port** : CLI command to modify stp-port.
* **community.network.pn_switch_setup** : CLI command to modify switch-setup
* **community.network.pn_user** : CLI command to create/modify/delete user
* **community.network.pn_vflow_table_profile** : CLI command to modify vflow-table-profile
* **community.network.pn_vrouter_bgp** : CLI command to add/modify/remove vrouter-bgp
* **community.network.pn_vrouter_bgp_network** : CLI command to add/remove vrouter-bgp-network
* **community.network.pn_vrouter_interface_ip** : CLI command to add/remove vrouter-interface-ip
* **community.network.pn_vrouter_loopback_interface** : CLI command to add/remove vrouter-loopback-interface
* **community.network.pn_vrouter_ospf** : CLI command to add/remove vrouter-ospf
* **community.network.pn_vrouter_ospf6** : CLI command to add/remove vrouter-ospf6
* **community.network.pn_vrouter_packet_relay** : CLI command to add/remove vrouter-packet-relay
* **community.network.pn_vrouter_pim_config** : CLI command to modify vrouter-pim-config
* **community.network.pn_vtep** : CLI command to create/delete vtep
* **community.network.slxos_command** : Run commands on remote devices running Extreme Networks SLX-OS
* **community.network.slxos_config** : Manage Extreme Networks SLX-OS configuration sections
* **community.network.slxos_facts** : Collect facts from devices running Extreme SLX-OS
* **community.network.slxos_interface** : Manage Interfaces on Extreme SLX-OS network devices
* **community.network.slxos_l2_interface** : Manage Layer-2 interface on Extreme Networks SLX-OS devices.
* **community.network.slxos_l3_interface** : Manage L3 interfaces on Extreme Networks SLX-OS network devices.
* **community.network.slxos_linkagg** : Manage link aggregation groups on Extreme Networks SLX-OS network devices
* **community.network.slxos_lldp** : Manage LLDP configuration on Extreme Networks SLX-OS network devices.
* **community.network.slxos_vlan** : Manage VLANs on Extreme Networks SLX-OS network devices
* **community.network.sros_command** : Run commands on remote devices running Nokia SR OS
* **community.network.sros_config** : Manage Nokia SR OS device configuration
* **community.network.sros_rollback** : Configure Nokia SR OS rollback
* **community.network.vdirect_commit** : Commits pending configuration changes on Radware devices
* **community.network.vdirect_file** : Uploads a new or updates an existing runnable file into Radware vDirect server
* **community.network.vdirect_runnable** : Runs templates and workflow actions in Radware vDirect server
* **community.network.voss_command** : Run commands on remote devices running Extreme VOSS
* **community.network.voss_config** : Manage Extreme VOSS configuration sections
* **community.network.voss_facts** : Collect facts from remote devices running Extreme VOSS

## `community.okd` collection

* **community.okd.k8s** : Manage OpenShift objects
* **community.okd.openshift_adm_groups_sync** : Sync OpenShift Groups with records from an external provider.
* **community.okd.openshift_adm_migrate_template_instances** : Update TemplateInstances to point to the latest group-version-kinds
* **community.okd.openshift_adm_prune_auth** : Removes references to the specified roles, clusterroles, users, and groups
* **community.okd.openshift_adm_prune_builds** : Prune old completed and failed builds
* **community.okd.openshift_adm_prune_deployments** : Remove old completed and failed deployment configs
* **community.okd.openshift_adm_prune_images** : Remove unreferenced images
* **community.okd.openshift_auth** : Authenticate to OpenShift clusters which require an explicit login step
* **community.okd.openshift_build** : Start a new build or Cancel running, pending, or new builds.
* **community.okd.openshift_import_image** : Import the latest image information from a tag in a container image registry.
* **community.okd.openshift_process** : Process an OpenShift template.openshift.io/v1 Template
* **community.okd.openshift_registry_info** : Display information about the integrated registry.
* **community.okd.openshift_route** : Expose a Service as an OpenShift Route.

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

## `community.proxysql` collection

* **community.proxysql.proxysql_backend_servers** : Adds or removes mysql hosts from proxysql admin interface
* **community.proxysql.proxysql_global_variables** : Gets or sets the proxysql global variables
* **community.proxysql.proxysql_info** : Gathers information about proxysql server
* **community.proxysql.proxysql_manage_config** : Writes the proxysql configuration settings between layers
* **community.proxysql.proxysql_mysql_users** : Adds or removes mysql users from proxysql admin interface
* **community.proxysql.proxysql_query_rules** : Modifies query rules using the proxysql admin interface
* **community.proxysql.proxysql_query_rules_fast_routing** : Modifies query rules for fast routing policies using the proxysql admin interface
* **community.proxysql.proxysql_replication_hostgroups** : Manages replication hostgroups using the proxysql admin interface
* **community.proxysql.proxysql_scheduler** : Adds or removes schedules from proxysql admin interface

## `community.rabbitmq` collection

* **community.rabbitmq.rabbitmq_binding** : Manage rabbitMQ bindings
* **community.rabbitmq.rabbitmq_exchange** : Manage rabbitMQ exchange
* **community.rabbitmq.rabbitmq_feature_flag** : Enables feature flag
* **community.rabbitmq.rabbitmq_global_parameter** : Manage RabbitMQ global parameters
* **community.rabbitmq.rabbitmq_parameter** : Manage RabbitMQ parameters
* **community.rabbitmq.rabbitmq_plugin** : Manage RabbitMQ plugins
* **community.rabbitmq.rabbitmq_policy** : Manage the state of policies in RabbitMQ
* **community.rabbitmq.rabbitmq_publish** : Publish a message to a RabbitMQ queue.
* **community.rabbitmq.rabbitmq_queue** : Manage rabbitMQ queues
* **community.rabbitmq.rabbitmq_upgrade** : Execute rabbitmq-upgrade commands
* **community.rabbitmq.rabbitmq_user** : Manage RabbitMQ users
* **community.rabbitmq.rabbitmq_user_limits** : Manage RabbitMQ user limits
* **community.rabbitmq.rabbitmq_vhost** : Manage the state of a virtual host in RabbitMQ
* **community.rabbitmq.rabbitmq_vhost_limits** : Manage the state of virtual host limits in RabbitMQ

## `community.routeros` collection

* **community.routeros.api** : Ansible module for RouterOS API
* **community.routeros.api_facts** : Collect facts from remote devices running MikroTik RouterOS using the API
* **community.routeros.api_find_and_modify** : Find and modify information using the API
* **community.routeros.api_info** : Retrieve information from API
* **community.routeros.api_modify** : Modify data at paths with API
* **community.routeros.command** : Run commands on remote devices running MikroTik RouterOS
* **community.routeros.facts** : Collect facts from remote devices running MikroTik RouterOS

## `community.sap` collection

* **community.sap.hana_query** : Execute SQL on HANA
* **community.sap.sapcar_extract** : Manages SAP SAPCAR archives
* **community.sap.sap_company** : This module will manage a company entities in a SAP S4HANA environment
* **community.sap.sap_user** : This module will manage a user entities in a SAP S4/HANA environment
* **community.sap.sap_snote** : This module will upload and (de)implements C(SNOTES) in a SAP S4HANA environment.
* **community.sap.sap_system_facts** : Gathers SAP facts in a host
* **community.sap.sap_task_list_execute** : Perform SAP Task list execution

## `community.sap_libs` collection

* **community.sap_libs.sap_company** : This module will manage a company entities in a SAP S4HANA environment
* **community.sap_libs.sap_control_exec** : Ansible Module to execute SAPCONTROL
* **community.sap_libs.sap_hdbsql** : Ansible Module to execute SQL on SAP HANA
* **community.sap_libs.sap_pyrfc** : Ansible Module for use of SAP PyRFC to execute SAP RFCs (Remote Function Calls) to SAP remote-enabled function modules
* **community.sap_libs.sap_snote** : This module will upload and (de)implements C(SNOTES) in a SAP S4HANA environment.
* **community.sap_libs.sap_system_facts** : Gathers SAP facts in a host
* **community.sap_libs.sap_task_list_execute** : Perform SAP Task list execution
* **community.sap_libs.sap_user** : This module will manage a user entities in a SAP S4/HANA environment
* **community.sap_libs.sapcar_extract** : Manages SAP SAPCAR archives

## `community.skydive` collection

* **community.skydive.skydive_capture** : Module which manages flow capture on interfaces
* **community.skydive.skydive_edge** : Module to add edges to Skydive topology
* **community.skydive.skydive_node** : Module which add nodes to Skydive topology

## `community.sops` collection

* **community.sops.load_vars** : Load sops-encrypted variables from files, dynamically within a task
* **community.sops.sops_encrypt** : Encrypt data with sops

## `community.vmware` collection

* **community.vmware.vcenter_domain_user_group_info** : Gather user or group information of a domain
* **community.vmware.vcenter_extension** : Register/deregister vCenter Extensions
* **community.vmware.vcenter_extension_info** : Gather info vCenter extensions
* **community.vmware.vcenter_folder** : Manage folders on given datacenter
* **community.vmware.vcenter_license** : Manage VMware vCenter license keys
* **community.vmware.vcenter_standard_key_provider** : Add, reconfigure or remove Standard Key Provider on vCenter server
* **community.vmware.vmware_about_info** : Provides information about VMware server to which user is connecting to
* **community.vmware.vmware_category** : Manage VMware categories
* **community.vmware.vmware_category_info** : Gather info about VMware tag categories
* **community.vmware.vmware_cfg_backup** : Backup / Restore / Reset ESXi host configuration
* **community.vmware.vmware_cluster** : Manage VMware vSphere clusters
* **community.vmware.vmware_cluster_dpm** : Manage Distributed Power Management (DPM) on VMware vSphere clusters
* **community.vmware.vmware_cluster_drs** : Manage Distributed Resource Scheduler (DRS) on VMware vSphere clusters
* **community.vmware.vmware_cluster_ha** : Manage High Availability (HA) on VMware vSphere clusters
* **community.vmware.vmware_cluster_info** : Gather info about clusters available in given vCenter
* **community.vmware.vmware_cluster_vcls** : Override the default vCLS (vSphere Cluster Services) VM disk placement for this cluster.
* **community.vmware.vmware_cluster_vsan** : Manages virtual storage area network (vSAN) configuration on VMware vSphere clusters
* **community.vmware.vmware_content_deploy_ovf_template** : Deploy Virtual Machine from ovf template stored in content library.
* **community.vmware.vmware_content_deploy_template** : Deploy Virtual Machine from template stored in content library.
* **community.vmware.vmware_content_library_info** : Gather information about VMWare Content Library
* **community.vmware.vmware_content_library_manager** : Create, update and delete VMware content library
* **community.vmware.vmware_custom_attribute** : Manage custom attributes definitions
* **community.vmware.vmware_custom_attribute_manager** : Manage custom attributes from VMware for the given vSphere object
* **community.vmware.vmware_datacenter** : Manage VMware vSphere Datacenters
* **community.vmware.vmware_datacenter_info** : Gather information about VMware vSphere Datacenters
* **community.vmware.vmware_datastore** : Configure Datastores
* **community.vmware.vmware_datastore_cluster** : Manage VMware vSphere datastore clusters
* **community.vmware.vmware_datastore_cluster_manager** : Manage VMware vSphere datastore cluster&#39;s members
* **community.vmware.vmware_datastore_info** : Gather info about datastores available in given vCenter
* **community.vmware.vmware_datastore_maintenancemode** : Place a datastore into maintenance mode
* **community.vmware.vmware_deploy_ovf** : Deploys a VMware virtual machine from an OVF or OVA file
* **community.vmware.vmware_drs_group** : Creates vm/host group in a given cluster.
* **community.vmware.vmware_drs_group_info** : Gathers info about DRS VM/Host groups on the given cluster
* **community.vmware.vmware_drs_group_manager** : Manage VMs and Hosts in DRS group.
* **community.vmware.vmware_drs_rule_info** : Gathers info about DRS rule on the given cluster
* **community.vmware.vmware_dvs_host** : Add or remove a host from distributed virtual switch
* **community.vmware.vmware_dvs_portgroup** : Create or remove a Distributed vSwitch portgroup.
* **community.vmware.vmware_dvs_portgroup_find** : Find portgroup(s) in a VMware environment
* **community.vmware.vmware_dvs_portgroup_info** : Gathers info DVS portgroup configurations
* **community.vmware.vmware_dvswitch** : Create or remove a Distributed Switch
* **community.vmware.vmware_dvswitch_info** : Gathers info dvswitch configurations
* **community.vmware.vmware_dvswitch_lacp** : Manage LACP configuration on a Distributed Switch
* **community.vmware.vmware_dvswitch_nioc** : Manage distributed switch Network IO Control
* **community.vmware.vmware_dvswitch_pvlans** : Manage Private VLAN configuration of a Distributed Switch
* **community.vmware.vmware_dvswitch_uplink_pg** : Manage uplink portproup configuration of a Distributed Switch
* **community.vmware.vmware_evc_mode** : Enable/Disable EVC mode on vCenter
* **community.vmware.vmware_export_ovf** : Exports a VMware virtual machine to an OVF file, device files and a manifest file
* **community.vmware.vmware_first_class_disk** : Manage VMware vSphere First Class Disks
* **community.vmware.vmware_folder_info** : Provides information about folders in a datacenter
* **community.vmware.vmware_guest** : Manages virtual machines in vCenter
* **community.vmware.vmware_guest_boot_info** : Gather info about boot options for the given virtual machine
* **community.vmware.vmware_guest_boot_manager** : Manage boot options for the given virtual machine
* **community.vmware.vmware_guest_controller** : Manage disk or USB controllers related to virtual machine in given vCenter infrastructure
* **community.vmware.vmware_guest_cross_vc_clone** : Cross-vCenter VM/template clone
* **community.vmware.vmware_guest_custom_attribute_defs** : Manage custom attributes definitions for virtual machine from VMware
* **community.vmware.vmware_guest_custom_attributes** : Manage custom attributes from VMware for the given virtual machine
* **community.vmware.vmware_guest_customization_info** : Gather info about VM customization specifications
* **community.vmware.vmware_guest_disk** : Manage disks related to virtual machine in given vCenter infrastructure
* **community.vmware.vmware_guest_disk_info** : Gather info about disks of given virtual machine
* **community.vmware.vmware_guest_file_operation** : Files operation in a VMware guest operating system without network
* **community.vmware.vmware_guest_find** : Find the folder path(s) for a virtual machine by name or UUID
* **community.vmware.vmware_guest_info** : Gather info about a single VM
* **community.vmware.vmware_guest_instant_clone** : Instant Clone VM
* **community.vmware.vmware_guest_move** : Moves virtual machines in vCenter
* **community.vmware.vmware_guest_network** : Manage network adapters of specified virtual machine in given vCenter infrastructure
* **community.vmware.vmware_guest_powerstate** : Manages power states of virtual machines in vCenter
* **community.vmware.vmware_guest_register_operation** : VM inventory registration operation
* **community.vmware.vmware_guest_screenshot** : Create a screenshot of the Virtual Machine console.
* **community.vmware.vmware_guest_sendkey** : Send USB HID codes to the Virtual Machine&#39;s keyboard.
* **community.vmware.vmware_guest_serial_port** : Manage serial ports on an existing VM
* **community.vmware.vmware_guest_snapshot** : Manages virtual machines snapshots in vCenter
* **community.vmware.vmware_guest_snapshot_info** : Gather info about virtual machine&#39;s snapshots in vCenter
* **community.vmware.vmware_guest_storage_policy** : Set VM Home and disk(s) storage policy profiles.
* **community.vmware.vmware_guest_tools_info** : Gather info about VMware tools installed in VM
* **community.vmware.vmware_guest_tools_upgrade** : Module to upgrade VMTools
* **community.vmware.vmware_guest_tools_wait** : Wait for VMware tools to become available
* **community.vmware.vmware_guest_tpm** : Add or remove vTPM device for specified VM.
* **community.vmware.vmware_guest_vgpu** : Modify vGPU video card profile of the specified virtual machine in the given vCenter infrastructure
* **community.vmware.vmware_guest_vgpu_info** : Gather information about vGPU profiles of the specified virtual machine in the given vCenter infrastructure
* **community.vmware.vmware_guest_video** : Modify video card configurations of specified virtual machine in given vCenter infrastructure
* **community.vmware.vmware_host** : Add, remove, or move an ESXi host to, from, or within vCenter
* **community.vmware.vmware_host_acceptance** : Manage the host acceptance level of an ESXi host
* **community.vmware.vmware_host_active_directory** : Joins an ESXi host system to an Active Directory domain or leaves it
* **community.vmware.vmware_host_auto_start** : Manage the auto power ON or OFF for vm on ESXi host
* **community.vmware.vmware_host_capability_info** : Gathers info about an ESXi host&#39;s capability information
* **community.vmware.vmware_host_config_info** : Gathers info about an ESXi host&#39;s advance configuration information
* **community.vmware.vmware_host_config_manager** : Manage advanced system settings of an ESXi host
* **community.vmware.vmware_host_custom_attributes** : Manage custom attributes from VMware for the given ESXi host
* **community.vmware.vmware_host_datastore** : Manage a datastore on ESXi host
* **community.vmware.vmware_host_disk_info** : Gathers information about disks attached to given ESXi host/s.
* **community.vmware.vmware_host_dns** : Manage DNS configuration of an ESXi host system
* **community.vmware.vmware_host_dns_info** : Gathers info about an ESXi host&#39;s DNS configuration information
* **community.vmware.vmware_host_facts** : Gathers facts about remote ESXi hostsystem
* **community.vmware.vmware_host_feature_info** : Gathers info about an ESXi host&#39;s feature capability information
* **community.vmware.vmware_host_firewall_info** : Gathers info about an ESXi host&#39;s firewall configuration information
* **community.vmware.vmware_host_firewall_manager** : Manage firewall configurations about an ESXi host
* **community.vmware.vmware_host_hyperthreading** : Enables/Disables Hyperthreading optimization for an ESXi host system
* **community.vmware.vmware_host_ipv6** : Enables/Disables IPv6 support for an ESXi host system
* **community.vmware.vmware_host_iscsi** : Manage the iSCSI configuration of ESXi host
* **community.vmware.vmware_host_iscsi_info** : Gather iSCSI configuration information of ESXi host
* **community.vmware.vmware_host_kernel_manager** : Manage kernel module options on ESXi hosts
* **community.vmware.vmware_host_lockdown** : Manage administrator permission for the local administrative account for the ESXi host
* **community.vmware.vmware_host_lockdown_exceptions** : Manage Lockdown Mode Exception Users
* **community.vmware.vmware_host_logbundle** : Fetch logbundle file from ESXi
* **community.vmware.vmware_host_logbundle_info** : Gathers manifest info for logbundle
* **community.vmware.vmware_host_ntp** : Manage NTP server configuration of an ESXi host
* **community.vmware.vmware_host_ntp_info** : Gathers info about NTP configuration on an ESXi host
* **community.vmware.vmware_host_package_info** : Gathers info about available packages on an ESXi host
* **community.vmware.vmware_host_passthrough** : Manage PCI device passthrough settings on host
* **community.vmware.vmware_host_powermgmt_policy** : Manages the Power Management Policy of an ESXI host system
* **community.vmware.vmware_host_powerstate** : Manages power states of host systems in vCenter
* **community.vmware.vmware_host_scanhba** : Rescan host HBA&#39;s and optionally refresh the storage system
* **community.vmware.vmware_host_scsidisk_info** : Gather information about SCSI disk attached to the given ESXi
* **community.vmware.vmware_host_service_info** : Gathers info about an ESXi host&#39;s services
* **community.vmware.vmware_host_service_manager** : Manage services on a given ESXi host
* **community.vmware.vmware_host_snmp** : Configures SNMP on an ESXi host system
* **community.vmware.vmware_host_sriov** : Manage SR-IOV settings on host
* **community.vmware.vmware_host_ssl_info** : Gather info of ESXi host system about SSL
* **community.vmware.vmware_host_tcpip_stacks** : Manage the TCP/IP Stacks configuration of ESXi host
* **community.vmware.vmware_host_user_manager** : Manage users of ESXi
* **community.vmware.vmware_host_vmhba_info** : Gathers info about vmhbas available on the given ESXi host
* **community.vmware.vmware_host_vmnic_info** : Gathers info about vmnics available on the given ESXi host
* **community.vmware.vmware_local_role_info** : Gather info about local roles on an ESXi host
* **community.vmware.vmware_object_role_permission** : Manage local roles on an ESXi host
* **community.vmware.vmware_local_user_info** : Gather info about users on the given ESXi host
* **community.vmware.vmware_local_user_manager** : Manage local users on an ESXi host
* **community.vmware.vmware_maintenancemode** : Place a host into maintenance mode
* **community.vmware.vmware_migrate_vmk** : Migrate a VMK interface from VSS to VDS
* **community.vmware.vmware_object_custom_attributes_info** : Gather custom attributes of an object
* **community.vmware.vmware_object_rename** : Renames VMware objects
* **community.vmware.vmware_object_role_permission_info** : Gather information about object&#39;s permissions
* **community.vmware.vmware_portgroup** : Create a VMware portgroup
* **community.vmware.vmware_portgroup_info** : Gathers info about an ESXi host&#39;s Port Group configuration
* **community.vmware.vmware_recommended_datastore** : Returns the recommended datastore from a SDRS-enabled datastore cluster
* **community.vmware.vmware_resource_pool** : Add/remove resource pools to/from vCenter
* **community.vmware.vmware_resource_pool_info** : Gathers info about resource pool information
* **community.vmware.vmware_tag** : Manage VMware tags
* **community.vmware.vmware_tag_info** : Manage VMware tag info
* **community.vmware.vmware_tag_manager** : Manage association of VMware tags with VMware objects
* **community.vmware.vmware_target_canonical_info** : Return canonical (NAA) from an ESXi host system
* **community.vmware.vmware_vc_infraprofile_info** : List and Export VMware vCenter infra profile configs.
* **community.vmware.vmware_vcenter_settings** : Configures general settings on a vCenter server
* **community.vmware.vmware_vcenter_settings_info** : Gather info vCenter settings
* **community.vmware.vmware_vcenter_statistics** : Configures statistics on a vCenter server
* **community.vmware.vmware_vm_config_option** : Return supported guest ID list and VM recommended config option for specific guest OS
* **community.vmware.vmware_vm_host_drs_rule** : Creates vm/host group in a given cluster
* **community.vmware.vmware_vm_info** : Return basic info pertaining to a VMware machine guest
* **community.vmware.vmware_vm_shell** : Run commands in a VMware guest operating system
* **community.vmware.vmware_vm_storage_policy** : Create vSphere storage policies
* **community.vmware.vmware_vm_storage_policy_info** : Gather information about vSphere storage profile defined storage policy information.
* **community.vmware.vmware_vm_vm_drs_rule** : Configure VMware DRS Affinity rule for virtual machines in the given cluster
* **community.vmware.vmware_vm_vss_dvs_migrate** : Migrates a virtual machine from a standard vswitch to distributed
* **community.vmware.vmware_vmkernel** : Manages a VMware VMkernel Adapter of an ESXi host.
* **community.vmware.vmware_vmkernel_info** : Gathers VMKernel info about an ESXi host
* **community.vmware.vmware_vmotion** : Move a virtual machine using vMotion, and/or its vmdks using storage vMotion.
* **community.vmware.vmware_vsan_cluster** : Configure VSAN clustering on an ESXi host
* **community.vmware.vmware_vsan_health_info** : Gather information about a VMware vSAN cluster&#39;s health
* **community.vmware.vmware_vspan_session** : Create or remove a Port Mirroring session.
* **community.vmware.vmware_vswitch** : Manage a VMware Standard Switch to an ESXi host.
* **community.vmware.vmware_vswitch_info** : Gathers info about an ESXi host&#39;s vswitch configurations
* **community.vmware.vsphere_copy** : Copy a file to a VMware datastore
* **community.vmware.vsphere_file** : Manage files on a vCenter datastore

## `community.windows` collection

* **community.windows.psexec** : Runs commands on a remote Windows host based on the PsExec model
* **community.windows.win_audit_policy_system** : Used to make changes to the system wide Audit Policy
* **community.windows.win_audit_rule** : Adds an audit rule to files, folders, or registry keys
* **community.windows.win_auto_logon** : Adds or Sets auto logon registry keys.
* **community.windows.win_certificate_info** : Get information on certificates from a Windows Certificate Store
* **community.windows.win_computer_description** : Set windows description, owner and organization
* **community.windows.win_credential** : Manages Windows Credentials in the Credential Manager
* **community.windows.win_data_deduplication** : Module to enable Data Deduplication on a volume.
* **community.windows.win_defrag** : Consolidate fragmented files on local volumes
* **community.windows.win_dhcp_lease** : Manage Windows Server DHCP Leases
* **community.windows.win_disk_facts** : Show the attached disks and disk information of the target host
* **community.windows.win_disk_image** : Manage ISO/VHD/VHDX mounts on Windows hosts
* **community.windows.win_dns_record** : Manage Windows Server DNS records
* **community.windows.win_dns_zone** : Manage Windows Server DNS Zones
* **community.windows.win_domain_computer** : Manage computers in Active Directory
* **community.windows.win_domain_group** : Creates, modifies or removes domain groups
* **community.windows.win_domain_group_membership** : Manage Windows domain group membership
* **community.windows.win_domain_object_info** : Gather information an Active Directory object
* **community.windows.win_domain_ou** : Manage Active Directory Organizational Units
* **community.windows.win_domain_user** : Manages Windows Active Directory user accounts
* **community.windows.win_dotnet_ngen** : Runs ngen to recompile DLLs after .NET  updates
* **community.windows.win_eventlog** : Manage Windows event logs
* **community.windows.win_eventlog_entry** : Write entries to Windows event logs
* **community.windows.win_feature_info** : Gather information about Windows features
* **community.windows.win_file_compression** : Alters the compression of files and directories on NTFS partitions.
* **community.windows.win_file_version** : Get DLL or EXE file build version
* **community.windows.win_firewall** : Enable or disable the Windows Firewall
* **community.windows.win_firewall_rule** : Windows firewall automation
* **community.windows.win_format** : Formats an existing volume or a new volume on an existing partition on Windows
* **community.windows.win_hosts** : Manages hosts file entries on Windows.
* **community.windows.win_hotfix** : Install and uninstalls Windows hotfixes
* **community.windows.win_http_proxy** : Manages proxy settings for WinHTTP
* **community.windows.win_iis_virtualdirectory** : Configures a virtual directory in IIS
* **community.windows.win_iis_webapplication** : Configures IIS web applications
* **community.windows.win_iis_webapppool** : Configure IIS Web Application Pools
* **community.windows.win_iis_webbinding** : Configures a IIS Web site binding
* **community.windows.win_iis_website** : Configures a IIS Web site
* **community.windows.win_inet_proxy** : Manages proxy settings for WinINet and Internet Explorer
* **community.windows.win_initialize_disk** : Initializes disks on Windows Server
* **community.windows.win_lineinfile** : Ensure a particular line is in a file, or replace an existing line using a back-referenced regular expression
* **community.windows.win_listen_ports_facts** : Recopilates the facts of the listening ports of the machine
* **community.windows.win_mapped_drive** : Map network drives for users
* **community.windows.win_msg** : Sends a message to logged in users on Windows hosts
* **community.windows.win_net_adapter_feature** : Enable or disable certain network adapters.
* **community.windows.win_netbios** : Manage NetBIOS over TCP/IP settings on Windows.
* **community.windows.win_nssm** : Install a service using NSSM
* **community.windows.win_pagefile** : Query or change pagefile configuration
* **community.windows.win_partition** : Creates, changes and removes partitions on Windows Server
* **community.windows.win_pester** : Run Pester tests on Windows hosts
* **community.windows.win_power_plan** : Changes the power plan of a Windows system
* **community.windows.win_product_facts** : Provides Windows product and license information
* **community.windows.win_psexec** : Runs commands (remotely) as another (privileged) user
* **community.windows.win_psmodule** : Adds or removes a Windows PowerShell module
* **community.windows.win_psmodule_info** : Gather information about PowerShell Modules
* **community.windows.win_psrepository** : Adds, removes or updates a Windows PowerShell repository.
* **community.windows.win_psrepository_copy** : Copies registered PSRepositories to other user profiles
* **community.windows.win_psrepository_info** : Gather information about PSRepositories
* **community.windows.win_psscript** : Install and manage PowerShell scripts from a PSRepository
* **community.windows.win_psscript_info** : Gather information about installed PowerShell Scripts
* **community.windows.win_pssession_configuration** : Manage PSSession Configurations
* **community.windows.win_rabbitmq_plugin** : Manage RabbitMQ plugins
* **community.windows.win_rds_cap** : Manage Connection Authorization Policies (CAP) on a Remote Desktop Gateway server
* **community.windows.win_rds_rap** : Manage Resource Authorization Policies (RAP) on a Remote Desktop Gateway server
* **community.windows.win_rds_settings** : Manage main settings of a Remote Desktop Gateway server
* **community.windows.win_region** : Set the region and format settings
* **community.windows.win_regmerge** : Merges the contents of a registry file into the Windows registry
* **community.windows.win_robocopy** : Synchronizes the contents of two directories using Robocopy
* **community.windows.win_route** : Add or remove a static route
* **community.windows.win_say** : Text to speech module for Windows to speak messages and optionally play sounds
* **community.windows.win_scheduled_task** : Manage scheduled tasks
* **community.windows.win_scheduled_task_stat** : Get information about Windows Scheduled Tasks
* **community.windows.win_scoop** : Manage packages using Scoop
* **community.windows.win_scoop_bucket** : Manage Scoop buckets
* **community.windows.win_security_policy** : Change local security policy settings
* **community.windows.win_shortcut** : Manage shortcuts on Windows
* **community.windows.win_snmp** : Configures the Windows SNMP service
* **community.windows.win_timezone** : Sets Windows machine timezone
* **community.windows.win_toast** : Sends Toast windows notification to logged in users on Windows 10 or later hosts
* **community.windows.win_unzip** : Unzips compressed files and archives on the Windows node
* **community.windows.win_user_profile** : Manages the Windows user profiles.
* **community.windows.win_wait_for_process** : Waits for a process to exist or not exist before continuing.
* **community.windows.win_wakeonlan** : Send a magic Wake-on-LAN (WoL) broadcast packet
* **community.windows.win_webpicmd** : Installs packages using Web Platform Installer command-line
* **community.windows.win_xml** : Manages XML file content on Windows hosts
* **community.windows.win_zip** : Compress file or directory as zip archive on the Windows node

## `community.zabbix` collection

* **community.zabbix.zabbix_action** : Create/Delete/Update Zabbix actions
* **community.zabbix.zabbix_authentication** : Update Zabbix authentication
* **community.zabbix.zabbix_autoregister** : Update Zabbix autoregistration
* **community.zabbix.zabbix_discovery_rule** : Create/delete/update Zabbix discovery rules
* **community.zabbix.zabbix_globalmacro** : Create/update/delete Zabbix Global macros
* **community.zabbix.zabbix_group** : Create/delete Zabbix host groups
* **community.zabbix.zabbix_group_info** : Gather information about Zabbix hostgroup
* **community.zabbix.zabbix_host** : Create/update/delete Zabbix hosts
* **community.zabbix.zabbix_host_events_info** : Get all triggers about a Zabbix host
* **community.zabbix.zabbix_host_info** : Gather information about Zabbix host
* **community.zabbix.zabbix_hostmacro** : Create/update/delete Zabbix host macros
* **community.zabbix.zabbix_housekeeping** : Update Zabbix housekeeping
* **community.zabbix.zabbix_maintenance** : Create Zabbix maintenance windows
* **community.zabbix.zabbix_map** : Create/update/delete Zabbix maps
* **community.zabbix.zabbix_mediatype** : Create/Update/Delete Zabbix media types
* **community.zabbix.zabbix_proxy** : Create/delete/get/update Zabbix proxies
* **community.zabbix.zabbix_proxy_info** : Gather information about Zabbix proxy
* **community.zabbix.zabbix_screen** : Create/update/delete Zabbix screens
* **community.zabbix.zabbix_script** : Create/update/delete Zabbix scripts
* **community.zabbix.zabbix_service** : Create/update/delete Zabbix service
* **community.zabbix.zabbix_template** : Create/update/delete/dump Zabbix template
* **community.zabbix.zabbix_template_info** : Gather information about Zabbix template
* **community.zabbix.zabbix_user** : Create/update/delete Zabbix users
* **community.zabbix.zabbix_user_directory** : Create/update/delete Zabbix user directories
* **community.zabbix.zabbix_user_info** : Gather information about Zabbix user
* **community.zabbix.zabbix_user_role** : Adds or removes zabbix roles
* **community.zabbix.zabbix_usergroup** : Create/delete/update Zabbix user groups
* **community.zabbix.zabbix_valuemap** : Create/update/delete Zabbix value maps

## `containers.podman` collection

* **containers.podman.podman_container** : Manage podman containers
* **containers.podman.podman_container_info** : Gather facts about containers using podman
* **containers.podman.podman_containers** : Manage podman containers in a batch
* **containers.podman.podman_export** : Export a podman container
* **containers.podman.podman_generate_systemd** : Generate systemd unit from a pod or a container
* **containers.podman.podman_image** : Pull images for use by podman
* **containers.podman.podman_image_info** : Gather info about images using podman
* **containers.podman.podman_import** : Import Podman container from a tar file.
* **containers.podman.podman_load** : Load image from a tar file.
* **containers.podman.podman_login** : Login to a container registry using podman
* **containers.podman.podman_login_info** : Return the logged-in user if any for a given registry
* **containers.podman.podman_logout** : Log out of a container registry using podman
* **containers.podman.podman_network** : Manage podman networks
* **containers.podman.podman_network_info** : Gather info about podman networks
* **containers.podman.podman_play** : Play kubernetes YAML file using podman
* **containers.podman.podman_pod** : Manage Podman pods
* **containers.podman.podman_pod_info** : Gather info about podman pods
* **containers.podman.podman_save** : Saves podman image to tar file
* **containers.podman.podman_secret** : Manage podman secrets
* **containers.podman.podman_tag** : Add an additional name to a local image
* **containers.podman.podman_volume** : Manage Podman volumes
* **containers.podman.podman_volume_info** : Gather info about podman volumes

## `cyberark.pas` collection

* **cyberark.pas.cyberark_account** : Module for CyberArk Account object creation, deletion, and modification using PAS Web Services SDK.
* **cyberark.pas.cyberark_authentication** : CyberArk Authentication using PAS Web Services SDK.
* **cyberark.pas.cyberark_credential** : Credential retrieval using AAM Central Credential Provider.
* **cyberark.pas.cyberark_user** : CyberArk User Management using PAS Web Services SDK.

## `dellemc.enterprise_sonic` collection

* **dellemc.enterprise_sonic.sonic_aaa** : Manage AAA and its parameters
* **dellemc.enterprise_sonic.sonic_api** : Manages REST operations on devices running Enterprise SONiC
* **dellemc.enterprise_sonic.sonic_bgp** : Manage global BGP and its parameters
* **dellemc.enterprise_sonic.sonic_bgp_af** : Manage global BGP address-family and its parameters
* **dellemc.enterprise_sonic.sonic_bgp_as_paths** : Manage BGP autonomous system path (or as-path-list) and its parameters
* **dellemc.enterprise_sonic.sonic_bgp_communities** : Manage BGP community and its parameters
* **dellemc.enterprise_sonic.sonic_bgp_ext_communities** : Manage BGP extended community-list and its parameters
* **dellemc.enterprise_sonic.sonic_bgp_neighbors** : Manage a BGP neighbor and its parameters
* **dellemc.enterprise_sonic.sonic_bgp_neighbors_af** : Manage the BGP neighbor address-family and its parameters
* **dellemc.enterprise_sonic.sonic_command** : Runs commands on devices running Enterprise SONiC
* **dellemc.enterprise_sonic.sonic_config** : Manages configuration sections on devices running Enterprise SONiC
* **dellemc.enterprise_sonic.sonic_facts** : Collects facts on devices running Enterprise SONiC
* **dellemc.enterprise_sonic.sonic_interfaces** : Configure Interface attributes on interfaces such as, Eth, LAG, VLAN, and loopback. (create a loopback interface if it does not exist.)
* **dellemc.enterprise_sonic.sonic_l2_interfaces** : Configure interface-to-VLAN association that is based on access or trunk mode
* **dellemc.enterprise_sonic.sonic_l3_interfaces** : Configure the IPv4 and IPv6 parameters on Interfaces such as, Eth, LAG, VLAN, and loopback
* **dellemc.enterprise_sonic.sonic_lag_interfaces** : Manage link aggregation group (LAG) interface parameters
* **dellemc.enterprise_sonic.sonic_mclag** : Manage multi chassis link aggregation groups domain (MCLAG) and its parameters
* **dellemc.enterprise_sonic.sonic_ntp** : Manage NTP configuration on SONiC.
* **dellemc.enterprise_sonic.sonic_port_breakout** : Configure port breakout settings on physical interfaces
* **dellemc.enterprise_sonic.sonic_prefix_lists** : prefix list configuration handling for SONiC
* **dellemc.enterprise_sonic.sonic_radius_server** : Manage RADIUS server and its parameters
* **dellemc.enterprise_sonic.sonic_static_routes** : Manage static routes configuration on SONiC
* **dellemc.enterprise_sonic.sonic_system** : Configure system parameters
* **dellemc.enterprise_sonic.sonic_tacacs_server** : Manage TACACS server and its parameters
* **dellemc.enterprise_sonic.sonic_users** : Manage users and its parameters
* **dellemc.enterprise_sonic.sonic_vlans** : Manage VLAN and its parameters
* **dellemc.enterprise_sonic.sonic_vrfs** : Manage VRFs and associate VRFs to interfaces such as, Eth, LAG, VLAN, and loopback
* **dellemc.enterprise_sonic.sonic_vxlans** : Manage VxLAN EVPN and its parameters

## `dellemc.openmanage` collection

* **dellemc.openmanage.dellemc_idrac_storage_volume** : Configures the RAID configuration attributes
* **dellemc.openmanage.idrac_attributes** : Configure the iDRAC attributes.
* **dellemc.openmanage.idrac_bios** : Modify and clear BIOS attributes, reset BIOS settings and configure boot sources
* **dellemc.openmanage.idrac_boot** : Configure the boot order settings.
* **dellemc.openmanage.idrac_certificates** : Configure certificates for iDRAC
* **dellemc.openmanage.idrac_firmware** : Firmware update from a repository on a network share (CIFS, NFS, HTTP, HTTPS, FTP)
* **dellemc.openmanage.idrac_firmware_info** : Get Firmware Inventory
* **dellemc.openmanage.idrac_lifecycle_controller_job_status_info** : Get the status of a Lifecycle Controller job
* **dellemc.openmanage.idrac_lifecycle_controller_jobs** : Delete the Lifecycle Controller Jobs
* **dellemc.openmanage.idrac_lifecycle_controller_logs** : Export Lifecycle Controller logs to a network share or local path.
* **dellemc.openmanage.idrac_lifecycle_controller_status_info** : Get the status of the Lifecycle Controller
* **dellemc.openmanage.idrac_os_deployment** : Boot to a network ISO image
* **dellemc.openmanage.idrac_redfish_storage_controller** : Configures the physical disk, virtual disk, and storage controller settings
* **dellemc.openmanage.idrac_reset** : Reset iDRAC
* **dellemc.openmanage.idrac_server_config_profile** : Export or Import iDRAC Server Configuration Profile (SCP)
* **dellemc.openmanage.idrac_syslog** : Enable or disable the syslog on iDRAC
* **dellemc.openmanage.idrac_system_info** : Get the PowerEdge Server System Inventory
* **dellemc.openmanage.idrac_user** : Configure settings for user accounts
* **dellemc.openmanage.idrac_virtual_media** : Configure the Remote File Share settings.
* **dellemc.openmanage.ome_active_directory** : Configure Active Directory groups to be used with Directory Services
* **dellemc.openmanage.ome_application_alerts_smtp** : This module allows to configure SMTP or email configurations
* **dellemc.openmanage.ome_application_alerts_syslog** : Configure syslog forwarding settings on OpenManage Enterprise and OpenManage Enterprise Modular
* **dellemc.openmanage.ome_application_certificate** : This module allows to generate a CSR and upload the certificate
* **dellemc.openmanage.ome_application_console_preferences** : Configure console preferences on OpenManage Enterprise.
* **dellemc.openmanage.ome_application_network_address** : Updates the network configuration on OpenManage Enterprise
* **dellemc.openmanage.ome_application_network_proxy** : Updates the proxy configuration on OpenManage Enterprise
* **dellemc.openmanage.ome_application_network_settings** : This module allows you to configure the session inactivity timeout settings
* **dellemc.openmanage.ome_application_network_time** : Updates the network time on OpenManage Enterprise
* **dellemc.openmanage.ome_application_network_webserver** : Updates the Web server configuration on OpenManage Enterprise
* **dellemc.openmanage.ome_application_security_settings** : Configure the login security properties
* **dellemc.openmanage.ome_chassis_slots** : Rename sled slots on OpenManage Enterprise Modular
* **dellemc.openmanage.ome_configuration_compliance_baseline** : Create, modify, and delete a configuration compliance baseline and remediate non-compliant devices on OpenManage Enterprise
* **dellemc.openmanage.ome_configuration_compliance_info** : Device compliance report for devices managed in OpenManage Enterprise
* **dellemc.openmanage.ome_device_group** : Add or remove device(s) from a static device group on OpenManage Enterprise
* **dellemc.openmanage.ome_device_info** : Retrieves the information of devices inventoried by OpenManage Enterprise
* **dellemc.openmanage.ome_device_local_access_configuration** : Configure local access settings on OpenManage Enterprise Modular.
* **dellemc.openmanage.ome_device_location** : Configure device location settings on OpenManage Enterprise Modular
* **dellemc.openmanage.ome_device_mgmt_network** : Configure network settings of devices on OpenManage Enterprise Modular
* **dellemc.openmanage.ome_device_network_services** : Configure chassis network services settings on OpenManage Enterprise Modular
* **dellemc.openmanage.ome_device_power_settings** : Configure chassis power settings on OpenManage Enterprise Modular
* **dellemc.openmanage.ome_device_quick_deploy** : Configure Quick Deploy settings on OpenManage Enterprise Modular.
* **dellemc.openmanage.ome_devices** : Perform device-specific operations on target devices
* **dellemc.openmanage.ome_diagnostics** : Export technical support logs(TSR) to network share location
* **dellemc.openmanage.ome_discovery** : Create, modify, or delete a discovery job on OpenManage Enterprise
* **dellemc.openmanage.ome_domain_user_groups** : Create, modify, or delete an Active Directory user group on OpenManage Enterprise and OpenManage Enterprise Modular
* **dellemc.openmanage.ome_firmware** : Update firmware on PowerEdge devices and its components through OpenManage Enterprise
* **dellemc.openmanage.ome_firmware_baseline** : Create, modify, or delete a firmware baseline on OpenManage Enterprise or OpenManage Enterprise Modular
* **dellemc.openmanage.ome_firmware_baseline_compliance_info** : Retrieves baseline compliance details on OpenManage Enterprise
* **dellemc.openmanage.ome_firmware_baseline_info** : Retrieves baseline details from OpenManage Enterprise
* **dellemc.openmanage.ome_firmware_catalog** : Create, modify, or delete a firmware catalog on OpenManage Enterprise or OpenManage Enterprise Modular
* **dellemc.openmanage.ome_groups** : Manages static device groups on OpenManage Enterprise
* **dellemc.openmanage.ome_identity_pool** : Manages identity pool settings on OpenManage Enterprise
* **dellemc.openmanage.ome_job_info** : Get job details for a given job ID or an entire job queue on OpenMange Enterprise
* **dellemc.openmanage.ome_network_port_breakout** : This module allows to automate the port portioning or port breakout to logical sub ports
* **dellemc.openmanage.ome_network_vlan** : Create, modify &amp; delete a VLAN
* **dellemc.openmanage.ome_network_vlan_info** : Retrieves the information about networks VLAN(s) present in OpenManage Enterprise
* **dellemc.openmanage.ome_powerstate** : Performs the power management operations on OpenManage Enterprise
* **dellemc.openmanage.ome_profile** : Create, modify, delete, assign, unassign and migrate a profile on OpenManage Enterprise
* **dellemc.openmanage.ome_server_interface_profile_info** : Retrieves the information of server interface profile on OpenManage Enterprise Modular.
* **dellemc.openmanage.ome_server_interface_profiles** : Configure server interface profiles
* **dellemc.openmanage.ome_smart_fabric** : Create, modify or delete a fabric on OpenManage Enterprise Modular
* **dellemc.openmanage.ome_smart_fabric_uplink** : Create, modify or delete a uplink for a fabric on OpenManage Enterprise Modular
* **dellemc.openmanage.ome_template** : Create, modify, deploy, delete, export, import and clone a template on OpenManage Enterprise
* **dellemc.openmanage.ome_template_identity_pool** : Attach or detach an identity pool to a requested template on OpenManage Enterprise
* **dellemc.openmanage.ome_template_info** : Retrieves template details from OpenManage Enterprise
* **dellemc.openmanage.ome_template_network_vlan** : Set tagged and untagged vlans to native network card supported by a template on OpenManage Enterprise
* **dellemc.openmanage.ome_user** : Create, modify or delete a user on OpenManage Enterprise
* **dellemc.openmanage.ome_user_info** : Retrieves details of all accounts or a specific account on OpenManage Enterprise
* **dellemc.openmanage.redfish_event_subscription** : Manage Redfish Subscriptions
* **dellemc.openmanage.redfish_firmware** : To perform a component firmware update using the image file available on the local or remote system
* **dellemc.openmanage.redfish_powerstate** : Manage device power state
* **dellemc.openmanage.redfish_storage_volume** : Manages the storage volume configuration

## `dellemc.os10` collection

* **dellemc.os10.base_xml_to_dict** : Operations for show command output convertion from xml to json format.
* **dellemc.os10.bgp_validate** : Validate the bgp neighbor state,raise error if it is not in established state
* **dellemc.os10.mtu_validate** : Validate the MTU value for lldp neighbors
* **dellemc.os10.os10_command** : Run commands on devices running Dell EMC SmartFabric OS10
* **dellemc.os10.os10_config** : Manage Dell EMC SmartFabric OS10 configuration sections
* **dellemc.os10.os10_facts** : Collect facts from devices running Dell EMC SmartFabric OS10
* **dellemc.os10.show_system_network_summary** : Operations for show_system_network output in json/yaml format.
* **dellemc.os10.vlt_validate** : Validate the vlt info, raise an error if peer is not in up state
* **dellemc.os10.wiring_validate** : Validate the wiring based on the planned wiring details

## `dellemc.os6` collection

* **dellemc.os6.os6_command** : Run commands on devices running Dell EMC OS6
* **dellemc.os6.os6_config** : Manage Dell EMC OS6 configuration sections
* **dellemc.os6.os6_facts** : Collect facts from devices running Dell EMC OS6

## `dellemc.os9` collection

* **dellemc.os9.os9_command** : Run commands on remote devices running Dell OS9
* **dellemc.os9.os9_config** : Manage Dell EMC Networking OS9 configuration sections
* **dellemc.os9.os9_facts** : Collect facts from remote devices running Dell EMC Networking OS9

## `dellemc.powerflex` collection

* **dellemc.powerflex.device** : Manage device on Dell PowerFlex
* **dellemc.powerflex.info** : Gathering information about Dell PowerFlex
* **dellemc.powerflex.mdm_cluster** : Manage MDM cluster on Dell PowerFlex
* **dellemc.powerflex.protection_domain** : Manage Protection Domain on Dell PowerFlex
* **dellemc.powerflex.replication_consistency_group** : Manage replication consistency groups on Dell PowerFlex
* **dellemc.powerflex.sdc** : Manage SDCs on Dell PowerFlex
* **dellemc.powerflex.sds** : Manage SDS on Dell PowerFlex
* **dellemc.powerflex.snapshot** : Manage Snapshots on Dell PowerFlex
* **dellemc.powerflex.storagepool** : Managing Dell PowerFlex storage pool
* **dellemc.powerflex.volume** : Manage volumes on Dell PowerFlex

## `dellemc.unity` collection

* **dellemc.unity.cifsserver** : Manage CIFS server on Unity storage system
* **dellemc.unity.consistencygroup** : Manage consistency groups on Unity storage system
* **dellemc.unity.filesystem** : Manage filesystem on Unity storage system
* **dellemc.unity.filesystem_snapshot** : Manage filesystem snapshot on the Unity storage system
* **dellemc.unity.host** : Manage Host operations on Unity
* **dellemc.unity.info** : Gathering information about Unity
* **dellemc.unity.interface** : Manage Interfaces on Unity storage system
* **dellemc.unity.nasserver** : Manage NAS servers on Unity storage system
* **dellemc.unity.nfs** : Manage NFS export on Unity storage system
* **dellemc.unity.nfsserver** : Manage NFS server on Unity storage system
* **dellemc.unity.smbshare** : Manage SMB shares on Unity storage system
* **dellemc.unity.snapshot** : Manage snapshots on the Unity storage system
* **dellemc.unity.snapshotschedule** : Manage snapshot schedules on Unity storage system
* **dellemc.unity.storagepool** : Manage storage pool on Unity
* **dellemc.unity.tree_quota** : Manage quota tree on the Unity storage system
* **dellemc.unity.user_quota** : Manage user quota on the Unity storage system
* **dellemc.unity.volume** : Manage volume on Unity storage system

## `f5networks.f5_modules` collection

* **f5networks.f5_modules.bigip_apm_acl** : Manage user-defined APM ACLs
* **f5networks.f5_modules.bigip_apm_network_access** : Manage APM Network Access resource
* **f5networks.f5_modules.bigip_apm_policy_fetch** : Exports the APM policy or APM access profile from remote nodes.
* **f5networks.f5_modules.bigip_apm_policy_import** : Manage BIG-IP APM policy or APM access profile imports
* **f5networks.f5_modules.bigip_asm_advanced_settings** : Manage BIG-IP system ASM advanced settings
* **f5networks.f5_modules.bigip_asm_dos_application** : Manage application settings for a DOS profile
* **f5networks.f5_modules.bigip_asm_policy_fetch** : Exports the ASM policy from remote nodes.
* **f5networks.f5_modules.bigip_asm_policy_import** : Manage BIG-IP ASM policy imports
* **f5networks.f5_modules.bigip_asm_policy_manage** : Manage BIG-IP ASM policies
* **f5networks.f5_modules.bigip_asm_policy_server_technology** : Manages Server Technology on an ASM policy
* **f5networks.f5_modules.bigip_asm_policy_signature_set** : Manages Signature Sets on an ASM policy
* **f5networks.f5_modules.bigip_cgnat_lsn_pool** : Manage CGNAT LSN Pools
* **f5networks.f5_modules.bigip_cli_alias** : Manage CLI aliases on a BIG-IP
* **f5networks.f5_modules.bigip_cli_script** : Manage CLI scripts on a BIG-IP
* **f5networks.f5_modules.bigip_command** : Run TMSH and BASH commands on F5 devices
* **f5networks.f5_modules.bigip_config** : Manage BIG-IP configuration sections
* **f5networks.f5_modules.bigip_configsync_action** : Perform different actions related to config-sync
* **f5networks.f5_modules.bigip_data_group** : Manage data groups on a BIG-IP
* **f5networks.f5_modules.bigip_device_auth** : Manage system authentication on a BIG-IP
* **f5networks.f5_modules.bigip_device_auth_ldap** : Manage LDAP device authentication settings on BIG-IP
* **f5networks.f5_modules.bigip_device_auth_radius** : Manages RADIUS auth configuration on a BIG-IP device
* **f5networks.f5_modules.bigip_device_auth_radius_server** : Manages the RADIUS server configuration of the device
* **f5networks.f5_modules.bigip_device_certificate** : Manage self-signed device certificates
* **f5networks.f5_modules.bigip_device_connectivity** : Manages device IP configuration settings for HA on a BIG-IP.
* **f5networks.f5_modules.bigip_device_dns** : Manage DNS settings on a BIG-IP
* **f5networks.f5_modules.bigip_device_group** : Manage device groups on a BIG-IP
* **f5networks.f5_modules.bigip_device_group_member** : Manages members in a device group
* **f5networks.f5_modules.bigip_device_ha_group** : Manage HA group settings on a BIG-IP system
* **f5networks.f5_modules.bigip_device_httpd** : Manage HTTPD related settings on a BIG-IP system
* **f5networks.f5_modules.bigip_device_info** : Collect information from F5 BIG-IP devices
* **f5networks.f5_modules.bigip_device_license** : Manage license installation and activation on BIG-IP devices
* **f5networks.f5_modules.bigip_device_ntp** : Manage NTP servers on a BIG-IP
* **f5networks.f5_modules.bigip_device_sshd** : Manage the SSHD settings of a BIG-IP
* **f5networks.f5_modules.bigip_device_syslog** : Manage system-level syslog settings on BIG-IP
* **f5networks.f5_modules.bigip_device_traffic_group** : Manages traffic groups on BIG-IP
* **f5networks.f5_modules.bigip_device_trust** : Manage the trust relationships between BIG-IPs
* **f5networks.f5_modules.bigip_dns_cache_resolver** : Manage DNS resolver cache configuration on a BIG-IP
* **f5networks.f5_modules.bigip_dns_nameserver** : Manage LTM DNS nameservers on a BIG-IP
* **f5networks.f5_modules.bigip_dns_resolver** : Manage DNS resolvers on a BIG-IP
* **f5networks.f5_modules.bigip_dns_zone** : Manage DNS zones on BIG-IP
* **f5networks.f5_modules.bigip_file_copy** : Manage files in datastores on a BIG-IP
* **f5networks.f5_modules.bigip_firewall_address_list** : Manage address lists on BIG-IP AFM
* **f5networks.f5_modules.bigip_firewall_dos_profile** : Manage AFM DoS profiles on a BIG-IP
* **f5networks.f5_modules.bigip_firewall_dos_vector** : Manage attack vector configuration in an AFM DoS profile
* **f5networks.f5_modules.bigip_firewall_global_rules** : Manage AFM global rule settings on BIG-IP
* **f5networks.f5_modules.bigip_firewall_log_profile** : Manages AFM logging profiles configured in the system
* **f5networks.f5_modules.bigip_firewall_log_profile_network** : Configures Network Firewall related settings of the log profile
* **f5networks.f5_modules.bigip_firewall_rule_list** : Manage AFM security firewall policies on a BIG-IP
* **f5networks.f5_modules.bigip_firewall_port_list** : Manage port lists on BIG-IP AFM
* **f5networks.f5_modules.bigip_firewall_rule** : Manage AFM Firewall rules
* **f5networks.f5_modules.bigip_firewall_schedule** : Manage BIG-IP AFM schedule configurations
* **f5networks.f5_modules.bigip_gtm_datacenter** : Manage Datacenter configuration in BIG-IP
* **f5networks.f5_modules.bigip_gtm_dns_listener** : Configures the BIG-IP DNS system to answer TCP or UDP DNS requests
* **f5networks.f5_modules.bigip_gtm_global** : Manages global GTM settings
* **f5networks.f5_modules.bigip_gtm_monitor_bigip** : Manages F5 BIG-IP GTM BIG-IP monitors
* **f5networks.f5_modules.bigip_gtm_monitor_external** : Manages external GTM monitors on a BIG-IP
* **f5networks.f5_modules.bigip_gtm_monitor_firepass** : Manages F5 BIG-IP GTM FirePass monitors
* **f5networks.f5_modules.bigip_gtm_monitor_http** : Manages F5 BIG-IP GTM HTTP monitors
* **f5networks.f5_modules.bigip_gtm_monitor_https** : Manages F5 BIG-IP GTM HTTPS monitors
* **f5networks.f5_modules.bigip_gtm_monitor_tcp** : Manages F5 BIG-IP GTM TCP monitors
* **f5networks.f5_modules.bigip_gtm_monitor_tcp_half_open** : Manages F5 BIG-IP GTM TCP half-open monitors
* **f5networks.f5_modules.bigip_gtm_pool** : Manages F5 BIG-IP GTM pools
* **f5networks.f5_modules.bigip_gtm_pool_member** : Manage GTM pool member settings
* **f5networks.f5_modules.bigip_gtm_server** : Manages F5 BIG-IP GTM servers
* **f5networks.f5_modules.bigip_gtm_topology_record** : Manages GTM Topology Records
* **f5networks.f5_modules.bigip_gtm_topology_region** : Manages GTM Topology Regions
* **f5networks.f5_modules.bigip_gtm_virtual_server** : Manages F5 BIG-IP GTM virtual servers
* **f5networks.f5_modules.bigip_gtm_wide_ip** : Manages F5 BIG-IP GTM Wide IP
* **f5networks.f5_modules.bigip_hostname** : Manage the hostname of a BIG-IP
* **f5networks.f5_modules.bigip_iapp_service** : Manages TCL iApp services on a BIG-IP
* **f5networks.f5_modules.bigip_iapp_template** : Manages TCL iApp templates on a BIG-IP.
* **f5networks.f5_modules.bigip_ike_peer** : Manage IPSec IKE Peer configuration on BIG-IP
* **f5networks.f5_modules.bigip_imish_config** : Manage BIG-IP advanced routing configuration sections
* **f5networks.f5_modules.bigip_interface** : Module to manage BIG-IP physical interfaces.
* **f5networks.f5_modules.bigip_ipsec_policy** : Manage IPSec policies on a BIG-IP
* **f5networks.f5_modules.bigip_irule** : Manage iRules across different modules on a BIG-IP
* **f5networks.f5_modules.bigip_log_destination** : Manages log destinations on a BIG-IP.
* **f5networks.f5_modules.bigip_log_publisher** : Manages log publishers on a BIG-IP
* **f5networks.f5_modules.bigip_ltm_global** : Manages global LTM settings
* **f5networks.f5_modules.bigip_lx_package** : Manages Javascript LX packages on a BIG-IP
* **f5networks.f5_modules.bigip_management_route** : Manage system management routes on a BIG-IP
* **f5networks.f5_modules.bigip_message_routing_peer** : Manage peers for routing generic message protocol messages
* **f5networks.f5_modules.bigip_message_routing_protocol** : Manage the generic message parser profile.
* **f5networks.f5_modules.bigip_message_routing_route** : Manages static routes for routing message protocol messages
* **f5networks.f5_modules.bigip_message_routing_router** : Manages router profiles for message-routing protocols
* **f5networks.f5_modules.bigip_message_routing_transport_config** : Manages configuration for an outgoing connection
* **f5networks.f5_modules.bigip_monitor_dns** : Manage DNS monitors on a BIG-IP
* **f5networks.f5_modules.bigip_monitor_external** : Manages external LTM monitors on a BIG-IP
* **f5networks.f5_modules.bigip_monitor_ftp** : Manage FTP monitors on a BIG-IP
* **f5networks.f5_modules.bigip_monitor_gateway_icmp** : Manages F5 BIG-IP LTM gateway ICMP monitors
* **f5networks.f5_modules.bigip_monitor_http** : Manages F5 BIG-IP LTM HTTP monitors
* **f5networks.f5_modules.bigip_monitor_https** : Manages F5 BIG-IP LTM HTTPS monitors
* **f5networks.f5_modules.bigip_monitor_icmp** : Manages F5 BIG-IP LTM ICMP monitors
* **f5networks.f5_modules.bigip_monitor_ldap** : Manages BIG-IP LDAP monitors
* **f5networks.f5_modules.bigip_monitor_mysql** : Manages BIG-IP MySQL monitors
* **f5networks.f5_modules.bigip_monitor_oracle** : Manages BIG-IP Oracle monitors
* **f5networks.f5_modules.bigip_monitor_smtp** : Manage SMTP monitors on a BIG-IP
* **f5networks.f5_modules.bigip_monitor_snmp_dca** : Manages BIG-IP SNMP data collecting agent (DCA) monitors
* **f5networks.f5_modules.bigip_monitor_tcp** : Manages F5 BIG-IP LTM TCP monitors
* **f5networks.f5_modules.bigip_monitor_tcp_echo** : Manages F5 BIG-IP LTM TCP echo monitors
* **f5networks.f5_modules.bigip_monitor_tcp_half_open** : Manages F5 BIG-IP LTM TCP half-open monitors
* **f5networks.f5_modules.bigip_monitor_udp** : Manages F5 BIG-IP LTM UDP monitors
* **f5networks.f5_modules.bigip_network_globals** : Manage network global settings on BIG-IP
* **f5networks.f5_modules.bigip_node** : Manages F5 BIG-IP LTM nodes
* **f5networks.f5_modules.bigip_partition** : Manage BIG-IP partitions
* **f5networks.f5_modules.bigip_password_policy** : Manages the authentication password policy on a BIG-IP
* **f5networks.f5_modules.bigip_policy** : Manage general policy configuration on a BIG-IP
* **f5networks.f5_modules.bigip_policy_rule** : Manage LTM policy rules on a BIG-IP
* **f5networks.f5_modules.bigip_pool** : Manages F5 BIG-IP LTM pools
* **f5networks.f5_modules.bigip_pool_member** : Manages F5 BIG-IP LTM pool members
* **f5networks.f5_modules.bigip_profile_analytics** : Manage HTTP analytics profiles on a BIG-IP
* **f5networks.f5_modules.bigip_profile_client_ssl** : Manages client SSL profiles on a BIG-IP
* **f5networks.f5_modules.bigip_profile_dns** : Manage DNS profiles on a BIG-IP
* **f5networks.f5_modules.bigip_profile_fastl4** : Manages Fast L4 profiles
* **f5networks.f5_modules.bigip_profile_ftp** : Manages FTP profiles
* **f5networks.f5_modules.bigip_profile_http** : Manage HTTP profiles on a BIG-IP
* **f5networks.f5_modules.bigip_profile_http2** : Manage HTTP2 profiles on a BIG-IP
* **f5networks.f5_modules.bigip_profile_http_compression** : Manage HTTP compression profiles on a BIG-IP
* **f5networks.f5_modules.bigip_profile_oneconnect** : Manage OneConnect profiles on a BIG-IP
* **f5networks.f5_modules.bigip_profile_persistence_cookie** : Manage cookie persistence profiles on BIG-IP
* **f5networks.f5_modules.bigip_profile_persistence_src_addr** : Manage source address persistence profiles
* **f5networks.f5_modules.bigip_profile_persistence_universal** : Manage universal persistence profiles
* **f5networks.f5_modules.bigip_profile_server_ssl** : Manages server SSL profiles on a BIG-IP
* **f5networks.f5_modules.bigip_profile_sip** : Manage SIP profiles on a BIG-IP
* **f5networks.f5_modules.bigip_profile_tcp** : Manage TCP profiles on a BIG-IP
* **f5networks.f5_modules.bigip_profile_udp** : Manage UDP profiles on a BIG-IP
* **f5networks.f5_modules.bigip_provision** : Manage BIG-IP module provisioning
* **f5networks.f5_modules.bigip_qkview** : Manage QKviews on the device
* **f5networks.f5_modules.bigip_remote_role** : Manage remote roles on a BIG-IP
* **f5networks.f5_modules.bigip_remote_syslog** : Manipulate remote syslog settings on a BIG-IP
* **f5networks.f5_modules.bigip_remote_user** : Manages default settings for remote user accounts on a BIG-IP
* **f5networks.f5_modules.bigip_routedomain** : Manage route domains on a BIG-IP
* **f5networks.f5_modules.bigip_selfip** : Manage Self-IPs on a BIG-IP system
* **f5networks.f5_modules.bigip_service_policy** : Manages service policies on a BIG-IP.
* **f5networks.f5_modules.bigip_smtp** : Manages SMTP settings on the BIG-IP
* **f5networks.f5_modules.bigip_snat_pool** : Manage SNAT pools on a BIG-IP
* **f5networks.f5_modules.bigip_snat_translation** : Manage SNAT translations on a BIG-IP
* **f5networks.f5_modules.bigip_snmp** : Manipulate general SNMP settings on a BIG-IP
* **f5networks.f5_modules.bigip_snmp_community** : Manages SNMP communities on a BIG-IP.
* **f5networks.f5_modules.bigip_snmp_trap** : Manipulate SNMP trap information on a BIG-IP
* **f5networks.f5_modules.bigip_software_image** : Manage software images on a BIG-IP
* **f5networks.f5_modules.bigip_software_install** : Install software images on a BIG-IP
* **f5networks.f5_modules.bigip_software_update** : Manage the software update settings of a BIG-IP
* **f5networks.f5_modules.bigip_ssl_certificate** : Import/Delete certificates from BIG-IP
* **f5networks.f5_modules.bigip_ssl_csr** : Create SSL CSR files on the BIG-IP
* **f5networks.f5_modules.bigip_ssl_key** : Import/Delete SSL keys from BIG-IP
* **f5networks.f5_modules.bigip_ssl_key_cert** : Import/Delete SSL keys and certs from BIG-IP
* **f5networks.f5_modules.bigip_ssl_ocsp** : Manage OCSP configurations on BIG-IP
* **f5networks.f5_modules.bigip_static_route** : Manipulate static routes on a BIG-IP
* **f5networks.f5_modules.bigip_sys_daemon_log_tmm** : Manage BIG-IP tmm daemon log settings
* **f5networks.f5_modules.bigip_sys_db** : Manage BIG-IP system database variables
* **f5networks.f5_modules.bigip_sys_global** : Manage BIG-IP global settings
* **f5networks.f5_modules.bigip_timer_policy** : Manage timer policies on a BIG-IP
* **f5networks.f5_modules.bigip_traffic_selector** : Manage IPSec Traffic Selectors on BIG-IP
* **f5networks.f5_modules.bigip_trunk** : Manage trunks on a BIG-IP
* **f5networks.f5_modules.bigip_tunnel** : Manage tunnels on a BIG-IP
* **f5networks.f5_modules.bigip_ucs** : Manage upload, installation, and removal of UCS files
* **f5networks.f5_modules.bigip_ucs_fetch** : Fetches a UCS file from remote nodes
* **f5networks.f5_modules.bigip_user** : Manage user accounts and user attributes on a BIG-IP
* **f5networks.f5_modules.bigip_vcmp_guest** : Manages vCMP guests on a BIG-IP
* **f5networks.f5_modules.bigip_virtual_address** : Manage LTM virtual addresses on a BIG-IP
* **f5networks.f5_modules.bigip_virtual_server** : Manage LTM virtual servers on a BIG-IP
* **f5networks.f5_modules.bigip_vlan** : Manage VLANs on a BIG-IP system
* **f5networks.f5_modules.bigip_wait** : Wait for a BIG-IP condition before continuing
* **f5networks.f5_modules.bigiq_application_fasthttp** : Manages BIG-IQ FastHTTP applications
* **f5networks.f5_modules.bigiq_application_fastl4_tcp** : Manages BIG-IQ FastL4 TCP applications
* **f5networks.f5_modules.bigiq_application_fastl4_udp** : Manages BIG-IQ FastL4 UDP applications
* **f5networks.f5_modules.bigiq_application_http** : Manages BIG-IQ HTTP applications
* **f5networks.f5_modules.bigiq_application_https_offload** : Manages BIG-IQ HTTPS offload applications
* **f5networks.f5_modules.bigiq_application_https_waf** : Manages BIG-IQ HTTPS WAF applications
* **f5networks.f5_modules.bigiq_device_discovery** : Manage BIG-IP devices through BIG-IQ
* **f5networks.f5_modules.bigiq_device_info** : Collect information from F5 BIG-IQ devices
* **f5networks.f5_modules.bigiq_regkey_license** : Manages licenses in a BIG-IQ registration key pool
* **f5networks.f5_modules.bigiq_regkey_license_assignment** : Manage regkey license assignment on BIG-IPs from a BIG-IQ
* **f5networks.f5_modules.bigiq_regkey_pool** : Manages registration key pools on BIG-IQ
* **f5networks.f5_modules.bigiq_utility_license** : Manage utility licenses on a BIG-IQ
* **f5networks.f5_modules.bigiq_utility_license_assignment** : Manage utility license assignment on BIG-IPs from a BIG-IQ

## `fortinet.fortimanager` collection

* **fortinet.fortimanager.fmgr_wtpprofile_splittunnelingacl** : no description
* **fortinet.fortimanager.fmgr_clone** : Clone an object in FortiManager.
* **fortinet.fortimanager.fmgr_export_playbooks** : Export fortimanager configuration as playbooks.
* **fortinet.fortimanager.fmgr_fact** : Gather fortimanager facts.
* **fortinet.fortimanager.fmgr_generic** : Build and send generic FortiManager API request.
* **fortinet.fortimanager.fmgr_move** : Move fortimanager defined Object.
* **fortinet.fortimanager.fmgr_rename** : Rename an object in FortiManager.

## `fortinet.fortios` collection

* **fortinet.fortios.fortios_alertemail_setting** : Configure alert email settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_antivirus_heuristic** : Configure global heuristic options in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_antivirus_mms_checksum** : Configure MMS content checksum list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_antivirus_notification** : Configure AntiVirus notification lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_antivirus_profile** : Configure AntiVirus profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_antivirus_quarantine** : Configure quarantine options in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_antivirus_settings** : Configure AntiVirus settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_application_custom** : Configure custom application signatures in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_application_group** : Configure firewall application groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_application_list** : Configure application control lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_application_name** : Configure application signatures in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_application_rule_settings** : Configure application rule settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_authentication_rule** : Configure Authentication Rules in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_authentication_scheme** : Configure Authentication Schemes in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_authentication_setting** : Configure authentication setting in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_automation_setting** : Automation setting configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_certificate_ca** : CA certificate in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_certificate_crl** : Certificate Revocation List as a PEM file in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_certificate_local** : Local keys and certificates in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_certificate_remote** : Remote certificate as a PEM file in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_credential_store_domain_controller** : Define known domain controller servers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_cifs_profile** : Configure CIFS profile in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_configuration_fact** : Retrieve Facts of FortiOS Configurable Objects.
* **fortinet.fortios.fortios_dlp_data_type** : Configure predefined data type used by DLP blocking in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dlp_dictionary** : Configure dictionaries used by DLP blocking in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dlp_filepattern** : Configure file patterns used by DLP blocking in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dlp_fp_doc_source** : Create a DLP fingerprint database by allowing the FortiGate to access a file server containing files from which to create fingerprints in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dlp_sensitivity** : Create self-explanatory DLP sensitivity levels to be used when setting sensitivity under config fp-doc-source in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dlp_profile** : Configure DLP profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dlp_sensor** : Configure sensors used by DLP blocking in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dlp_settings** : Designate logical storage for DLP fingerprint database in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dnsfilter_domain_filter** : Configure DNS domain filters in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dnsfilter_profile** : Configure DNS domain filter profile in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dpdk_cpus** : Configure CPUs enabled to run engines in each DPDK stage in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_dpdk_global** : Configure global DPDK options in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_emailfilter_block_allow_list** : Configure anti-spam block/allow list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_spamfilter_bwl** : Configure anti-spam black/white list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_spamfilter_bword** : Configure AntiSpam banned word list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_spamfilter_dnsbl** : Configure AntiSpam DNSBL/ORBL in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_spamfilter_fortishield** : Configure FortiGuard - AntiSpam in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_spamfilter_iptrust** : Configure AntiSpam IP trust in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_spamfilter_mheader** : Configure AntiSpam MIME header in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_spamfilter_options** : Configure AntiSpam options in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_emailfilter_profile** : Configure Email Filter profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_endpoint_control_client** : Configure endpoint control client lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_endpoint_control_forticlient_ems** : Configure FortiClient Enterprise Management Server (EMS) entries in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_endpoint_control_forticlient_registration_sync** : Configure FortiClient registration synchronization settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_endpoint_control_profile** : Configure FortiClient endpoint control profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_endpoint_control_registered_forticlient** : Registered FortiClient list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_endpoint_control_settings** : Configure endpoint control settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_export_config_playbook** : Collect the current configurations of the modules and convert then into playbooks.
* **fortinet.fortios.fortios_extension_controller_dataplan** : FortiExtender dataplan configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_extension_controller_extender** : Extender controller configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_extension_controller_extender_profile** : FortiExtender extender profile configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_extender_extender_info** : Display FortiExtender struct information in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_extender_lte_carrier_by_mcc_mnc** : Display FortiExtender modem carrier based on MCC and MNC in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_extender_lte_carrier_list** : Display FortiExtender modem carrier list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_extender_modem_status** : Display detailed FortiExtender modem status in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_extender_sys_info** : Display detailed FortiExtender system information in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_extension_controller_fortigate** : FortiGate controller configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_extension_controller_fortigate_profile** : FortiGate connector profile configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_file_filter_profile** : Configure file-filter profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_access_proxy** : Configure IPv4 access proxy in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_access_proxy6** : Configure IPv6 access proxy in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_access_proxy_ssh_client_cert** : Configure Access Proxy SSH client certificate in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_access_proxy_virtual_host** : Configure Access Proxy virtual hosts in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_acl** : Configure IPv4 access control list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_acl6** : Configure IPv6 access control list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_address** : Configure IPv4 addresses in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_address6** : Configure IPv6 firewall addresses in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_address6_template** : Configure IPv6 address templates in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_addrgrp** : Configure IPv4 address groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_addrgrp6** : Configure IPv6 address groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_auth_portal** : Configure firewall authentication portals in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_carrier_endpoint_bwl** : Carrier end point black/white list tables in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_central_snat_map** : Configure IPv4 and IPv6 central SNAT policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_city** : Define city table in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_consolidated_policy** : Configure consolidated IPv4/IPv6 policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_country** : Define country table in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_decrypted_traffic_mirror** : Configure decrypted traffic mirror in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_dnstranslation** : Configure DNS translation in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_dos_policy** : Configure IPv4 DoS policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_dos_policy6** : Configure IPv6 DoS policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_global** : Global firewall settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_gtp** : Configure GTP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_identity_based_route** : Configure identity based routing in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_interface_policy** : Configure IPv4 interface policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_interface_policy6** : Configure IPv6 interface policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service** : Show Internet Service application in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_addition** : Configure Internet Services Addition in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_append** : Configure additional port mappings for Internet Services in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_botnet** : Show Internet Service botnet in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_custom** : Configure custom Internet Services in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_custom_group** : Configure custom Internet Service group in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_definition** : Configure Internet Service definition in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_extension** : Configure Internet Services Extension in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_group** : Configure group of Internet Service in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_ipbl_reason** : IP block list reason in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_ipbl_vendor** : IP block list vendor in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_list** : Internet Service list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_name** : Define internet service names in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_owner** : Internet Service owner in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_reputation** : Show Internet Service reputation in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_internet_service_sld** : Internet Service Second Level Domain in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ip_translation** : Configure firewall IP-translation in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ipmacbinding_setting** : Configure IP to MAC binding settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ipmacbinding_table** : Configure IP to MAC address pairs in the IP/MAC binding table in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ippool** : Configure IPv4 IP pools in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ippool6** : Configure IPv6 IP pools in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_iprope_list** : List in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ipv6_eh_filter** : Configure IPv6 extension header filter in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ldb_monitor** : Configure server load balancing health monitors in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_local_in_policy** : Configure user defined IPv4 local-in policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_local_in_policy6** : Configure user defined IPv6 local-in policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_mms_profile** : Configure MMS profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_multicast_address** : Configure multicast addresses in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_multicast_address6** : Configure IPv6 multicast address in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_multicast_policy** : Configure multicast NAT policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_multicast_policy6** : Configure IPv6 multicast NAT policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_network_service_dynamic** : Configure Dynamic Network Services in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_pfcp** : Configure PFCP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_policy** : Configure IPv4/IPv6 policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_policy46** : Configure IPv4 to IPv6 policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_policy6** : Configure IPv6 policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_policy64** : Configure IPv6 to IPv4 policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_profile_group** : Configure profile groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_profile_protocol_options** : Configure protocol options in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_proute** : List policy routing in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_proxy_address** : Configure web proxy address in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_proxy_addrgrp** : Configure web proxy address group in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_proxy_policy** : Configure proxy policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_region** : Define region table in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_schedule_group** : Schedule group configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_schedule_onetime** : Onetime schedule configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_schedule_recurring** : Recurring schedule configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_security_policy** : Configure NGFW IPv4/IPv6 application policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_service_category** : Configure service categories in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_service_custom** : Configure custom services in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_service_group** : Configure service groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_shaper_per_ip_shaper** : Configure per-IP traffic shaper in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_shaper_traffic_shaper** : Configure shared traffic shaper in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_shaping_policy** : Configure shaping policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_shaping_profile** : Configure shaping profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_sniffer** : Configure sniffer in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ssh_host_key** : SSH proxy host public keys in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ssh_local_ca** : SSH proxy local CA in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ssh_local_key** : SSH proxy local keys in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ssh_setting** : SSH proxy settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ssl_server** : Configure SSL servers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ssl_setting** : SSL proxy settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ssl_ssh_profile** : Configure SSL/SSH protocol options in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_traffic_class** : Configure names for shaping classes in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_ttl_policy** : Configure TTL policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_vendor_mac** : Show vendor and the MAC address they have in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_vip** : Configure virtual IP for IPv4 in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_vip46** : Configure IPv4 to IPv6 virtual IPs in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_vip6** : Configure virtual IP for IPv6 in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_vip64** : Configure IPv6 to IPv4 virtual IPs in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_vipgrp** : Configure IPv4 virtual IP groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_vipgrp46** : Configure IPv4 to IPv6 virtual IP groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_vipgrp6** : Configure IPv6 virtual IP groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_vipgrp64** : Configure IPv6 to IPv4 virtual IP groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_wildcard_fqdn_custom** : Config global/VDOM Wildcard FQDN address in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_firewall_wildcard_fqdn_group** : Config global Wildcard FQDN address groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_ftp_proxy_explicit** : Configure explicit FTP proxy settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_gtp_apn** : Configure APN for GTP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_gtp_apn_shaper** : Global per-APN shaper in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_gtp_apngrp** : Configure APN groups for GTP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_gtp_ie_allow_list** : IE allow list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_gtp_ie_white_list** : IE white list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_gtp_message_filter_v0v1** : Message filter for GTPv0/v1 messages in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_gtp_message_filter_v2** : Message filter for GTPv2 messages in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_gtp_rat_timeout_profile** : RAT timeout profil in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_gtp_tunnel_limit** : GTP tunnel limiter in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_hardware_nic** : Display NIC information in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_hardware_npu_np6_dce** : Show NP6 non-zero subengine drop counters in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_hardware_npu_np6_session_stats** : Show NP6 session offloading statistics counters in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_hardware_npu_np6_sse_stats** : Show NP6 hardware session statistics counters in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_icap_profile** : Configure ICAP profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_icap_server** : Configure ICAP servers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_icap_server_group** : Configure an ICAP server group consisting of multiple forward servers. Supports failover and load balancing in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_ips_custom** : Configure IPS custom signature in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_ips_decoder** : Configure IPS decoder in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_ips_global** : Configure IPS global parameter in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_ips_rule** : Configure IPS rules in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_ips_rule_settings** : Configure IPS rule setting in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_ips_sensor** : Configure IPS sensor in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_ips_settings** : Configure IPS VDOM parameter in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_ips_view_map** : Configure IPS view-map in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_json_generic** : Config Fortinet&#39;s FortiOS and FortiGate with json generic method.
* **fortinet.fortios.fortios_log_custom_field** : Configure custom log fields in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_disk_filter** : Configure filters for local disk logging. Use these filters to determine the log messages to record according to severity and type in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_disk_setting** : Settings for local disk logging in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_eventfilter** : Configure log event filters in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fact** : Retrieve log data of fortios log objects.
* **fortinet.fortios.fortios_log_fortianalyzer_filter** : Filters for FortiAnalyzer in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortianalyzer_override_filter** : Override filters for FortiAnalyzer in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortianalyzer_override_setting** : Override FortiAnalyzer settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortianalyzer_setting** : Global FortiAnalyzer settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortianalyzer_cloud_filter** : Filters for FortiAnalyzer Cloud in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortianalyzer_cloud_override_filter** : Override filters for FortiAnalyzer Cloud in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortianalyzer_cloud_override_setting** : Override FortiAnalyzer Cloud settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortianalyzer_cloud_setting** : Global FortiAnalyzer Cloud settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortiguard_filter** : Filters for FortiCloud in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortiguard_override_filter** : Override filters for FortiCloud in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortiguard_override_setting** : Override global FortiCloud logging settings for this VDOM in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_fortiguard_setting** : Configure logging to FortiCloud in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_gui_display** : Configure how log messages are displayed on the GUI in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_memory_filter** : Filters for memory buffer in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_memory_global_setting** : Global settings for memory logging in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_memory_setting** : Settings for memory buffer in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_null_device_filter** : Filters for null device logging in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_null_device_setting** : Settings for null device logging in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_setting** : Configure general log settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_syslogd_filter** : Filters for remote system server in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_syslogd_override_filter** : Override filters for remote system server in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_syslogd_override_setting** : Override settings for remote syslog server in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_syslogd_setting** : Global settings for remote syslog server in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_tacacsplusaccounting_filter** : Settings for TACACS+ accounting events filter in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_tacacsplusaccounting_setting** : Settings for TACACS+ accounting in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_threat_weight** : Configure threat weight settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_webtrends_filter** : Filters for WebTrends in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_log_webtrends_setting** : Settings for WebTrends in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_monitor** : Ansible Module for FortiOS Monitor API
* **fortinet.fortios.fortios_monitor_fact** : Retrieve Facts of FortiOS Monitor Objects.
* **fortinet.fortios.fortios_monitoring_np6_ipsec_engine** : Configure NP6 IPsec engine status monitoring in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_monitoring_npu_hpe** : Configure npu-hpe status monitoring in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_nsxt_service_chain** : Configure NSX-T service chain in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_nsxt_setting** : Configure NSX-T setting in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_pfcp_message_filter** : Message filter for PFCP messages in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_report_chart** : Report chart widget configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_report_dataset** : Report dataset configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_report_layout** : Report layout configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_report_setting** : Report setting configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_report_style** : Report style configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_report_theme** : Report themes configuratio in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_access_list** : Configure access lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_access_list6** : Configure IPv6 access lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_aspath_list** : Configure Autonomous System (AS) path lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_auth_path** : Configure authentication based routing in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_bfd** : Configure BFD in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_bfd6** : Configure IPv6 BFD in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_bgp** : Configure BGP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_community_list** : Configure community lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_isis** : Configure IS-IS in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_key_chain** : Configure key-chain in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_multicast** : Configure router multicast in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_multicast6** : Configure IPv6 multicast in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_multicast_flow** : Configure multicast-flow in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_ospf** : Configure OSPF in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_ospf6** : Configure IPv6 OSPF in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_policy** : Configure IPv4 routing policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_policy6** : Configure IPv6 routing policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_prefix_list** : Configure IPv4 prefix lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_prefix_list6** : Configure IPv6 prefix lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_rip** : Configure RIP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_ripng** : Configure RIPng in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_route_map** : Configure route maps in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_setting** : Configure router settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_static** : Configure IPv4 static routing tables in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_router_static6** : Configure IPv6 static routing tables in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_sctp_filter_profile** : Configure SCTP filter profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_spamfilter_profile** : Configure AntiSpam profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_ssh_filter_profile** : Configure SSH filter profile in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_802_1x_settings** : Configure global 802.1X settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_auto_config_custom** : Policies which can override the &#39;default&#39; for specific ISL/ICL/FortiLink interface in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_auto_config_default** : Policies which are applied automatically to all ISL/ICL/FortiLink interfaces in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_auto_config_policy** : Policy definitions which can define the behavior on auto configured interfaces in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_custom_command** : Configure the FortiGate switch controller to send custom commands to managed FortiSwitch devices in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_dynamic_port_policy** : Configure Dynamic port policy to be applied on the managed FortiSwitch ports through DPP device in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_flow_tracking** : Configure FortiSwitch flow tracking and export via ipfix/netflow in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_fortilink_settings** : Configure integrated FortiLink settings for FortiSwitch in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_global** : Configure FortiSwitch global settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_igmp_snooping** : Configure FortiSwitch IGMP snooping global settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_initial_config_template** : Configure template for auto-generated VLANs in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_initial_config_vlans** : Configure initial template for auto-generated VLAN interfaces in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_lldp_profile** : Configure FortiSwitch LLDP profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_lldp_settings** : Configure FortiSwitch LLDP settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_location** : Configure FortiSwitch location services in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_mac_policy** : Configure MAC policy to be applied on the managed FortiSwitch devices through NAC device in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_mac_sync_settings** : Configure global MAC synchronization settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_managed_switch** : Configure FortiSwitch devices that are managed by this FortiGate in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_nac_device** : Configure/list NAC devices learned on the managed FortiSwitch ports which matches NAC policy in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_nac_settings** : Configure integrated NAC settings for FortiSwitch in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_network_monitor_settings** : Configure network monitor settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_poe** : List PoE end-points status in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_port_policy** : Configure port policy to be applied on the managed FortiSwitch ports through NAC device in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_ptp_policy** : PTP policy configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_ptp_settings** : Global PTP settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_qos_dot1p_map** : Configure FortiSwitch QoS 802.1p in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_qos_ip_dscp_map** : Configure FortiSwitch QoS IP precedence/DSCP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_qos_qos_policy** : Configure FortiSwitch QoS policy in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_qos_queue_policy** : Configure FortiSwitch QoS egress queue policy in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_quarantine** : Configure FortiSwitch quarantine support in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_remote_log** : Configure logging by FortiSwitch device to a remote syslog server in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_security_policy_802_1x** : Configure 802.1x MAC Authentication Bypass (MAB) policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_security_policy_captive_portal** : Names of VLANs that use captive portal authentication in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_security_policy_local_access** : Configure allowaccess list for mgmt and internal interfaces on managed FortiSwitch units in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_sflow** : Configure FortiSwitch sFlow in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_snmp_community** : Configure FortiSwitch SNMP v1/v2c communities globally in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_snmp_sysinfo** : Configure FortiSwitch SNMP system information globally in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_snmp_trap_threshold** : Configure FortiSwitch SNMP trap threshold values globally in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_snmp_user** : Configure FortiSwitch SNMP v3 users globally in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_storm_control** : Configure FortiSwitch storm control in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_storm_control_policy** : Configure FortiSwitch storm control policy to be applied on managed-switch ports in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_stp_instance** : Configure FortiSwitch multiple spanning tree protocol (MSTP) instances in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_stp_settings** : Configure FortiSwitch spanning tree protocol (STP) in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_switch_group** : Configure FortiSwitch switch groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_switch_interface_tag** : Configure switch object tags in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_switch_log** : Configure FortiSwitch logging (logs are transferred to and inserted into FortiGate event log) in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_switch_profile** : Configure FortiSwitch switch profile in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_system** : Configure system-wide switch controller settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_traffic_policy** : Configure FortiSwitch traffic policy in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_traffic_sniffer** : Configure FortiSwitch RSPAN/ERSPAN traffic sniffing parameters in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_virtual_port_pool** : Configure virtual pool in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_vlan** : Configure VLANs for switch controller in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_switch_controller_vlan_policy** : Configure VLAN policy to be applied on the managed FortiSwitch ports through dynamic-port-policy in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_3g_modem_custom** : 3G MODEM custom in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_accprofile** : Configure access profiles for system administrators in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_acme** : Configure ACME client in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_admin** : Configure admin users in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_affinity_interrupt** : Configure interrupt affinity in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_affinity_packet_redistribution** : Configure packet redistribution in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_alarm** : Configure alarm in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_alias** : Configure alias command in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_api_user** : Configure API users in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_arp_table** : Configure ARP table in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_auto_install** : Configure USB auto installation in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_auto_script** : Configure auto script in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_automation_action** : Action for automation stitches in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_automation_destination** : Automation destinations in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_automation_stitch** : Automation stitches in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_automation_trigger** : Trigger for automation stitches in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_autoupdate_push_update** : Configure push updates in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_autoupdate_schedule** : Configure update schedule in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_autoupdate_tunneling** : Configure web proxy tunneling for the FDN in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_central_management** : Configure central management in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_cluster_sync** : Configure FortiGate Session Life Support Protocol (FGSP) session synchronization in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_console** : Configure console in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_csf** : Add this FortiGate to a Security Fabric or set up a new Security Fabric on this FortiGate in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_custom_language** : Configure custom languages in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ddns** : Configure DDNS in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_dedicated_mgmt** : Configure dedicated management in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_dhcp6_server** : Configure DHCPv6 servers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_dhcp_server** : Configure DHCP servers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_dns** : Configure DNS in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_dns64** : Configure DNS64 in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_dns_database** : Configure DNS databases in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_dns_server** : Configure DNS servers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_dscp_based_priority** : Configure DSCP based priority table in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_email_server** : Configure the email server used by the FortiGate various things. For example, for sending email messages to users to support user authentication features in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_external_resource** : Configure external resource in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_federated_upgrade** : Coordinate federated upgrades within the Security Fabric in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_fips_cc** : Configure FIPS-CC mode in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_fm** : Configure FM in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_fortiai** : Configure FortiAI in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_fortiguard** : Configure FortiGuard services in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_fortimanager** : Configure FortiManager in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_fortindr** : Configure FortiNDR in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_fortisandbox** : Configure FortiSandbox in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_fsso_polling** : Configure Fortinet Single Sign On (FSSO) server in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ftm_push** : Configure FortiToken Mobile push services in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_geneve** : Configure GENEVE devices in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_geoip_country** : Define geoip country name-ID table in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_geoip_override** : Configure geographical location mapping for IP address(es) to override mappings from FortiGuard in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_gi_gk** : Configure Gi Firewall Gatekeeper in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_global** : Configure global attributes in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_gre_tunnel** : Configure GRE tunnel in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ha** : Configure HA in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ha_monitor** : Configure HA monitor in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ike** : Configure IKE global attributes in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_interface** : Configure interfaces in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ipam** : Configure IP address management services in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ipip_tunnel** : Configure IP in IP Tunneling in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ips** : Configure IPS system settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ips_urlfilter_dns** : Configure IPS URL filter DNS servers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ips_urlfilter_dns6** : Configure IPS URL filter IPv6 DNS servers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ipsec_aggregate** : Configure an aggregate of IPsec tunnels in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ipv6_neighbor_cache** : Configure IPv6 neighbor cache table in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ipv6_tunnel** : Configure IPv6/IPv4 in IPv6 tunnel in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_isf_queue_profile** : Create a queue profile of switch in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_link_monitor** : Configure Link Health Monitor in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_lldp_network_policy** : Configure LLDP network policy in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_lte_modem** : Configure USB LTE/WIMAX devices in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_mac_address_table** : Configure MAC address tables in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_management_tunnel** : Management tunnel configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_mem_mgr** : Configure memory manager in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_mobile_tunnel** : Configure Mobile tunnels, an implementation of Network Mobility (NEMO) extensions for Mobile IPv4 RFC5177 in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_modem** : Configure MODEM in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_nat64** : Configure NAT64 in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_nd_proxy** : Configure IPv6 neighbor discovery proxy (RFC4389) in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_netflow** : Configure NetFlow in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_network_visibility** : Configure network visibility settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_np6** : Configure NP6 attributes in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_npu** : Configure NPU attributes in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ntp** : Configure system NTP information in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_object_tagging** : Configure object tagging in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_password_policy** : Configure password policy for locally defined administrator passwords and IPsec VPN pre-shared keys in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_password_policy_guest_admin** : Configure the password policy for guest administrators in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_performance_top** : Display information about the top CPU processes in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_physical_switch** : Configure physical switches in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_pppoe_interface** : Configure the PPPoE interfaces in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_probe_response** : Configure system probe response in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_proxy_arp** : Configure proxy-ARP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_ptp** : Configure system PTP information in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_replacemsg_webproxy** : Replacement messages in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_replacemsg_group** : Configure replacement message groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_replacemsg_image** : Configure replacement message images in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_resource_limits** : Configure resource limits in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_saml** : Global settings for SAML authentication in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_sdn_connector** : Configure connection to SDN Connector in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_sdwan** : Configure redundant Internet connections with multiple outbound links and health-check profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_session_helper** : Configure session helper in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_session_ttl** : Configure global session TTL timers for this FortiGate in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_settings** : Configure VDOM settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_sflow** : Configure sFlow in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_sit_tunnel** : Configure IPv6 tunnel over IPv4 in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_smc_ntp** : Configure SMC NTP information in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_sms_server** : Configure SMS server for sending SMS messages to support user authentication in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_snmp_community** : SNMP community configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_snmp_mib_view** : SNMP Access Control MIB View configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_snmp_sysinfo** : SNMP system info configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_snmp_user** : SNMP user configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_speed_test_schedule** : Speed test schedule for each interface in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_speed_test_server** : Configure speed test server list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_sso_admin** : Configure SSO admin users in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_sso_forticloud_admin** : Configure FortiCloud SSO admin users in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_standalone_cluster** : Configure FortiGate Session Life Support Protocol (FGSP) cluster attributes in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_storage** : Configure logical storage in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_stp** : Configure Spanning Tree Protocol (STP) in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_switch_interface** : Configure software switch interfaces by grouping physical and WiFi interfaces in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_tos_based_priority** : Configure Type of Service (ToS) based priority table to set network traffic priorities in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_vdom** : Configure virtual domain in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_vdom_dns** : Configure DNS servers for a non-management VDOM in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_vdom_exception** : Global configuration objects that can be configured independently across different ha peers for all VDOMs or for the defined VDOM scope in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_vdom_link** : Configure VDOM links in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_vdom_netflow** : Configure NetFlow per VDOM in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_vdom_property** : Configure VDOM property in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_vdom_radius_server** : Configure a RADIUS server to use as a RADIUS Single Sign On (RSSO) server for this VDOM in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_vdom_sflow** : Configure sFlow per VDOM to add or change the IP address and UDP port that FortiGate sFlow agents in this VDOM use to send sFlow datagrams to an sFlow collector in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_virtual_switch** : Configure virtual hardware switch interfaces in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_virtual_wan_link** : Configure redundant internet connections using SD-WAN (formerly virtual WAN link) in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_virtual_wire_pair** : Configure virtual wire pairs in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_vne_tunnel** : Configure virtual network enabler tunnel in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_vxlan** : Configure VXLAN devices in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_wccp** : Configure WCCP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_system_zone** : Configure zones to group two or more interfaces. When a zone is created you can configure policies for the zone instead of individual interfaces in the zone in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_adgrp** : Configure FSSO groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_certificate** : Configure certificate users in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_device** : Configure devices in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_device_access_list** : Configure device access control lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_device_category** : Configure device categories in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_device_group** : Configure device groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_domain_controller** : Configure domain controller entries in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_exchange** : Configure MS Exchange server entries in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_fortitoken** : Configure FortiToken in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_fsso** : Configure Fortinet Single Sign On (FSSO) agents in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_fsso_polling** : Configure FSSO active directory servers for polling mode in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_group** : Configure user groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_krb_keytab** : Configure Kerberos keytab entries in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_ldap** : Configure LDAP server entries in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_local** : Configure local users in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_nac_policy** : Configure NAC policy matching pattern to identify matching NAC devices in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_password_policy** : Configure user password policy in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_peer** : Configure peer users in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_peergrp** : Configure peer groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_pop3** : POP3 server entry configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_quarantine** : Configure quarantine support in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_radius** : Configure RADIUS server entries in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_saml** : SAML server entry configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_security_exempt_list** : Configure security exemption list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_setting** : Configure user authentication setting in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_user_tacacsplus** : Configure TACACS+ server entries in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_videofilter_profile** : Configure VideoFilter profile in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_videofilter_youtube_channel_filter** : Configure YouTube channel filter in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_videofilter_youtube_key** : Configure YouTube API keys in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_voip_profile** : Configure VoIP profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_certificate_ocsp_server** : OCSP server configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_certificate_setting** : VPN certificate setting in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ike_gateway** : List gateways in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ipsec_concentrator** : Concentrator configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ipsec_fec** : Configure Forward Error Correction (FEC) mapping profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ipsec_forticlient** : Configure FortiClient policy realm in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ipsec_manualkey_interface** : Configure IPsec manual keys in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ipsec_phase1_interface** : Configure VPN remote gateway in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ipsec_phase2_interface** : Configure VPN autokey tunnel in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_l2tp** : Configure L2TP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ocvpn** : Configure Overlay Controller VPN settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_pptp** : Configure PPTP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ssl_client** : Client in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ssl_settings** : Configure SSL-VPN in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ssl_web_host_check_software** : SSL-VPN host check software in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ssl_web_portal** : Portal in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ssl_web_realm** : Realm in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ssl_web_user_bookmark** : Configure SSL-VPN user bookmark in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_vpn_ssl_web_user_group_bookmark** : Configure SSL-VPN user group bookmark in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_waf_sub_class** : Hidden table for datasource in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_waf_profile** : Configure Web application firewall configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wanopt_auth_group** : Configure WAN optimization authentication groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wanopt_cache_service** : Designate cache-service for wan-optimization and webcache in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wanopt_content_delivery_network_rule** : Configure WAN optimization content delivery network rules in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wanopt_peer** : Configure WAN optimization peers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wanopt_profile** : Configure WAN optimization profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wanopt_remote_storage** : Configure a remote cache device as Web cache storage in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wanopt_settings** : Configure WAN optimization settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wanopt_webcache** : Configure global Web cache settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_web_proxy_debug_url** : Configure debug URL addresses in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_web_proxy_explicit** : Configure explicit Web proxy settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_web_proxy_forward_server** : Configure forward-server addresses in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_web_proxy_forward_server_group** : Configure a forward server group consisting or multiple forward servers. Supports failover and load balancing in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_web_proxy_global** : Configure Web proxy global settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_web_proxy_profile** : Configure web proxy profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_web_proxy_url_match** : Exempt URLs from web proxy forwarding and caching in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_web_proxy_wisp** : Configure Websense Integrated Services Protocol (WISP) servers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_content** : Configure Web filter banned word table in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_content_header** : Configure content types used by Web filter in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_fortiguard** : Configure FortiGuard Web Filter service in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_ftgd_local_cat** : Configure FortiGuard Web Filter local categories in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_ftgd_local_rating** : Configure local FortiGuard Web Filter local ratings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_ips_urlfilter_cache_setting** : Configure IPS URL filter cache settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_ips_urlfilter_setting** : Configure IPS URL filter settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_ips_urlfilter_setting6** : Configure IPS URL filter settings for IPv6 in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_override** : Configure FortiGuard Web Filter administrative overrides in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_profile** : Configure Web filter profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_search_engine** : Configure web filter search engines in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_status** : Display rating info in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_webfilter_urlfilter** : Configure URL filter lists in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_access_control_list** : Configure WiFi bridge access control list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_address** : Configure the client with its MAC address in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_addrgrp** : Configure the MAC address group in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_ap_status** : Configure access point status (rogue | accepted | suppressed) in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_apcfg_profile** : Configure AP local configuration profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_arrp_profile** : Configure WiFi Automatic Radio Resource Provisioning (ARRP) profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_ble_profile** : Configure Bluetooth Low Energy profile in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_bonjour_profile** : Configure Bonjour profiles. Bonjour is Apple&#39;s zero configuration networking protocol. Bonjour profiles allow APs and FortiAPs to connnect to networks using Bonjour in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_client_info** : Wireless controller client-info in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_global** : Configure wireless controller global settings in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_anqp_3gpp_cellular** : Configure 3GPP public land mobile network (PLMN) in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_anqp_ip_address_type** : Configure IP address type availability in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_anqp_nai_realm** : Configure network access identifier (NAI) realm in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_anqp_network_auth_type** : Configure network authentication type in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_anqp_roaming_consortium** : Configure roaming consortium in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_anqp_venue_name** : Configure venue name duple in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_anqp_venue_url** : Configure venue URL in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_h2qp_advice_of_charge** : Configure advice of charge in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_h2qp_conn_capability** : Configure connection capability in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_h2qp_operator_name** : Configure operator friendly name in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_h2qp_osu_provider** : Configure online sign up (OSU) provider list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_h2qp_osu_provider_nai** : Configure online sign up (OSU) provider NAI list in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_h2qp_terms_and_conditions** : Configure terms and conditions in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_h2qp_wan_metric** : Configure WAN metrics in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_hs_profile** : Configure hotspot profile in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_icon** : Configure OSU provider icon in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_hotspot20_qos_map** : Configure QoS map set in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_inter_controller** : Configure inter wireless controller operation in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_log** : Configure wireless controller event log filters in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_mpsk_profile** : Configure MPSK profile in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_nac_profile** : Configure WiFi network access control (NAC) profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_qos_profile** : Configure WiFi quality of service (QoS) profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_region** : Configure FortiAP regions (for floor plans and maps) in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_rf_analysis** : Wireless controller rf-analysis in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_setting** : VDOM wireless controller configuration in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_snmp** : Configure SNMP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_spectral_info** : Wireless controller spectrum analysis in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_ssid_policy** : Configure WiFi SSID policies in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_status** : Wireless controller status in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_syslog_profile** : Configure Wireless Termination Points (WTP) system log server profile in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_timers** : Configure CAPWAP timers in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_utm_profile** : Configure UTM (Unified Threat Management) profile in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_vap** : Configure Virtual Access Points (VAPs) in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_vap_group** : Configure virtual Access Point (VAP) groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_vap_status** : Wireless controller VAP-status in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_wag_profile** : Configure wireless access gateway (WAG) profiles used for tunnels on AP in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_wids_profile** : Configure wireless intrusion detection system (WIDS) profiles in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_wtp** : Configure Wireless Termination Points (WTPs), that is, FortiAPs or APs to be managed by FortiGate in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_wtp_group** : Configure WTP groups in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_wtp_profile** : Configure WTP profiles or FortiAP profiles that define radio settings for manageable FortiAP platforms in Fortinet&#39;s FortiOS and FortiGate.
* **fortinet.fortios.fortios_wireless_controller_wtp_status** : Wireless controller WTP-status in Fortinet&#39;s FortiOS and FortiGate.

## `frr.frr` collection

* **frr.frr.frr_bgp** : Configure global BGP settings on Free Range Routing(FRR).
* **frr.frr.frr_facts** : Collect facts from remote devices running Free Range Routing (FRR).

## `gluster.gluster` collection

* **gluster.gluster.geo_rep** : Manage geo-replication sessions
* **gluster.gluster.gluster_heal_info** : Gather information on self-heal or rebalance status
* **gluster.gluster.gluster_peer** : Attach/Detach peers to/from the cluster
* **gluster.gluster.gluster_volume** : Manage GlusterFS volumes

## `google.cloud` collection

* **google.cloud.gcp_appengine_firewall_rule** : Creates a GCP FirewallRule
* **google.cloud.gcp_appengine_firewall_rule_info** : Gather info for GCP FirewallRule
* **google.cloud.gcp_bigquery_dataset** : Creates a GCP Dataset
* **google.cloud.gcp_bigquery_dataset_info** : Gather info for GCP Dataset
* **google.cloud.gcp_bigquery_table** : Creates a GCP Table
* **google.cloud.gcp_bigquery_table_info** : Gather info for GCP Table
* **google.cloud.gcp_sql_instance** : Creates a GCP Instance
* **google.cloud.gcp_sql_instance_info** : Gather info for GCP Instance
* **google.cloud.gcp_cloudbuild_trigger** : Creates a GCP Trigger
* **google.cloud.gcp_cloudbuild_trigger_info** : Gather info for GCP Trigger
* **google.cloud.gcp_cloudfunctions_cloud_function** : Creates a GCP CloudFunction
* **google.cloud.gcp_cloudfunctions_cloud_function_info** : Gather info for GCP CloudFunction
* **google.cloud.gcp_cloudscheduler_job** : Creates a GCP Job
* **google.cloud.gcp_cloudscheduler_job_info** : Gather info for GCP Job
* **google.cloud.gcp_cloudtasks_queue** : Creates a GCP Queue
* **google.cloud.gcp_cloudtasks_queue_info** : Gather info for GCP Queue
* **google.cloud.gcp_compute_address** : Creates a GCP Address
* **google.cloud.gcp_compute_address_info** : Gather info for GCP Address
* **google.cloud.gcp_compute_autoscaler** : Creates a GCP Autoscaler
* **google.cloud.gcp_compute_autoscaler_info** : Gather info for GCP Autoscaler
* **google.cloud.gcp_compute_backend_bucket** : Creates a GCP BackendBucket
* **google.cloud.gcp_compute_backend_bucket_info** : Gather info for GCP BackendBucket
* **google.cloud.gcp_compute_backend_service** : Creates a GCP BackendService
* **google.cloud.gcp_compute_backend_service_info** : Gather info for GCP BackendService
* **google.cloud.gcp_compute_disk** : Creates a GCP Disk
* **google.cloud.gcp_compute_disk_info** : Gather info for GCP Disk
* **google.cloud.gcp_compute_external_vpn_gateway** : Creates a GCP ExternalVpnGateway
* **google.cloud.gcp_compute_external_vpn_gateway_info** : Gather info for GCP ExternalVpnGateway
* **google.cloud.gcp_compute_firewall** : Creates a GCP Firewall
* **google.cloud.gcp_compute_firewall_info** : Gather info for GCP Firewall
* **google.cloud.gcp_compute_forwarding_rule** : Creates a GCP ForwardingRule
* **google.cloud.gcp_compute_forwarding_rule_info** : Gather info for GCP ForwardingRule
* **google.cloud.gcp_compute_global_address** : Creates a GCP GlobalAddress
* **google.cloud.gcp_compute_global_address_info** : Gather info for GCP GlobalAddress
* **google.cloud.gcp_compute_global_forwarding_rule** : Creates a GCP GlobalForwardingRule
* **google.cloud.gcp_compute_global_forwarding_rule_info** : Gather info for GCP GlobalForwardingRule
* **google.cloud.gcp_compute_health_check** : Creates a GCP HealthCheck
* **google.cloud.gcp_compute_health_check_info** : Gather info for GCP HealthCheck
* **google.cloud.gcp_compute_http_health_check** : Creates a GCP HttpHealthCheck
* **google.cloud.gcp_compute_http_health_check_info** : Gather info for GCP HttpHealthCheck
* **google.cloud.gcp_compute_https_health_check** : Creates a GCP HttpsHealthCheck
* **google.cloud.gcp_compute_https_health_check_info** : Gather info for GCP HttpsHealthCheck
* **google.cloud.gcp_compute_image** : Creates a GCP Image
* **google.cloud.gcp_compute_image_info** : Gather info for GCP Image
* **google.cloud.gcp_compute_instance_group** : Creates a GCP InstanceGroup
* **google.cloud.gcp_compute_instance_group_info** : Gather info for GCP InstanceGroup
* **google.cloud.gcp_compute_instance_group_manager** : Creates a GCP InstanceGroupManager
* **google.cloud.gcp_compute_instance_group_manager_info** : Gather info for GCP InstanceGroupManager
* **google.cloud.gcp_compute_instance_template** : Creates a GCP InstanceTemplate
* **google.cloud.gcp_compute_instance_template_info** : Gather info for GCP InstanceTemplate
* **google.cloud.gcp_compute_interconnect_attachment** : Creates a GCP InterconnectAttachment
* **google.cloud.gcp_compute_interconnect_attachment_info** : Gather info for GCP InterconnectAttachment
* **google.cloud.gcp_compute_network** : Creates a GCP Network
* **google.cloud.gcp_compute_network_endpoint_group** : Creates a GCP NetworkEndpointGroup
* **google.cloud.gcp_compute_network_endpoint_group_info** : Gather info for GCP NetworkEndpointGroup
* **google.cloud.gcp_compute_network_info** : Gather info for GCP Network
* **google.cloud.gcp_compute_node_group** : Creates a GCP NodeGroup
* **google.cloud.gcp_compute_node_group_info** : Gather info for GCP NodeGroup
* **google.cloud.gcp_compute_node_template** : Creates a GCP NodeTemplate
* **google.cloud.gcp_compute_node_template_info** : Gather info for GCP NodeTemplate
* **google.cloud.gcp_compute_region_autoscaler** : Creates a GCP RegionAutoscaler
* **google.cloud.gcp_compute_region_autoscaler_info** : Gather info for GCP RegionAutoscaler
* **google.cloud.gcp_compute_region_backend_service** : Creates a GCP RegionBackendService
* **google.cloud.gcp_compute_region_backend_service_info** : Gather info for GCP RegionBackendService
* **google.cloud.gcp_compute_region_disk** : Creates a GCP RegionDisk
* **google.cloud.gcp_compute_region_disk_info** : Gather info for GCP RegionDisk
* **google.cloud.gcp_compute_region_health_check** : Creates a GCP RegionHealthCheck
* **google.cloud.gcp_compute_region_health_check_info** : Gather info for GCP RegionHealthCheck
* **google.cloud.gcp_compute_region_instance_group_manager** : Creates a GCP RegionInstanceGroupManager
* **google.cloud.gcp_compute_region_instance_group_manager_info** : Gather info for GCP RegionInstanceGroupManager
* **google.cloud.gcp_compute_region_target_http_proxy** : Creates a GCP RegionTargetHttpProxy
* **google.cloud.gcp_compute_region_target_http_proxy_info** : Gather info for GCP RegionTargetHttpProxy
* **google.cloud.gcp_compute_region_target_https_proxy** : Creates a GCP RegionTargetHttpsProxy
* **google.cloud.gcp_compute_region_target_https_proxy_info** : Gather info for GCP RegionTargetHttpsProxy
* **google.cloud.gcp_compute_region_url_map** : Creates a GCP RegionUrlMap
* **google.cloud.gcp_compute_region_url_map_info** : Gather info for GCP RegionUrlMap
* **google.cloud.gcp_compute_reservation** : Creates a GCP Reservation
* **google.cloud.gcp_compute_reservation_info** : Gather info for GCP Reservation
* **google.cloud.gcp_compute_resource_policy** : Creates a GCP ResourcePolicy
* **google.cloud.gcp_compute_resource_policy_info** : Gather info for GCP ResourcePolicy
* **google.cloud.gcp_compute_route** : Creates a GCP Route
* **google.cloud.gcp_compute_route_info** : Gather info for GCP Route
* **google.cloud.gcp_compute_router** : Creates a GCP Router
* **google.cloud.gcp_compute_router_info** : Gather info for GCP Router
* **google.cloud.gcp_compute_snapshot** : Creates a GCP Snapshot
* **google.cloud.gcp_compute_snapshot_info** : Gather info for GCP Snapshot
* **google.cloud.gcp_compute_ssl_certificate** : Creates a GCP SslCertificate
* **google.cloud.gcp_compute_ssl_certificate_info** : Gather info for GCP SslCertificate
* **google.cloud.gcp_compute_ssl_policy** : Creates a GCP SslPolicy
* **google.cloud.gcp_compute_ssl_policy_info** : Gather info for GCP SslPolicy
* **google.cloud.gcp_compute_subnetwork** : Creates a GCP Subnetwork
* **google.cloud.gcp_compute_subnetwork_info** : Gather info for GCP Subnetwork
* **google.cloud.gcp_compute_target_http_proxy** : Creates a GCP TargetHttpProxy
* **google.cloud.gcp_compute_target_http_proxy_info** : Gather info for GCP TargetHttpProxy
* **google.cloud.gcp_compute_target_https_proxy** : Creates a GCP TargetHttpsProxy
* **google.cloud.gcp_compute_target_https_proxy_info** : Gather info for GCP TargetHttpsProxy
* **google.cloud.gcp_compute_target_instance** : Creates a GCP TargetInstance
* **google.cloud.gcp_compute_target_instance_info** : Gather info for GCP TargetInstance
* **google.cloud.gcp_compute_target_pool** : Creates a GCP TargetPool
* **google.cloud.gcp_compute_target_pool_info** : Gather info for GCP TargetPool
* **google.cloud.gcp_compute_target_ssl_proxy** : Creates a GCP TargetSslProxy
* **google.cloud.gcp_compute_target_ssl_proxy_info** : Gather info for GCP TargetSslProxy
* **google.cloud.gcp_compute_target_tcp_proxy** : Creates a GCP TargetTcpProxy
* **google.cloud.gcp_compute_target_tcp_proxy_info** : Gather info for GCP TargetTcpProxy
* **google.cloud.gcp_compute_target_vpn_gateway** : Creates a GCP TargetVpnGateway
* **google.cloud.gcp_compute_target_vpn_gateway_info** : Gather info for GCP TargetVpnGateway
* **google.cloud.gcp_compute_url_map** : Creates a GCP UrlMap
* **google.cloud.gcp_compute_url_map_info** : Gather info for GCP UrlMap
* **google.cloud.gcp_compute_vpn_tunnel** : Creates a GCP VpnTunnel
* **google.cloud.gcp_compute_vpn_tunnel_info** : Gather info for GCP VpnTunnel
* **google.cloud.gcp_container_cluster** : Creates a GCP Cluster
* **google.cloud.gcp_container_cluster_info** : Gather info for GCP Cluster
* **google.cloud.gcp_container_node_pool** : Creates a GCP NodePool
* **google.cloud.gcp_container_node_pool_info** : Gather info for GCP NodePool
* **google.cloud.gcp_dns_managed_zone** : Creates a GCP ManagedZone
* **google.cloud.gcp_dns_managed_zone_info** : Gather info for GCP ManagedZone
* **google.cloud.gcp_dns_resource_record_set** : Creates a GCP ResourceRecordSet
* **google.cloud.gcp_dns_resource_record_set_info** : Gather info for GCP ResourceRecordSet
* **google.cloud.gcp_iam_role** : Creates a GCP Role
* **google.cloud.gcp_iam_role_info** : Gather info for GCP Role
* **google.cloud.gcp_iam_service_account** : Creates a GCP ServiceAccount
* **google.cloud.gcp_iam_service_account_info** : Gather info for GCP ServiceAccount
* **google.cloud.gcp_iam_service_account_key** : Creates a GCP ServiceAccountKey
* **google.cloud.gcp_kms_crypto_key** : Creates a GCP CryptoKey
* **google.cloud.gcp_kms_crypto_key_info** : Gather info for GCP CryptoKey
* **google.cloud.gcp_kms_key_ring** : Creates a GCP KeyRing
* **google.cloud.gcp_kms_key_ring_info** : Gather info for GCP KeyRing
* **google.cloud.gcp_logging_metric** : Creates a GCP Metric
* **google.cloud.gcp_logging_metric_info** : Gather info for GCP Metric
* **google.cloud.gcp_mlengine_model** : Creates a GCP Model
* **google.cloud.gcp_mlengine_model_info** : Gather info for GCP Model
* **google.cloud.gcp_mlengine_version** : Creates a GCP Version
* **google.cloud.gcp_mlengine_version_info** : Gather info for GCP Version
* **google.cloud.gcp_pubsub_subscription** : Creates a GCP Subscription
* **google.cloud.gcp_pubsub_subscription_info** : Gather info for GCP Subscription
* **google.cloud.gcp_pubsub_topic** : Creates a GCP Topic
* **google.cloud.gcp_pubsub_topic_info** : Gather info for GCP Topic
* **google.cloud.gcp_resourcemanager_project** : Creates a GCP Project
* **google.cloud.gcp_resourcemanager_project_info** : Gather info for GCP Project
* **google.cloud.gcp_runtimeconfig_config** : Creates a GCP Config
* **google.cloud.gcp_runtimeconfig_config_info** : Gather info for GCP Config
* **google.cloud.gcp_runtimeconfig_variable** : Creates a GCP Variable
* **google.cloud.gcp_runtimeconfig_variable_info** : Gather info for GCP Variable
* **google.cloud.gcp_serviceusage_service** : Creates a GCP Service
* **google.cloud.gcp_serviceusage_service_info** : Gather info for GCP Service
* **google.cloud.gcp_sourcerepo_repository** : Creates a GCP Repository
* **google.cloud.gcp_sourcerepo_repository_info** : Gather info for GCP Repository
* **google.cloud.gcp_sql_database** : Creates a GCP Database
* **google.cloud.gcp_sql_database_info** : Gather info for GCP Database
* **google.cloud.gcp_sql_ssl_cert** : Creates a GCP SslCert
* **google.cloud.gcp_sql_user** : Creates a GCP User
* **google.cloud.gcp_sql_user_info** : Gather info for GCP User
* **google.cloud.gcp_storage_bucket** : Creates a GCP Bucket
* **google.cloud.gcp_storage_bucket_access_control** : Creates a GCP BucketAccessControl
* **google.cloud.gcp_storage_default_object_acl** : Creates a GCP DefaultObjectACL
* **google.cloud.gcp_storage_object** : Creates a GCP Object
* **google.cloud.gcp_tpu_node** : Creates a GCP Node
* **google.cloud.gcp_tpu_node_info** : Gather info for GCP Node

## `grafana.grafana` collection

* **grafana.grafana.alert_contact_point** : Manage Alerting Contact points in Grafana Cloud
* **grafana.grafana.alert_notification_policy** : Sets the notification policy tree in Alerting on Grafana Cloud
* **grafana.grafana.cloud_api_key** : Manage Grafana Cloud API keys
* **grafana.grafana.cloud_plugin** : Manage Grafana Cloud Plugins
* **grafana.grafana.cloud_stack** : Manage Grafana Cloud stack
* **grafana.grafana.dashboard** : Manage Dashboards in Grafana Cloud
* **grafana.grafana.datasource** : Manage Data sources in Grafana Cloud
* **grafana.grafana.folder** : Manage Folders in Grafana Cloud

## `hetzner.hcloud` collection

* **hetzner.hcloud.hcloud_certificate** : Create and manage certificates on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_certificate_info** : Gather infos about your Hetzner Cloud certificates.
* **hetzner.hcloud.hcloud_datacenter_info** : Gather info about the Hetzner Cloud datacenters.
* **hetzner.hcloud.hcloud_firewall** : Create and manage firewalls on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_floating_ip** : Create and manage cloud Floating IPs on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_floating_ip_info** : Gather infos about the Hetzner Cloud Floating IPs.
* **hetzner.hcloud.hcloud_image_info** : Gather infos about your Hetzner Cloud images.
* **hetzner.hcloud.hcloud_load_balancer** : Create and manage cloud Load Balancers on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_load_balancer_info** : Gather infos about your Hetzner Cloud Load Balancers.
* **hetzner.hcloud.hcloud_load_balancer_network** : Manage the relationship between Hetzner Cloud Networks and Load Balancers
* **hetzner.hcloud.hcloud_load_balancer_service** : Create and manage the services of cloud Load Balancers on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_load_balancer_target** : Manage Hetzner Cloud Load Balancer targets
* **hetzner.hcloud.hcloud_load_balancer_type_info** : Gather infos about the Hetzner Cloud Load Balancer types.
* **hetzner.hcloud.hcloud_location_info** : Gather infos about your Hetzner Cloud locations.
* **hetzner.hcloud.hcloud_network** : Create and manage cloud Networks on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_network_info** : Gather info about your Hetzner Cloud networks.
* **hetzner.hcloud.hcloud_placement_group** : Create and manage placement groups on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_primary_ip** : Create and manage cloud Primary IPs on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_rdns** : Create and manage reverse DNS entries on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_route** : Create and delete cloud routes on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_server** : Create and manage cloud servers on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_server_info** : Gather infos about your Hetzner Cloud servers.
* **hetzner.hcloud.hcloud_server_network** : Manage the relationship between Hetzner Cloud Networks and servers
* **hetzner.hcloud.hcloud_server_type_info** : Gather infos about the Hetzner Cloud server types.
* **hetzner.hcloud.hcloud_ssh_key** : Create and manage ssh keys on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_ssh_key_info** : Gather infos about your Hetzner Cloud ssh_keys.
* **hetzner.hcloud.hcloud_subnetwork** : Manage cloud subnetworks on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_volume** : Create and manage block Volume on the Hetzner Cloud.
* **hetzner.hcloud.hcloud_volume_info** : Gather infos about your Hetzner Cloud Volumes.

## `hpe.nimble` collection

* **hpe.nimble.hpe_nimble_access_control_record** : Manage the HPE Nimble Storage access control records
* **hpe.nimble.hpe_nimble_array** : Manage the HPE Nimble Storage array
* **hpe.nimble.hpe_nimble_chap_user** : Manage the HPE Nimble Storage CHAP user
* **hpe.nimble.hpe_nimble_disk** : Manage the HPE Nimble Storage disk
* **hpe.nimble.hpe_nimble_encryption** : Manage the HPE Nimble Storage encryption
* **hpe.nimble.hpe_nimble_fc** : Manage the HPE Nimble Storage Fibre Channel
* **hpe.nimble.hpe_nimble_group** : Manage the HPE Nimble Storage group
* **hpe.nimble.hpe_nimble_info** : Collect information from HPE Nimble Storage array
* **hpe.nimble.hpe_nimble_initiator_group** : Manage the HPE Nimble Storage initiator groups
* **hpe.nimble.hpe_nimble_network** : Manage the HPE Nimble Storage network configuration
* **hpe.nimble.hpe_nimble_partner** : Manage the HPE Nimble Storage Replication Partner
* **hpe.nimble.hpe_nimble_performance_policy** : Manage the HPE Nimble Storage performance policies
* **hpe.nimble.hpe_nimble_pool** : Manage the HPE Nimble Storage pools
* **hpe.nimble.hpe_nimble_protection_schedule** : Manage the HPE Nimble Storage protection schedules
* **hpe.nimble.hpe_nimble_protection_template** : Manage the HPE Nimble Storage protection templates
* **hpe.nimble.hpe_nimble_shelf** : Manage the HPE Nimble Storage shelves
* **hpe.nimble.hpe_nimble_snapshot** : Manage the HPE Nimble Storage snapshots
* **hpe.nimble.hpe_nimble_snapshot_collection** : Manage the HPE Nimble Storage snapshot collections
* **hpe.nimble.hpe_nimble_user** : Manage the HPE Nimble Storage users
* **hpe.nimble.hpe_nimble_user_policy** : Manage the HPE Nimble Storage user policies
* **hpe.nimble.hpe_nimble_volume** : Manage the HPE Nimble Storage volumes
* **hpe.nimble.hpe_nimble_volume_collection** : Manage the HPE Nimble Storage volume collections

## `ibm.qradar` collection

* **ibm.qradar.deploy** : Trigger a qradar configuration deployment
* **ibm.qradar.offense_action** : Take action on a QRadar Offense
* **ibm.qradar.offense_info** : Obtain information about one or many QRadar Offenses, with filter options
* **ibm.qradar.offense_note** : Create or update a QRadar Offense Note
* **ibm.qradar.qradar_analytics_rules** : Qradar Analytics Rules Management resource module
* **ibm.qradar.qradar_log_sources_management** : Qradar Log Sources Management resource module

## `ibm.spectrum_virtualize` collection

* **ibm.spectrum_virtualize.ibm_sv_manage_awss3_cloudaccount** : This module configures and manages Amazon Simple Storage Service (Amazon S3) cloud account on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_sv_manage_cloud_backups** : This module configures and manages cloud backups on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_sv_manage_ip_partnership** : This module manages IP partnerships on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_sv_manage_provisioning_policy** : This module configures and manages provisioning policies on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_sv_manage_replication_policy** : This module configures and manages replication policies on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_sv_manage_snapshot** : This module manages snapshots (PiT image of a volume) on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_sv_manage_snapshotpolicy** : This module manages snapshot policy configuration on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_sv_manage_ssl_certificate** : This module exports existing system-signed certificate on to IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_sv_manage_truststore_for_replication** : This module manages certificate trust stores for replication on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_sv_restore_cloud_backup** : This module restores the cloud backup on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_sv_switch_replication_direction** : This module switches the replication direction on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_auth** : This module generates an authentication token for a user on IBM Spectrum Virtualize family storage system
* **ibm.spectrum_virtualize.ibm_svc_complete_initial_setup** : This module completes the initial setup configuration for LMC systems
* **ibm.spectrum_virtualize.ibm_svc_host** : This module manages hosts on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_hostcluster** : This module manages host cluster on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_info** : This module gathers various information from the IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_initial_setup** : This module allows users to manage the initial setup configuration on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_callhome** : This module manages Call Home feature configuration on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_consistgrp_flashcopy** : This module manages FlashCopy consistency groups on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_cv** : This module manages the change volume for a given volume on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_flashcopy** : This module manages FlashCopy mappings on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_ip** : This module manages IP provisioning on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_migration** : This module manages volume migration between clusters on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_mirrored_volume** : This module manages mirrored volumes on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_ownershipgroup** : This module manages ownership group on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_portset** : This module manages portset configuration on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_replication** : This module manages remote copies (or rcrelationship) on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_replicationgroup** : This module manages remote copy consistency group on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_safeguarded_policy** : This module manages safeguarded policy configuration on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_sra** : This module manages remote support assistance configuration on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_user** : This module manages user on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_usergroup** : This module manages user group on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_volume** : This module manages standard volumes on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_manage_volumegroup** : This module manages volume groups on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_mdisk** : This module manages MDisks on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_mdiskgrp** : This module manages pools on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_start_stop_flashcopy** : This module starts or stops FlashCopy mapping and consistency groups on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_start_stop_replication** : This module starts or stops remote copies on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svc_vol_map** : This module manages volume mapping on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svcinfo_command** : This module implements SSH Client which helps to run svcinfo CLI command on IBM Spectrum Virtualize family storage systems
* **ibm.spectrum_virtualize.ibm_svctask_command** : This module implements SSH Client which helps to run svctask CLI command(s) on IBM Spectrum Virtualize family storage systems

## `infinidat.infinibox` collection

* **infinidat.infinibox.infini_cluster** : Create, Delete and Modify Host Cluster on Infinibox
* **infinidat.infinibox.infini_export** : Create, Delete or Modify NFS Exports on Infinibox
* **infinidat.infinibox.infini_export_client** : Create, Delete or Modify NFS Client(s) for existing exports on Infinibox
* **infinidat.infinibox.infini_fs** : Create, Delete or Modify filesystems on Infinibox
* **infinidat.infinibox.infini_host** : Create, Delete or Modify Hosts on Infinibox
* **infinidat.infinibox.infini_map** : Create and Delete mapping of a volume to a host or cluster on Infinibox
* **infinidat.infinibox.infini_network_space** : Create, Delete and Modify network spaces on Infinibox
* **infinidat.infinibox.infini_pool** : Create, Delete and Modify Pools on Infinibox
* **infinidat.infinibox.infini_port** : Add and Delete fiber channel and iSCSI ports to a host on Infinibox
* **infinidat.infinibox.infini_user** : Create, Delete and Modify a User on Infinibox
* **infinidat.infinibox.infini_vol** : Create, Delete or Modify volumes on Infinibox

## `infoblox.nios_modules` collection

* **infoblox.nios_modules.nios_a_record** : Configure Infoblox NIOS A records
* **infoblox.nios_modules.nios_aaaa_record** : Configure Infoblox NIOS AAAA records
* **infoblox.nios_modules.nios_cname_record** : Configure Infoblox NIOS CNAME records
* **infoblox.nios_modules.nios_dns_view** : Configure Infoblox NIOS DNS views
* **infoblox.nios_modules.nios_dtc_lbdn** : Configure Infoblox NIOS DTC LBDN
* **infoblox.nios_modules.nios_dtc_pool** : Configure Infoblox NIOS DTC Pool
* **infoblox.nios_modules.nios_dtc_server** : Configure Infoblox NIOS DTC Server
* **infoblox.nios_modules.nios_fixed_address** : Configure Infoblox NIOS DHCP Fixed Address
* **infoblox.nios_modules.nios_host_record** : Configure Infoblox NIOS host records
* **infoblox.nios_modules.nios_member** : Configure Infoblox NIOS members
* **infoblox.nios_modules.nios_mx_record** : Configure Infoblox NIOS MX records
* **infoblox.nios_modules.nios_naptr_record** : Configure Infoblox NIOS NAPTR records
* **infoblox.nios_modules.nios_network** : Configure Infoblox NIOS network object
* **infoblox.nios_modules.nios_network_view** : Configure Infoblox NIOS network views
* **infoblox.nios_modules.nios_nsgroup** : Configure InfoBlox DNS Nameserver Groups
* **infoblox.nios_modules.nios_ptr_record** : Configure Infoblox NIOS PTR records
* **infoblox.nios_modules.nios_restartservices** : Restart grid services.
* **infoblox.nios_modules.nios_srv_record** : Configure Infoblox NIOS SRV records
* **infoblox.nios_modules.nios_txt_record** : Configure Infoblox NIOS txt records
* **infoblox.nios_modules.nios_zone** : Configure Infoblox NIOS DNS zones

## `inspur.ispim` collection

* **inspur.ispim.ad_group** : Manage active directory group information
* **inspur.ispim.ad_group_info** : Get active directory group information
* **inspur.ispim.ad_info** : Get active directory information
* **inspur.ispim.adapter_info** : Get adapter information
* **inspur.ispim.add_ldisk** : Create logical disk
* **inspur.ispim.alert_policy_info** : Get alert policy
* **inspur.ispim.audit_log_info** : Get BMC audit log information
* **inspur.ispim.auto_capture_info** : Get auto capture screen information
* **inspur.ispim.backplane_info** : Get disk backplane information
* **inspur.ispim.backup** : Backup server settings
* **inspur.ispim.bios_export** : Export BIOS config
* **inspur.ispim.bios_import** : Import BIOS config
* **inspur.ispim.bios_info** : Get BIOS setup
* **inspur.ispim.bmc_info** : Get BMC information
* **inspur.ispim.boot_image_info** : Get bmc boot image information
* **inspur.ispim.boot_option_info** : Get BIOS boot options
* **inspur.ispim.clear_audit_log** : Clear BMC audit log
* **inspur.ispim.clear_event_log** : Clear event log
* **inspur.ispim.clear_system_log** : Clear BMC system log
* **inspur.ispim.collect_blackbox** : Collect blackbox log
* **inspur.ispim.collect_log** : Collect logs
* **inspur.ispim.connect_media_info** : Get remote images redirection information
* **inspur.ispim.cpu_info** : Get CPU information
* **inspur.ispim.del_session** : Delete session
* **inspur.ispim.dns_info** : Get dns information
* **inspur.ispim.download_auto_screenshot** : Download auto screenshots
* **inspur.ispim.download_manual_screenshot** : Download manual screenshots
* **inspur.ispim.edit_ad** : Set active directory information
* **inspur.ispim.edit_alert_policy** : Set alert policy
* **inspur.ispim.edit_auto_capture** : Set auto capture screen
* **inspur.ispim.edit_bios** : Set BIOS setup attributes
* **inspur.ispim.edit_boot_image** : Set bmc boot image
* **inspur.ispim.edit_boot_option** : Set BIOS boot options
* **inspur.ispim.edit_connect_media** : Start/Stop virtual media Image
* **inspur.ispim.edit_dns** : Set dns information
* **inspur.ispim.edit_event_log_policy** : Set event log policy
* **inspur.ispim.edit_fan** : Set fan information
* **inspur.ispim.edit_fru** : Set fru settings
* **inspur.ispim.edit_ipv4** : Set ipv4 information
* **inspur.ispim.edit_ipv6** : Set ipv6 information
* **inspur.ispim.edit_kvm** : Set KVM
* **inspur.ispim.edit_ldap** : Set ldap information
* **inspur.ispim.edit_ldisk** : Set logical disk
* **inspur.ispim.edit_m6_log_setting** : Set bmc system and audit log setting
* **inspur.ispim.edit_manual_capture** : Set manual capture screen
* **inspur.ispim.edit_media_instance** : Set Virtual Media Instance
* **inspur.ispim.edit_ncsi** : Set ncsi information
* **inspur.ispim.edit_network** : Set network information
* **inspur.ispim.edit_network_bond** : Set network bond
* **inspur.ispim.edit_network_link** : Set network link
* **inspur.ispim.edit_ntp** : Set NTP
* **inspur.ispim.edit_pdisk** : Set physical disk
* **inspur.ispim.edit_power_budget** : Set power budget information
* **inspur.ispim.edit_power_restore** : Set power restore information
* **inspur.ispim.edit_power_status** : Set power status information
* **inspur.ispim.edit_preserve_config** : Set preserve config
* **inspur.ispim.edit_psu_config** : Set psu config information
* **inspur.ispim.edit_psu_peak** : Set psu peak information
* **inspur.ispim.edit_restore_factory_default** : Set preserver config
* **inspur.ispim.edit_service** : Set service settings
* **inspur.ispim.edit_smtp_dest** : Set SMTP information
* **inspur.ispim.edit_snmp** : Set snmp
* **inspur.ispim.edit_snmp_trap** : Set snmp trap
* **inspur.ispim.edit_threshold** : Set threshold information
* **inspur.ispim.edit_uid** : Set UID
* **inspur.ispim.edit_virtual_media** : Set virtual media
* **inspur.ispim.edit_vlan** : Set vlan information
* **inspur.ispim.event_log_info** : Get event log information
* **inspur.ispim.event_log_policy_info** : Get event log policy information
* **inspur.ispim.fan_info** : Get fan information
* **inspur.ispim.fru_info** : Get fru information
* **inspur.ispim.fw_version_info** : Get firmware version information
* **inspur.ispim.gpu_info** : Get GPU information
* **inspur.ispim.hard_disk_info** : Get hard disk information
* **inspur.ispim.kvm_info** : Get KVM information
* **inspur.ispim.ldap_group** : Manage ldap group information
* **inspur.ispim.ldap_group_info** : Get ldap group information
* **inspur.ispim.ldap_info** : Get ldap information
* **inspur.ispim.ldisk_info** : Get logical disks information
* **inspur.ispim.log_setting_info** : Get bmc log setting information
* **inspur.ispim.media_instance_info** : Get Virtual Media Instance information
* **inspur.ispim.mem_info** : Get memory information
* **inspur.ispim.ncsi_info** : Get ncsi information
* **inspur.ispim.network_bond_info** : Get network bond information
* **inspur.ispim.network_info** : Get network information
* **inspur.ispim.network_link_info** : Get network link information
* **inspur.ispim.ntp_info** : Get NTP information
* **inspur.ispim.onboard_disk_info** : Get onboard disks information
* **inspur.ispim.pcie_info** : Get PCIE information
* **inspur.ispim.pdisk_info** : Get physical disks information
* **inspur.ispim.power_budget_info** : Get power budget information
* **inspur.ispim.power_consumption_info** : Get power consumption information
* **inspur.ispim.power_restore_info** : Get power restore information
* **inspur.ispim.power_status_info** : Get power status information
* **inspur.ispim.preserve_config_info** : Get preserve config information
* **inspur.ispim.psu_config_info** : Get psu config information
* **inspur.ispim.psu_info** : Get psu information
* **inspur.ispim.psu_peak_info** : Get psu peak information
* **inspur.ispim.raid_info** : Get RAID/HBA card and controller information
* **inspur.ispim.reset_bmc** : BMC reset
* **inspur.ispim.reset_kvm** : KVM reset
* **inspur.ispim.restore** : Restore server settings
* **inspur.ispim.self_test_info** : Get self test information
* **inspur.ispim.sensor_info** : Get sensor information
* **inspur.ispim.server_info** : Get server status information
* **inspur.ispim.service_info** : Get service information
* **inspur.ispim.session_info** : Get online session information
* **inspur.ispim.smtp_info** : Get SMTP information
* **inspur.ispim.snmp_info** : Get snmp get/set information
* **inspur.ispim.snmp_trap_info** : Get snmp trap information
* **inspur.ispim.support_info** : Get support information
* **inspur.ispim.system_log_info** : Get BMC system log information
* **inspur.ispim.temp_info** : Get temp information
* **inspur.ispim.threshold_info** : Get threshold information
* **inspur.ispim.uid_info** : Get UID information
* **inspur.ispim.update_cpld** : Update CPLD
* **inspur.ispim.update_fw** : Update firmware
* **inspur.ispim.user** : Manage user
* **inspur.ispim.user_group** : Manage user group
* **inspur.ispim.user_group_info** : Get user group information
* **inspur.ispim.user_info** : Get user information
* **inspur.ispim.virtual_media_info** : Get Virtual Media information
* **inspur.ispim.volt_info** : Get volt information

## `inspur.sm` collection

* **inspur.sm.ad_group** : Manage active directory group information.
* **inspur.sm.ad_group_info** : Get active directory group information.
* **inspur.sm.ad_info** : Get active directory information.
* **inspur.sm.adapter_info** : Get adapter information.
* **inspur.sm.add_ldisk** : Create logical disk.
* **inspur.sm.alert_policy_info** : Get alert policy.
* **inspur.sm.audit_log_info** : Get BMC audit log information.
* **inspur.sm.auto_capture_info** : Get auto capture screen information.
* **inspur.sm.backplane_info** : Get disk backplane information.
* **inspur.sm.backup** : Backup server settings.
* **inspur.sm.bios_export** : Export BIOS config.
* **inspur.sm.bios_import** : Import BIOS config.
* **inspur.sm.bios_info** : Get BIOS setup.
* **inspur.sm.bmc_info** : Get BMC information.
* **inspur.sm.boot_image_info** : Get bmc boot image information.
* **inspur.sm.boot_option_info** : Get BIOS boot options.
* **inspur.sm.clear_audit_log** : Clear BMC audit log.
* **inspur.sm.clear_event_log** : Clear event log.
* **inspur.sm.clear_system_log** : Clear BMC system log.
* **inspur.sm.collect_blackbox** : Collect blackbox log.
* **inspur.sm.collect_log** : Collect logs.
* **inspur.sm.connect_media_info** : Get remote images redirection information.
* **inspur.sm.cpu_info** : Get CPU information.
* **inspur.sm.del_session** : Delete session.
* **inspur.sm.dns_info** : Get dns information.
* **inspur.sm.download_auto_screenshot** : Download auto screenshots.
* **inspur.sm.download_manual_screenshot** : Download manual screenshots.
* **inspur.sm.edit_ad** : Set active directory information.
* **inspur.sm.edit_alert_policy** : Set alert policy.
* **inspur.sm.edit_auto_capture** : Set auto capture screen.
* **inspur.sm.edit_bios** : Set BIOS setup attributes.
* **inspur.sm.edit_boot_image** : Set bmc boot image.
* **inspur.sm.edit_boot_option** : Set BIOS boot options.
* **inspur.sm.edit_connect_media** : Start/Stop virtual media Image
* **inspur.sm.edit_dns** : Set dns information.
* **inspur.sm.edit_event_log_policy** : Set event log policy.
* **inspur.sm.edit_fan** : Set fan information.
* **inspur.sm.edit_fru** : Set fru settings.
* **inspur.sm.edit_ipv4** : Set ipv4 information.
* **inspur.sm.edit_ipv6** : Set ipv6 information.
* **inspur.sm.edit_kvm** : Set KVM.
* **inspur.sm.edit_ldap** : Set ldap information.
* **inspur.sm.edit_ldisk** : Set logical disk.
* **inspur.sm.edit_log_setting** : Set bmc system and audit log setting.
* **inspur.sm.edit_manual_capture** : Set manual capture screen.
* **inspur.sm.edit_media_instance** : Set Virtual Media Instance
* **inspur.sm.edit_ncsi** : Set ncsi information.
* **inspur.sm.edit_network** : Set network information.
* **inspur.sm.edit_network_bond** : Set network bond.
* **inspur.sm.edit_network_link** : Set network link.
* **inspur.sm.edit_ntp** : Set NTP.
* **inspur.sm.edit_pdisk** : Set physical disk.
* **inspur.sm.edit_power_budget** : Set power budget information.
* **inspur.sm.edit_power_restore** : Set power restore information.
* **inspur.sm.edit_power_status** : Set power status information.
* **inspur.sm.edit_preserve_config** : Set preserve config.
* **inspur.sm.edit_psu_config** : Set psu config information.
* **inspur.sm.edit_psu_peak** : Set psu peak information.
* **inspur.sm.edit_restore_factory_default** : Set preserver config.
* **inspur.sm.edit_service** : Set service settings.
* **inspur.sm.edit_smtp_dest** : Set SMTP information.
* **inspur.sm.edit_snmp** : Set snmp.
* **inspur.sm.edit_snmp_trap** : Set snmp trap.
* **inspur.sm.edit_threshold** : Set threshold information.
* **inspur.sm.edit_uid** : Set UID.
* **inspur.sm.edit_virtual_media** : Set virtual media.
* **inspur.sm.edit_vlan** : Set vlan information.
* **inspur.sm.event_log_info** : Get event log information.
* **inspur.sm.event_log_policy_info** : Get event log policy information.
* **inspur.sm.fan_info** : Get fan information.
* **inspur.sm.fru_info** : Get fru information.
* **inspur.sm.fw_version_info** : Get firmware version information.
* **inspur.sm.gpu_info** : Get GPU information.
* **inspur.sm.hard_disk_info** : Get hard disk information.
* **inspur.sm.kvm_info** : Get KVM information.
* **inspur.sm.ldap_group** : Manage ldap group information.
* **inspur.sm.ldap_group_info** : Get ldap group information.
* **inspur.sm.ldap_info** : Get ldap information.
* **inspur.sm.ldisk_info** : Get logical disks information.
* **inspur.sm.log_setting_info** : Get bmc log setting information.
* **inspur.sm.media_instance_info** : Get Virtual Media Instance information.
* **inspur.sm.mem_info** : Get memory information.
* **inspur.sm.ncsi_info** : Get ncsi information.
* **inspur.sm.network_bond_info** : Get network bond information.
* **inspur.sm.network_info** : Get network information.
* **inspur.sm.network_link_info** : Get network link information.
* **inspur.sm.ntp_info** : Get NTP information.
* **inspur.sm.onboard_disk_info** : Get onboard disks information.
* **inspur.sm.pcie_info** : Get PCIE information.
* **inspur.sm.pdisk_info** : Get physical disks information.
* **inspur.sm.power_budget_info** : Get power budget information.
* **inspur.sm.power_consumption_info** : Get power consumption information.
* **inspur.sm.power_restore_info** : Get power restore information.
* **inspur.sm.power_status_info** : Get power status information.
* **inspur.sm.preserve_config_info** : Get preserve config information.
* **inspur.sm.psu_config_info** : Get psu config information.
* **inspur.sm.psu_info** : Get psu information.
* **inspur.sm.psu_peak_info** : Get psu peak information.
* **inspur.sm.raid_info** : Get RAID/HBA card and controller information.
* **inspur.sm.reset_bmc** : BMC reset.
* **inspur.sm.reset_kvm** : KVM reset.
* **inspur.sm.restore** : Restore server settings.
* **inspur.sm.self_test_info** : Get self test information.
* **inspur.sm.sensor_info** : Get sensor information.
* **inspur.sm.server_info** : Get server status information.
* **inspur.sm.service_info** : Get service information.
* **inspur.sm.session_info** : Get online session information.
* **inspur.sm.smtp_info** : Get SMTP information.
* **inspur.sm.snmp_info** : Get snmp get/set information.
* **inspur.sm.snmp_trap_info** : Get snmp trap information.
* **inspur.sm.system_log_info** : Get BMC system log information.
* **inspur.sm.temp_info** : Get temp information.
* **inspur.sm.threshold_info** : Get threshold information.
* **inspur.sm.uid_info** : Get UID information.
* **inspur.sm.update_cpld** : Update CPLD.
* **inspur.sm.update_fw** : Update firmware.
* **inspur.sm.user** : Manage user.
* **inspur.sm.user_group** : Manage user group.
* **inspur.sm.user_group_info** : Get user group information.
* **inspur.sm.user_info** : Get user information.
* **inspur.sm.virtual_media_info** : Get Virtual Media information.
* **inspur.sm.volt_info** : Get volt information.

## `junipernetworks.junos` collection

* **junipernetworks.junos.junos_acl_interfaces** : ACL interfaces resource module
* **junipernetworks.junos.junos_acls** : ACLs resource module
* **junipernetworks.junos.junos_banner** : Manage multiline banners on Juniper JUNOS devices
* **junipernetworks.junos.junos_bgp_address_family** : Manage BGP Address Family attributes of interfaces on Junos devices.
* **junipernetworks.junos.junos_bgp_global** : Manages BGP Global configuration on devices running Juniper JUNOS.
* **junipernetworks.junos.junos_command** : Run arbitrary commands on an Juniper JUNOS device
* **junipernetworks.junos.junos_config** : Manage configuration on devices running Juniper JUNOS
* **junipernetworks.junos.junos_facts** : Collect facts from remote devices running Juniper Junos
* **junipernetworks.junos.junos_hostname** : Manage Hostname server configuration on Junos devices.
* **junipernetworks.junos.junos_interfaces** : Junos Interfaces resource module
* **junipernetworks.junos.junos_l2_interfaces** : L2 interfaces resource module
* **junipernetworks.junos.junos_l3_interfaces** : L3 interfaces resource module
* **junipernetworks.junos.junos_lacp** : Global Link Aggregation Control Protocol (LACP) Junos resource module
* **junipernetworks.junos.junos_lacp_interfaces** : LACP interfaces resource module
* **junipernetworks.junos.junos_lag_interfaces** : Link Aggregation Juniper JUNOS resource module
* **junipernetworks.junos.junos_lldp_global** : LLDP resource module
* **junipernetworks.junos.junos_lldp_interfaces** : LLDP interfaces resource module
* **junipernetworks.junos.junos_logging_global** : Manage logging configuration on Junos devices.
* **junipernetworks.junos.junos_netconf** : Configures the Junos Netconf system service
* **junipernetworks.junos.junos_ntp_global** : Manage NTP configuration on Junos devices.
* **junipernetworks.junos.junos_ospf_interfaces** : OSPF Interfaces Resource Module.
* **junipernetworks.junos.junos_ospfv2** : OSPFv2 resource module
* **junipernetworks.junos.junos_ospfv3** : OSPFv3 resource module
* **junipernetworks.junos.junos_package** : Installs packages on remote devices running Junos
* **junipernetworks.junos.junos_ping** : Tests reachability using ping from devices running Juniper JUNOS
* **junipernetworks.junos.junos_prefix_lists** : Manage prefix-lists attributes of interfaces on Junos devices.
* **junipernetworks.junos.junos_routing_instances** : Manage routing instances on Junos devices.
* **junipernetworks.junos.junos_routing_options** : Manage routing-options configuration on Junos devices.
* **junipernetworks.junos.junos_rpc** : Runs an arbitrary RPC over NetConf on an Juniper JUNOS device
* **junipernetworks.junos.junos_scp** : Transfer files from or to remote devices running Junos
* **junipernetworks.junos.junos_security_policies** : Create and manage security policies on Juniper JUNOS devices
* **junipernetworks.junos.junos_security_policies_global** : Manage global security policy settings on Juniper JUNOS devices
* **junipernetworks.junos.junos_security_zones** : Manage security zones on Juniper JUNOS devices
* **junipernetworks.junos.junos_snmp_server** : Manage SNMP server configuration on Junos devices.
* **junipernetworks.junos.junos_static_routes** : Static routes resource module
* **junipernetworks.junos.junos_system** : Manage the system attributes on Juniper JUNOS devices
* **junipernetworks.junos.junos_user** : Manage local user accounts on Juniper JUNOS devices
* **junipernetworks.junos.junos_vlans** : VLANs resource module
* **junipernetworks.junos.junos_vrf** : Manage the VRF definitions on Juniper JUNOS devices

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

## `lowlydba.sqlserver` collection

* **lowlydba.sqlserver.ag_listener** : Configures an availability group listener
* **lowlydba.sqlserver.ag_replica** : Configures an availability group replica
* **lowlydba.sqlserver.agent_job** : Configures a SQL Agent job
* **lowlydba.sqlserver.agent_job_category** : Configures a SQL Agent job category
* **lowlydba.sqlserver.agent_job_schedule** : Configures a SQL Agent job schedule
* **lowlydba.sqlserver.agent_job_step** : Configures a SQL Agent job step
* **lowlydba.sqlserver.availability_group** : Configures availability group(s)
* **lowlydba.sqlserver.backup** : Performs a backup operation
* **lowlydba.sqlserver.credential** : Configures a credential on a SQL server
* **lowlydba.sqlserver.database** : Creates and configures a database
* **lowlydba.sqlserver.dba_multitool** : Install/update the DBA Multitool suite by John McCall
* **lowlydba.sqlserver.first_responder_kit** : Install/update the First Responder Kit scripts
* **lowlydba.sqlserver.hadr** : Enable or disable HADR
* **lowlydba.sqlserver.install_script** : Runs migration scripts against a database
* **lowlydba.sqlserver.instance_info** : Returns basic information for a SQL Server instance
* **lowlydba.sqlserver.login** : Configures a login for the target SQL Server instance
* **lowlydba.sqlserver.maintenance_solution** : Install/update Maintenance Solution by Ola Hallengren
* **lowlydba.sqlserver.memory** : Sets the maximum memory for a SQL Server instance
* **lowlydba.sqlserver.nonquery** : Executes a generic nonquery
* **lowlydba.sqlserver.resource_governor** : Configures the resource governor on a SQL Server instance
* **lowlydba.sqlserver.restore** : Performs a restore operation
* **lowlydba.sqlserver.rg_resource_pool** : Configures a resource pool for use by the Resource Governor
* **lowlydba.sqlserver.rg_workload_group** : Configures a workload group for use by the Resource Governor
* **lowlydba.sqlserver.sa** : Configure the C(sa) login for security best practices
* **lowlydba.sqlserver.sp_configure** : Make instance level system configuration changes via C(sp_configure)
* **lowlydba.sqlserver.sp_whoisactive** : Install/update C(sp_whoisactive) by Adam Mechanic
* **lowlydba.sqlserver.spn** : Configures SPNs for SQL Server
* **lowlydba.sqlserver.tcp_port** : Sets the TCP port for the instance
* **lowlydba.sqlserver.traceflag** : Enable or disable global trace flags on a SQL Server instance
* **lowlydba.sqlserver.user** : Configures a user within a database

## `mellanox.onyx` collection

* **mellanox.onyx.onyx_aaa** : Configures AAA parameters
* **mellanox.onyx.onyx_bfd** : Configures BFD parameters
* **mellanox.onyx.onyx_bgp** : Configures BGP on Mellanox ONYX network devices
* **mellanox.onyx.onyx_buffer_pool** : Configures Buffer Pool
* **mellanox.onyx.onyx_command** : Run commands on remote devices running Mellanox ONYX
* **mellanox.onyx.onyx_config** : Manage Mellanox ONYX configuration sections
* **mellanox.onyx.onyx_facts** : Collect facts from Mellanox ONYX network devices
* **mellanox.onyx.onyx_igmp** : Configures IGMP global parameters
* **mellanox.onyx.onyx_igmp_interface** : Configures IGMP interface parameters
* **mellanox.onyx.onyx_igmp_vlan** : Configures IGMP Vlan parameters
* **mellanox.onyx.onyx_interface** : Manage Interfaces on Mellanox ONYX network devices
* **mellanox.onyx.onyx_l2_interface** : Manage Layer-2 interface on Mellanox ONYX network devices
* **mellanox.onyx.onyx_l3_interface** : Manage L3 interfaces on Mellanox ONYX network devices
* **mellanox.onyx.onyx_linkagg** : Manage link aggregation groups on Mellanox ONYX network devices
* **mellanox.onyx.onyx_lldp** : Manage LLDP configuration on Mellanox ONYX network devices
* **mellanox.onyx.onyx_lldp_interface** : Manage LLDP interfaces configuration on Mellanox ONYX network devices
* **mellanox.onyx.onyx_magp** : Manage MAGP protocol on Mellanox ONYX network devices
* **mellanox.onyx.onyx_mlag_ipl** : Manage IPL (inter-peer link) on Mellanox ONYX network devices
* **mellanox.onyx.onyx_mlag_vip** : Configures MLAG VIP on Mellanox ONYX network devices
* **mellanox.onyx.onyx_ntp** : Manage NTP general configurations and ntp keys configurations on Mellanox ONYX network devices
* **mellanox.onyx.onyx_ntp_servers_peers** : Configures NTP peers and servers parameters
* **mellanox.onyx.onyx_ospf** : Manage OSPF protocol on Mellanox ONYX network devices
* **mellanox.onyx.onyx_pfc_interface** : Manage priority flow control on ONYX network devices
* **mellanox.onyx.onyx_protocol** : Enables/Disables protocols on Mellanox ONYX network devices
* **mellanox.onyx.onyx_ptp_global** : Configures PTP Global parameters
* **mellanox.onyx.onyx_ptp_interface** : Configures PTP on interface
* **mellanox.onyx.onyx_qos** : Configures QoS
* **mellanox.onyx.onyx_snmp** : Manages SNMP general configurations on Mellanox ONYX network devices
* **mellanox.onyx.onyx_snmp_hosts** : Configures SNMP host parameters
* **mellanox.onyx.onyx_snmp_users** : Configures SNMP User parameters
* **mellanox.onyx.onyx_syslog_files** : Configure file management syslog module
* **mellanox.onyx.onyx_syslog_remote** : Configure remote syslog module
* **mellanox.onyx.onyx_traffic_class** : Configures Traffic Class
* **mellanox.onyx.onyx_username** : Configure username module
* **mellanox.onyx.onyx_vlan** : Manage VLANs on Mellanox ONYX network devices
* **mellanox.onyx.onyx_vxlan** : Configures Vxlan
* **mellanox.onyx.onyx_wjh** : Configure what-just-happend module

## `netapp.aws` collection

* **netapp.aws.aws_netapp_cvs_active_directory** : NetApp AWS CloudVolumes Service Manage Active Directory.
* **netapp.aws.aws_netapp_cvs_filesystems** : NetApp AWS Cloud Volumes Service Manage FileSystem.
* **netapp.aws.aws_netapp_cvs_pool** : NetApp AWS Cloud Volumes Service Manage Pools.
* **netapp.aws.aws_netapp_cvs_snapshots** : NetApp AWS Cloud Volumes Service Manage Snapshots.

## `netapp.azure` collection

* **netapp.azure.azure_rm_netapp_account** : Manage NetApp Azure Files Account
* **netapp.azure.azure_rm_netapp_capacity_pool** : Manage NetApp Azure Files capacity pool
* **netapp.azure.azure_rm_netapp_snapshot** : Manage NetApp Azure Files Snapshot
* **netapp.azure.azure_rm_netapp_volume** : Manage NetApp Azure Files Volume

## `netapp.cloudmanager` collection

* **netapp.cloudmanager.na_cloudmanager_aggregate** : NetApp Cloud Manager Aggregate
* **netapp.cloudmanager.na_cloudmanager_aws_fsx** : Cloud ONTAP file system(FSx) in AWS
* **netapp.cloudmanager.na_cloudmanager_cifs_server** : NetApp Cloud Manager cifs server
* **netapp.cloudmanager.na_cloudmanager_connector_aws** : NetApp Cloud Manager connector for AWS
* **netapp.cloudmanager.na_cloudmanager_connector_azure** : NetApp Cloud Manager connector for Azure.
* **netapp.cloudmanager.na_cloudmanager_connector_gcp** : NetApp Cloud Manager connector for GCP.
* **netapp.cloudmanager.na_cloudmanager_cvo_aws** : NetApp Cloud Manager CVO for AWS
* **netapp.cloudmanager.na_cloudmanager_cvo_azure** : NetApp Cloud Manager CVO/working environment in single or HA mode for Azure.
* **netapp.cloudmanager.na_cloudmanager_cvo_gcp** : NetApp Cloud Manager CVO for GCP
* **netapp.cloudmanager.na_cloudmanager_info** : NetApp Cloud Manager info
* **netapp.cloudmanager.na_cloudmanager_nss_account** : NetApp Cloud Manager nss account
* **netapp.cloudmanager.na_cloudmanager_snapmirror** : NetApp Cloud Manager SnapMirror
* **netapp.cloudmanager.na_cloudmanager_volume** : NetApp Cloud Manager volume

## `netapp.elementsw` collection

* **netapp.elementsw.na_elementsw_access_group** : NetApp Element Software Manage Access Groups
* **netapp.elementsw.na_elementsw_access_group_volumes** : NetApp Element Software Add/Remove Volumes to/from Access Group
* **netapp.elementsw.na_elementsw_account** : NetApp Element Software Manage Accounts
* **netapp.elementsw.na_elementsw_admin_users** : NetApp Element Software Manage Admin Users
* **netapp.elementsw.na_elementsw_backup** : NetApp Element Software Create Backups
* **netapp.elementsw.na_elementsw_check_connections** : NetApp Element Software Check connectivity to MVIP and SVIP.
* **netapp.elementsw.na_elementsw_cluster** : NetApp Element Software Create Cluster
* **netapp.elementsw.na_elementsw_cluster_config** : Configure Element SW Cluster
* **netapp.elementsw.na_elementsw_cluster_pair** : NetApp Element Software Manage Cluster Pair
* **netapp.elementsw.na_elementsw_cluster_snmp** : Configure Element SW Cluster SNMP
* **netapp.elementsw.na_elementsw_drive** : NetApp Element Software Manage Node Drives
* **netapp.elementsw.na_elementsw_info** : NetApp Element Software Info
* **netapp.elementsw.na_elementsw_initiators** : Manage Element SW initiators
* **netapp.elementsw.na_elementsw_ldap** : NetApp Element Software Manage ldap admin users
* **netapp.elementsw.na_elementsw_network_interfaces** : NetApp Element Software Configure Node Network Interfaces
* **netapp.elementsw.na_elementsw_node** : NetApp Element Software Node Operation
* **netapp.elementsw.na_elementsw_qos_policy** : NetApp Element Software create/modify/rename/delete QOS Policy
* **netapp.elementsw.na_elementsw_snapshot** : NetApp Element Software Manage Snapshots
* **netapp.elementsw.na_elementsw_snapshot_restore** : NetApp Element Software Restore Snapshot
* **netapp.elementsw.na_elementsw_snapshot_schedule** : NetApp Element Software Snapshot Schedules
* **netapp.elementsw.na_elementsw_vlan** : NetApp Element Software Manage VLAN
* **netapp.elementsw.na_elementsw_volume** : NetApp Element Software Manage Volumes
* **netapp.elementsw.na_elementsw_volume_clone** : NetApp Element Software Create Volume Clone
* **netapp.elementsw.na_elementsw_volume_pair** : NetApp Element Software Volume Pair

## `netapp.ontap` collection

* **netapp.ontap.na_ontap_active_directory** : NetApp ONTAP configure active directory
* **netapp.ontap.na_ontap_aggregate** : NetApp ONTAP manage aggregates.
* **netapp.ontap.na_ontap_autosupport** : NetApp ONTAP autosupport
* **netapp.ontap.na_ontap_autosupport_invoke** : NetApp ONTAP send AutoSupport message
* **netapp.ontap.na_ontap_bgp_peer_group** : NetApp ONTAP module to create, modify or delete bgp peer group.
* **netapp.ontap.na_ontap_broadcast_domain** : NetApp ONTAP manage broadcast domains.
* **netapp.ontap.na_ontap_broadcast_domain_ports** : NetApp ONTAP manage broadcast domain ports
* **netapp.ontap.na_ontap_cg_snapshot** : NetApp ONTAP manage consistency group snapshot
* **netapp.ontap.na_ontap_cifs** : NetApp ONTAP Manage cifs-share
* **netapp.ontap.na_ontap_cifs_acl** : NetApp ONTAP manage cifs-share-access-control
* **netapp.ontap.na_ontap_cifs_local_group** : NetApp Ontap - create, delete or modify CIFS local group.
* **netapp.ontap.na_ontap_cifs_local_group_member** : NetApp Ontap - Add or remove CIFS local group member
* **netapp.ontap.na_ontap_cifs_local_user** : NetApp ONTAP local CIFS user.
* **netapp.ontap.na_ontap_cifs_local_user_modify** : NetApp ONTAP modify local CIFS user.
* **netapp.ontap.na_ontap_cifs_local_user_set_password** : NetApp ONTAP set local CIFS user password
* **netapp.ontap.na_ontap_cifs_server** : NetApp ONTAP CIFS server configuration
* **netapp.ontap.na_ontap_cluster** : NetApp ONTAP cluster - create a cluster and add/remove nodes.
* **netapp.ontap.na_ontap_cluster_ha** : NetApp ONTAP Manage HA status for cluster
* **netapp.ontap.na_ontap_cluster_peer** : NetApp ONTAP Manage Cluster peering
* **netapp.ontap.na_ontap_command** : NetApp ONTAP Run any cli command, the username provided needs to have console login permission.
* **netapp.ontap.na_ontap_debug** : NetApp ONTAP Debug netapp-lib import and connection.
* **netapp.ontap.na_ontap_disk_options** : NetApp ONTAP modify storage disk options
* **netapp.ontap.na_ontap_disks** : NetApp ONTAP Assign disks to nodes
* **netapp.ontap.na_ontap_dns** : NetApp ONTAP Create, delete, modify DNS servers.
* **netapp.ontap.na_ontap_domain_tunnel** : NetApp ONTAP domain tunnel
* **netapp.ontap.na_ontap_efficiency_policy** : NetApp ONTAP manage efficiency policies (sis policies)
* **netapp.ontap.na_ontap_ems_destination** : NetApp ONTAP configuration for EMS event destination
* **netapp.ontap.na_ontap_export_policy** : NetApp ONTAP manage export-policy
* **netapp.ontap.na_ontap_export_policy_rule** : NetApp ONTAP manage export policy rules
* **netapp.ontap.na_ontap_fcp** : NetApp ONTAP Start, Stop and Enable FCP services.
* **netapp.ontap.na_ontap_fdsd** : NetApp ONTAP create or remove a File Directory security descriptor.
* **netapp.ontap.na_ontap_fdsp** : NetApp ONTAP create or delete a file directory security policy
* **netapp.ontap.na_ontap_fdspt** : NetApp ONTAP create, delete or modify File Directory security policy tasks
* **netapp.ontap.na_ontap_fdss** : NetApp ONTAP File Directory Security Set.
* **netapp.ontap.na_ontap_file_directory_policy** : NetApp ONTAP create, delete, or modify vserver security file-directory policy
* **netapp.ontap.na_ontap_file_security_permissions** : NetApp ONTAP NTFS file security permissions
* **netapp.ontap.na_ontap_file_security_permissions_acl** : NetApp ONTAP file security permissions ACL
* **netapp.ontap.na_ontap_firewall_policy** : NetApp ONTAP Manage a firewall policy
* **netapp.ontap.na_ontap_firmware_upgrade** : NetApp ONTAP firmware upgrade for SP, shelf, ACP, and disk.
* **netapp.ontap.na_ontap_flexcache** : NetApp ONTAP FlexCache - create/delete relationship
* **netapp.ontap.na_ontap_fpolicy_event** : NetApp ONTAP FPolicy policy event configuration
* **netapp.ontap.na_ontap_fpolicy_ext_engine** : NetApp ONTAP fPolicy external engine configuration.
* **netapp.ontap.na_ontap_fpolicy_policy** : NetApp ONTAP - Create, delete or modify an FPolicy policy.
* **netapp.ontap.na_ontap_fpolicy_scope** : NetApp ONTAP - Create, delete or modify an FPolicy policy scope configuration.
* **netapp.ontap.na_ontap_fpolicy_status** : NetApp ONTAP - Enables or disables the specified fPolicy policy
* **netapp.ontap.na_ontap_igroup** : NetApp ONTAP iSCSI or FC igroup configuration
* **netapp.ontap.na_ontap_igroup_initiator** : NetApp ONTAP igroup initiator configuration
* **netapp.ontap.na_ontap_info** : NetApp information gatherer
* **netapp.ontap.na_ontap_interface** : NetApp ONTAP LIF configuration
* **netapp.ontap.na_ontap_ipspace** : NetApp ONTAP Manage an ipspace
* **netapp.ontap.na_ontap_iscsi** : NetApp ONTAP manage iSCSI service
* **netapp.ontap.na_ontap_iscsi_security** : NetApp ONTAP Manage iscsi security.
* **netapp.ontap.na_ontap_job_schedule** : NetApp ONTAP Job Schedule
* **netapp.ontap.na_ontap_kerberos_realm** : NetApp ONTAP vserver nfs kerberos realm
* **netapp.ontap.na_ontap_ldap** : NetApp ONTAP LDAP
* **netapp.ontap.na_ontap_ldap_client** : NetApp ONTAP LDAP client
* **netapp.ontap.na_ontap_license** : NetApp ONTAP protocol and feature license packages
* **netapp.ontap.na_ontap_local_hosts** : NetApp ONTAP local hosts
* **netapp.ontap.na_ontap_log_forward** : NetApp ONTAP Log Forward Configuration
* **netapp.ontap.na_ontap_login_messages** : Setup login banner and message of the day
* **netapp.ontap.na_ontap_lun** : NetApp ONTAP manage LUNs
* **netapp.ontap.na_ontap_lun_copy** : NetApp ONTAP copy LUNs
* **netapp.ontap.na_ontap_lun_map** : NetApp ONTAP LUN maps
* **netapp.ontap.na_ontap_lun_map_reporting_nodes** : NetApp ONTAP LUN maps reporting nodes
* **netapp.ontap.na_ontap_mcc_mediator** : NetApp ONTAP Add and Remove MetroCluster Mediator
* **netapp.ontap.na_ontap_metrocluster** : NetApp ONTAP set up a MetroCluster
* **netapp.ontap.na_ontap_metrocluster_dr_group** : NetApp ONTAP manage MetroCluster DR Group
* **netapp.ontap.na_ontap_motd** : Setup motd
* **netapp.ontap.na_ontap_name_mappings** : NetApp ONTAP name mappings
* **netapp.ontap.na_ontap_name_service_switch** : NetApp ONTAP Manage name service switch
* **netapp.ontap.na_ontap_ndmp** : NetApp ONTAP NDMP services configuration
* **netapp.ontap.na_ontap_net_ifgrp** : NetApp Ontap modify network interface group
* **netapp.ontap.na_ontap_net_port** : NetApp ONTAP network ports.
* **netapp.ontap.na_ontap_net_routes** : NetApp ONTAP network routes
* **netapp.ontap.na_ontap_net_subnet** : NetApp ONTAP Create, delete, modify network subnets.
* **netapp.ontap.na_ontap_net_vlan** : NetApp ONTAP network VLAN
* **netapp.ontap.na_ontap_nfs** : NetApp ONTAP NFS status
* **netapp.ontap.na_ontap_node** : NetApp ONTAP Modify or Rename a node.
* **netapp.ontap.na_ontap_ntfs_dacl** : NetApp Ontap create, delate or modify NTFS DACL (discretionary access control list)
* **netapp.ontap.na_ontap_ntfs_sd** : NetApp ONTAP create, delete or modify NTFS security descriptor
* **netapp.ontap.na_ontap_ntp** : NetApp ONTAP NTP server
* **netapp.ontap.na_ontap_ntp_key** : NetApp ONTAP NTP key
* **netapp.ontap.na_ontap_nvme** : NetApp ONTAP Manage NVMe Service
* **netapp.ontap.na_ontap_nvme_namespace** : NetApp ONTAP Manage NVME Namespace
* **netapp.ontap.na_ontap_nvme_subsystem** : NetApp ONTAP Manage NVME Subsystem
* **netapp.ontap.na_ontap_object_store** : NetApp ONTAP manage object store config.
* **netapp.ontap.na_ontap_partitions** : NetApp ONTAP Assign partitions and disks to nodes.
* **netapp.ontap.na_ontap_ports** : NetApp ONTAP add/remove ports
* **netapp.ontap.na_ontap_portset** : NetApp ONTAP Create/Delete portset
* **netapp.ontap.na_ontap_publickey** : NetApp ONTAP publickey configuration
* **netapp.ontap.na_ontap_qos_adaptive_policy_group** : NetApp ONTAP Adaptive Quality of Service policy group.
* **netapp.ontap.na_ontap_qos_policy_group** : NetApp ONTAP manage policy group in Quality of Service.
* **netapp.ontap.na_ontap_qtree** : NetApp ONTAP manage qtrees
* **netapp.ontap.na_ontap_quota_policy** : NetApp Ontap create, assign, rename or delete quota policy
* **netapp.ontap.na_ontap_quotas** : NetApp ONTAP Quotas
* **netapp.ontap.na_ontap_rest_cli** : NetApp ONTAP run any CLI command using REST api/private/cli/
* **netapp.ontap.na_ontap_rest_info** : NetApp ONTAP information gatherer using REST APIs
* **netapp.ontap.na_ontap_restit** : NetApp ONTAP Run any REST API on ONTAP
* **netapp.ontap.na_ontap_s3_buckets** : NetApp ONTAP S3 Buckets
* **netapp.ontap.na_ontap_s3_groups** : NetApp ONTAP S3 groups
* **netapp.ontap.na_ontap_s3_policies** : NetApp ONTAP S3 Policies
* **netapp.ontap.na_ontap_s3_services** : NetApp ONTAP S3 services
* **netapp.ontap.na_ontap_s3_users** : NetApp ONTAP S3 users
* **netapp.ontap.na_ontap_security_certificates** : NetApp ONTAP manage security certificates.
* **netapp.ontap.na_ontap_security_config** : NetApp ONTAP modify security config for SSL.
* **netapp.ontap.na_ontap_security_ipsec_ca_certificate** : NetApp ONTAP module to add or delete ipsec ca certificate.
* **netapp.ontap.na_ontap_security_ipsec_config** : NetApp ONTAP module to configure IPsec config.
* **netapp.ontap.na_ontap_security_ipsec_policy** : NetApp ONTAP module to create, modify or delete security IPsec policy.
* **netapp.ontap.na_ontap_security_key_manager** : NetApp ONTAP security key manager.
* **netapp.ontap.na_ontap_security_ssh** : NetApp ONTAP security ssh
* **netapp.ontap.na_ontap_service_policy** : NetApp ONTAP service policy configuration
* **netapp.ontap.na_ontap_service_processor_network** : NetApp ONTAP service processor network
* **netapp.ontap.na_ontap_snaplock_clock** : NetApp ONTAP Sets the snaplock compliance clock.
* **netapp.ontap.na_ontap_snapmirror** : NetApp ONTAP or ElementSW Manage SnapMirror
* **netapp.ontap.na_ontap_snapmirror_policy** : NetApp ONTAP create, delete or modify SnapMirror policies
* **netapp.ontap.na_ontap_snapshot** : NetApp ONTAP manage Snapshots
* **netapp.ontap.na_ontap_snapshot_policy** : NetApp ONTAP manage Snapshot Policy
* **netapp.ontap.na_ontap_snmp** : NetApp ONTAP SNMP community
* **netapp.ontap.na_ontap_snmp_traphosts** : NetApp ONTAP SNMP traphosts.
* **netapp.ontap.na_ontap_software_update** : NetApp ONTAP Update Software
* **netapp.ontap.na_ontap_ssh_command** : NetApp ONTAP Run any cli command over plain SSH using paramiko.
* **netapp.ontap.na_ontap_storage_auto_giveback** : Enables or disables NetApp ONTAP storage auto giveback for a specified node
* **netapp.ontap.na_ontap_storage_failover** : Enables or disables NetApp Ontap storage failover for a specified node
* **netapp.ontap.na_ontap_svm** : NetApp ONTAP SVM
* **netapp.ontap.na_ontap_svm_options** : NetApp ONTAP Modify SVM Options
* **netapp.ontap.na_ontap_ucadapter** : NetApp ONTAP UC adapter configuration
* **netapp.ontap.na_ontap_unix_group** : NetApp ONTAP UNIX Group
* **netapp.ontap.na_ontap_unix_user** : NetApp ONTAP UNIX users
* **netapp.ontap.na_ontap_user** : NetApp ONTAP user configuration and management
* **netapp.ontap.na_ontap_user_role** : NetApp ONTAP user role configuration and management
* **netapp.ontap.na_ontap_volume** : NetApp ONTAP manage volumes.
* **netapp.ontap.na_ontap_volume_autosize** : NetApp ONTAP manage volume autosize
* **netapp.ontap.na_ontap_volume_clone** : NetApp ONTAP manage volume clones.
* **netapp.ontap.na_ontap_volume_efficiency** : NetApp ONTAP enables, disables or modifies volume efficiency
* **netapp.ontap.na_ontap_volume_snaplock** : NetApp ONTAP manage volume snaplock retention.
* **netapp.ontap.na_ontap_vscan** : NetApp ONTAP Vscan enable/disable.
* **netapp.ontap.na_ontap_vscan_on_access_policy** : NetApp ONTAP Vscan on access policy configuration.
* **netapp.ontap.na_ontap_vscan_on_demand_task** : NetApp ONTAP Vscan on demand task configuration.
* **netapp.ontap.na_ontap_vscan_scanner_pool** : NetApp ONTAP Vscan Scanner Pools Configuration.
* **netapp.ontap.na_ontap_vserver_audit** : NetApp Ontap - create, delete or modify vserver audit configuration.
* **netapp.ontap.na_ontap_vserver_cifs_security** : NetApp ONTAP vserver CIFS security modification
* **netapp.ontap.na_ontap_vserver_peer** : NetApp ONTAP Vserver peering
* **netapp.ontap.na_ontap_vserver_peer_permissions** : NetApp Ontap - create, delete or modify vserver peer permission.
* **netapp.ontap.na_ontap_wait_for_condition** : NetApp ONTAP wait_for_condition.  Loop over a get status request until a condition is met.
* **netapp.ontap.na_ontap_wwpn_alias** : NetApp ONTAP set FCP WWPN Alias
* **netapp.ontap.na_ontap_zapit** : NetApp ONTAP Run any ZAPI on ONTAP

## `netapp.storagegrid` collection

* **netapp.storagegrid.na_sg_grid_account** : NetApp StorageGRID manage accounts.
* **netapp.storagegrid.na_sg_grid_certificate** : Manage the Storage API and Grid Management certificates on StorageGRID.
* **netapp.storagegrid.na_sg_grid_client_certificate** : Manage Client Certificates on StorageGRID
* **netapp.storagegrid.na_sg_grid_dns** : NetApp StorageGRID manage external DNS servers for the grid.
* **netapp.storagegrid.na_sg_grid_gateway** : Manage Load balancer (gateway) endpoints on StorageGRID.
* **netapp.storagegrid.na_sg_grid_group** : NetApp StorageGRID manage groups.
* **netapp.storagegrid.na_sg_grid_ha_group** : Manage high availability (HA) group configuration on StorageGRID.
* **netapp.storagegrid.na_sg_grid_identity_federation** : NetApp StorageGRID manage Grid identity federation.
* **netapp.storagegrid.na_sg_grid_info** : NetApp StorageGRID Grid information gatherer.
* **netapp.storagegrid.na_sg_grid_ntp** : NetApp StorageGRID manage external NTP servers for the grid.
* **netapp.storagegrid.na_sg_grid_regions** : NetApp StorageGRID manage Regions for the grid.
* **netapp.storagegrid.na_sg_grid_traffic_classes** : Manage Traffic Classification Policy configuration on StorageGRID.
* **netapp.storagegrid.na_sg_grid_user** : NetApp StorageGRID manage users.
* **netapp.storagegrid.na_sg_org_container** : Manage buckets on StorageGRID.
* **netapp.storagegrid.na_sg_org_group** : NetApp StorageGRID manage groups within a tenancy.
* **netapp.storagegrid.na_sg_org_identity_federation** : NetApp StorageGRID manage Tenant identity federation.
* **netapp.storagegrid.na_sg_org_info** : NetApp StorageGRID Org information gatherer.
* **netapp.storagegrid.na_sg_org_user** : NetApp StorageGRID manage users within a tenancy.
* **netapp.storagegrid.na_sg_org_user_s3_key** : Creates NetApp StorageGRID User S3 keys.

## `netapp.um_info` collection

* **netapp.um_info.na_um_aggregates_info** : NetApp Unified Manager list aggregates.
* **netapp.um_info.na_um_clusters_info** : NetApp Unified Manager list cluster.
* **netapp.um_info.na_um_nodes_info** : NetApp Unified Manager list nodes.
* **netapp.um_info.na_um_svms_info** : NetApp Unified Manager list svms.
* **netapp.um_info.na_um_volumes_info** : NetApp Unified Manager list volumes.

## `netapp_eseries.santricity` collection

* **netapp_eseries.santricity.netapp_e_alerts** : NetApp E-Series manage email notification settings
* **netapp_eseries.santricity.na_santricity_alerts_syslog** : NetApp E-Series manage syslog servers receiving storage system alerts.
* **netapp_eseries.santricity.netapp_e_asup** : NetApp E-Series manage auto-support settings
* **netapp_eseries.santricity.netapp_e_auditlog** : NetApp E-Series manage audit-log configuration
* **netapp_eseries.santricity.na_santricity_auth** : NetApp E-Series set or update the password for a storage array device or SANtricity Web Services Proxy.
* **netapp_eseries.santricity.na_santricity_client_certificate** : NetApp E-Series manage remote server certificates.
* **netapp_eseries.santricity.na_santricity_discover** : NetApp E-Series discover E-Series storage systems
* **netapp_eseries.santricity.netapp_e_drive_firmware** : NetApp E-Series manage drive firmware
* **netapp_eseries.santricity.netapp_e_facts** : NetApp E-Series retrieve facts about NetApp E-Series storage arrays
* **netapp_eseries.santricity.netapp_e_firmware** : NetApp E-Series manage firmware.
* **netapp_eseries.santricity.netapp_e_global** : NetApp E-Series manage global settings configuration
* **netapp_eseries.santricity.netapp_e_host** : NetApp E-Series manage eseries hosts
* **netapp_eseries.santricity.netapp_e_hostgroup** : NetApp E-Series manage array host groups
* **netapp_eseries.santricity.na_santricity_ib_iser_interface** : NetApp E-Series manage InfiniBand iSER interface configuration
* **netapp_eseries.santricity.netapp_e_iscsi_target** : NetApp E-Series manage iSCSI target configuration
* **netapp_eseries.santricity.netapp_e_ldap** : NetApp E-Series manage LDAP integration to use for authentication
* **netapp_eseries.santricity.na_santricity_lun_mapping** : NetApp E-Series manage lun mappings
* **netapp_eseries.santricity.na_santricity_mgmt_interface** : NetApp E-Series manage management interface configuration
* **netapp_eseries.santricity.na_santricity_nvme_interface** : NetApp E-Series manage NVMe interface configuration
* **netapp_eseries.santricity.na_santricity_proxy_drive_firmware_upload** : NetApp E-Series manage proxy drive firmware files
* **netapp_eseries.santricity.na_santricity_proxy_firmware_upload** : NetApp E-Series manage proxy firmware uploads.
* **netapp_eseries.santricity.na_santricity_proxy_systems** : NetApp E-Series manage SANtricity web services proxy storage arrays
* **netapp_eseries.santricity.na_santricity_server_certificate** : NetApp E-Series manage the storage system&#39;s server SSL certificates.
* **netapp_eseries.santricity.na_santricity_snapshot** : NetApp E-Series storage system&#39;s snapshots.
* **netapp_eseries.santricity.netapp_e_storagepool** : NetApp E-Series manage volume groups and disk pools
* **netapp_eseries.santricity.netapp_e_syslog** : NetApp E-Series manage syslog settings
* **netapp_eseries.santricity.netapp_e_volume** : NetApp E-Series manage storage volumes (standard and thin)
* **netapp_eseries.santricity.netapp_e_amg** : NetApp E-Series create, remove, and update asynchronous mirror groups
* **netapp_eseries.santricity.netapp_e_amg_role** : NetApp E-Series update the role of a storage array within an Asynchronous Mirror Group (AMG).
* **netapp_eseries.santricity.netapp_e_amg_sync** : NetApp E-Series conduct synchronization actions on asynchronous mirror groups.
* **netapp_eseries.santricity.netapp_e_auth** : NetApp E-Series set or update the password for a storage array.
* **netapp_eseries.santricity.netapp_e_flashcache** : NetApp E-Series manage SSD caches
* **netapp_eseries.santricity.netapp_e_iscsi_interface** : NetApp E-Series manage iSCSI interface configuration
* **netapp_eseries.santricity.netapp_e_lun_mapping** : NetApp E-Series create, delete, or modify lun mappings
* **netapp_eseries.santricity.netapp_e_mgmt_interface** : NetApp E-Series management interface configuration
* **netapp_eseries.santricity.netapp_e_snapshot_group** : NetApp E-Series manage snapshot groups
* **netapp_eseries.santricity.netapp_e_snapshot_images** : NetApp E-Series create and delete snapshot images
* **netapp_eseries.santricity.netapp_e_snapshot_volume** : NetApp E-Series manage snapshot volumes.
* **netapp_eseries.santricity.netapp_e_storage_system** : NetApp E-Series Web Services Proxy manage storage arrays
* **netapp_eseries.santricity.netapp_e_volume_copy** : NetApp E-Series create volume copy pairs

## `netbox.netbox` collection

* **netbox.netbox.netbox_aggregate** : Creates or removes aggregates from NetBox
* **netbox.netbox.netbox_cable** : Create, update or delete cables within NetBox
* **netbox.netbox.netbox_circuit** : Create, update or delete circuits within NetBox
* **netbox.netbox.netbox_circuit_termination** : Create, update or delete circuit terminations within NetBox
* **netbox.netbox.netbox_circuit_type** : Create, update or delete circuit types within NetBox
* **netbox.netbox.netbox_cluster** : Create, update or delete clusters within NetBox
* **netbox.netbox.netbox_cluster_group** : Create, update or delete cluster groups within NetBox
* **netbox.netbox.netbox_cluster_type** : Create, update or delete cluster types within NetBox
* **netbox.netbox.netbox_config_context** : Creates, updates or deletes configuration contexts within NetBox
* **netbox.netbox.netbox_console_port** : Create, update or delete console ports within NetBox
* **netbox.netbox.netbox_console_port_template** : Create, update or delete console port templates within NetBox
* **netbox.netbox.netbox_console_server_port** : Create, update or delete console server ports within NetBox
* **netbox.netbox.netbox_console_server_port_template** : Create, update or delete console server port templates within NetBox
* **netbox.netbox.netbox_contact** : Creates or removes contacts from NetBox
* **netbox.netbox.netbox_contact_group** : Creates or removes contact groups from NetBox
* **netbox.netbox.netbox_contact_role** : Creates or removes contact roles from NetBox
* **netbox.netbox.netbox_custom_field** : Creates, updates or deletes custom fields within NetBox
* **netbox.netbox.netbox_custom_link** : Creates, updates or deletes custom links within NetBox
* **netbox.netbox.netbox_device** : Create, update or delete devices within NetBox
* **netbox.netbox.netbox_device_bay** : Create, update or delete device bays within NetBox
* **netbox.netbox.netbox_device_bay_template** : Create, update or delete device bay templates within NetBox
* **netbox.netbox.netbox_device_interface_template** : Creates or removes interfaces on devices from NetBox
* **netbox.netbox.netbox_inventory_item_role** : Create, update or delete devices roles within NetBox
* **netbox.netbox.netbox_device_type** : Create, update or delete device types within NetBox
* **netbox.netbox.netbox_export_template** : Creates, updates or deletes export templates within NetBox
* **netbox.netbox.netbox_front_port** : Create, update or delete front ports within NetBox
* **netbox.netbox.netbox_front_port_template** : Create, update or delete front port templates within NetBox
* **netbox.netbox.netbox_inventory_item** : Creates or removes inventory items from NetBox
* **netbox.netbox.netbox_ip_address** : Creates or removes IP addresses from NetBox
* **netbox.netbox.netbox_ipam_role** : Creates or removes ipam roles from NetBox
* **netbox.netbox.netbox_l2vpn** : Create, update or delete L2VPNs within NetBox
* **netbox.netbox.netbox_location** : Create, update or delete locations within NetBox
* **netbox.netbox.netbox_manufacturer** : Create or delete manufacturers within NetBox
* **netbox.netbox.netbox_module_type** : Create, update or delete module types within NetBox
* **netbox.netbox.netbox_platform** : Create or delete platforms within NetBox
* **netbox.netbox.netbox_power_feed** : Create, update or delete power feeds within NetBox
* **netbox.netbox.netbox_power_outlet** : Create, update or delete power outlets within NetBox
* **netbox.netbox.netbox_power_outlet_template** : Create, update or delete power outlet templates within NetBox
* **netbox.netbox.netbox_power_panel** : Create, update or delete power panels within NetBox
* **netbox.netbox.netbox_power_port** : Create, update or delete power ports within NetBox
* **netbox.netbox.netbox_power_port_template** : Create, update or delete power port templates within NetBox
* **netbox.netbox.netbox_prefix** : Creates or removes prefixes from NetBox
* **netbox.netbox.netbox_provider** : Create, update or delete providers within NetBox
* **netbox.netbox.netbox_provider_network** : Create, update or delete provider networks within NetBox
* **netbox.netbox.netbox_rack** : Create, update or delete racks within NetBox
* **netbox.netbox.netbox_rack_group** : Create, update or delete racks groups within NetBox
* **netbox.netbox.netbox_rack_role** : Create, update or delete racks roles within NetBox
* **netbox.netbox.netbox_rear_port** : Create, update or delete rear ports within NetBox
* **netbox.netbox.netbox_rear_port_template** : Create, update or delete rear port templates within NetBox
* **netbox.netbox.netbox_region** : Creates or removes regions from NetBox
* **netbox.netbox.netbox_rir** : Create, update or delete RIRs within NetBox
* **netbox.netbox.netbox_route_target** : Creates or removes route targets from NetBox
* **netbox.netbox.netbox_service** : Creates or removes service from NetBox
* **netbox.netbox.netbox_service_template** : Create, update or delete service templates within NetBox
* **netbox.netbox.netbox_site** : Creates or removes sites from NetBox
* **netbox.netbox.netbox_site_group** : Create, update, or delete site groups within NetBox
* **netbox.netbox.netbox_tag** : Creates or removes tags from NetBox
* **netbox.netbox.netbox_tenant** : Creates or removes tenants from NetBox
* **netbox.netbox.netbox_tenant_group** : Creates or removes tenant groups from NetBox
* **netbox.netbox.netbox_virtual_chassis** : Create, update or delete virtual chassis within NetBox
* **netbox.netbox.netbox_virtual_machine** : Create, update or delete virtual_machines within NetBox
* **netbox.netbox.netbox_vlan** : Create, update or delete vlans within NetBox
* **netbox.netbox.netbox_vlan_group** : Create, update or delete vlans groups within NetBox
* **netbox.netbox.netbox_vm_interface** : Creates or removes interfaces from virtual machines in NetBox
* **netbox.netbox.netbox_vrf** : Create, update or delete vrfs within NetBox
* **netbox.netbox.netbox_webhook** : Creates, updates or deletes webhook configuration within NetBox
* **netbox.netbox.netbox_wireless_lan** : Creates or removes Wireless LANs from NetBox
* **netbox.netbox.netbox_wireless_lan_group** : Creates or removes Wireless LAN Groups from NetBox
* **netbox.netbox.netbox_wireless_link** : Creates or removes Wireless links from NetBox

## `ngine_io.cloudstack` collection

* **ngine_io.cloudstack.cs_account** : Manages accounts on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_affinitygroup** : Manages affinity groups on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_cluster** : Manages host clusters on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_configuration** : Manages configuration on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_disk_offering** : Manages disk offerings on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_domain** : Manages domains on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_facts** : Gather facts on instances of Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_firewall** : Manages firewall rules on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_host** : Manages hosts on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_image_store** : Manages CloudStack Image Stores.
* **ngine_io.cloudstack.cs_instance** : Manages instances and virtual machines on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_instance_info** : Gathering information from the API of instances from Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_instance_nic** : Manages NICs of an instance on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_instance_nic_secondaryip** : Manages secondary IPs of an instance on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_instance_password_reset** : Allows resetting VM the default passwords on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_instancegroup** : Manages instance groups on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_ip_address** : Manages public IP address associations on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_iso** : Manages ISO images on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_loadbalancer_rule** : Manages load balancer rules on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_loadbalancer_rule_member** : Manages load balancer rule members on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_network** : Manages networks on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_network_acl** : Manages network access control lists (ACL) on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_network_acl_rule** : Manages network access control list (ACL) rules on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_network_offering** : Manages network offerings on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_physical_network** : Manages physical networks on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_pod** : Manages pods on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_portforward** : Manages port forwarding rules on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_project** : Manages projects on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_region** : Manages regions on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_resourcelimit** : Manages resource limits on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_role** : Manages user roles on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_role_permission** : Manages role permissions on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_router** : Manages routers on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_securitygroup** : Manages security groups on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_securitygroup_rule** : Manages security group rules on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_service_offering** : Manages service offerings on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_snapshot_policy** : Manages volume snapshot policies on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_sshkeypair** : Manages SSH keys on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_staticnat** : Manages static NATs on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_storage_pool** : Manages Primary Storage Pools on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_template** : Manages templates on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_traffic_type** : Manages traffic types on CloudStack Physical Networks
* **ngine_io.cloudstack.cs_user** : Manages users on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_vlan_ip_range** : Manages VLAN IP ranges on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_vmsnapshot** : Manages VM snapshots on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_volume** : Manages volumes on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_vpc** : Manages VPCs on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_vpc_offering** : Manages vpc offerings on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_vpn_connection** : Manages site-to-site VPN connections on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_vpn_customer_gateway** : Manages site-to-site VPN customer gateway configurations on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_vpn_gateway** : Manages site-to-site VPN gateways on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_zone** : Manages zones on Apache CloudStack based clouds.
* **ngine_io.cloudstack.cs_zone_info** : Gathering information about zones from Apache CloudStack based clouds.

## `ngine_io.exoscale` collection

* **ngine_io.exoscale.exo_dns_domain** : Manages domain records on Exoscale DNS API.
* **ngine_io.exoscale.exo_dns_record** : Manages DNS records on Exoscale DNS.

## `ngine_io.vultr` collection

* **ngine_io.vultr.vultr_account_info** : Get information about the Vultr account.
* **ngine_io.vultr.vultr_block_storage** : Manages block storage volumes on Vultr.
* **ngine_io.vultr.vultr_block_storage_info** : Get information about the Vultr block storage volumes available.
* **ngine_io.vultr.vultr_dns_domain** : Manages DNS domains on Vultr.
* **ngine_io.vultr.vultr_dns_domain_info** : Gather information about the Vultr DNS domains available.
* **ngine_io.vultr.vultr_dns_record** : Manages DNS records on Vultr.
* **ngine_io.vultr.vultr_firewall_group** : Manages firewall groups on Vultr.
* **ngine_io.vultr.vultr_firewall_group_info** : Gather information about the Vultr firewall groups available.
* **ngine_io.vultr.vultr_firewall_rule** : Manages firewall rules on Vultr.
* **ngine_io.vultr.vultr_network** : Manages networks on Vultr.
* **ngine_io.vultr.vultr_network_info** : Gather information about the Vultr networks available.
* **ngine_io.vultr.vultr_os_info** : Get information about the Vultr OSes available.
* **ngine_io.vultr.vultr_plan_baremetal_info** : Gather information about the Vultr Bare Metal plans available.
* **ngine_io.vultr.vultr_plan_info** : Gather information about the Vultr plans available.
* **ngine_io.vultr.vultr_region_info** : Gather information about the Vultr regions available.
* **ngine_io.vultr.vultr_server** : Manages virtual servers on Vultr.
* **ngine_io.vultr.vultr_server_baremetal** : Manages baremetal servers on Vultr.
* **ngine_io.vultr.vultr_server_info** : Gather information about the Vultr servers available.
* **ngine_io.vultr.vultr_ssh_key** : Manages ssh keys on Vultr.
* **ngine_io.vultr.vultr_ssh_key_info** : Get information about the Vultr SSH keys available.
* **ngine_io.vultr.vultr_startup_script** : Manages startup scripts on Vultr.
* **ngine_io.vultr.vultr_startup_script_info** : Gather information about the Vultr startup scripts available.
* **ngine_io.vultr.vultr_user** : Manages users on Vultr.
* **ngine_io.vultr.vultr_user_info** : Get information about the Vultr user available.

## `openstack.cloud` collection

* **openstack.cloud.address_scope** : Create or delete address scopes from OpenStack
* **openstack.cloud.auth** : Retrieve an auth token
* **openstack.cloud.baremetal_inspect** : Explicitly triggers baremetal node introspection in ironic.
* **openstack.cloud.baremetal_node** : Create/Delete Bare Metal Resources from OpenStack
* **openstack.cloud.baremetal_node_action** : Activate/Deactivate Bare Metal Resources from OpenStack
* **openstack.cloud.baremetal_node_info** : Retrieve information about Bare Metal nodes from OpenStack
* **openstack.cloud.baremetal_port** : Create/Delete Bare Metal port Resources from OpenStack
* **openstack.cloud.baremetal_port_info** : Retrieve information about Bare Metal ports from OpenStack
* **openstack.cloud.catalog_service** : Manage OpenStack Identity services
* **openstack.cloud.coe_cluster** : Add/Remove COE cluster from OpenStack Cloud
* **openstack.cloud.coe_cluster_template** : Add/Remove COE cluster template from OpenStack Cloud
* **openstack.cloud.compute_flavor** : Manage OpenStack compute flavors
* **openstack.cloud.compute_flavor_info** : Retrieve information about one or more flavors
* **openstack.cloud.compute_service_info** : Retrieve information about one or more OpenStack compute services
* **openstack.cloud.config** : Get OpenStack Client config
* **openstack.cloud.object_container** : Manage Swift container.
* **openstack.cloud.dns_zone** : Manage OpenStack DNS zones
* **openstack.cloud.dns_zone_info** : Getting information about dns zones
* **openstack.cloud.endpoint** : Manage OpenStack Identity service endpoints
* **openstack.cloud.federation_idp** : manage a federation Identity Provider
* **openstack.cloud.federation_idp_info** : Get the information about the available federation identity providers
* **openstack.cloud.federation_mapping** : Manage a federation mapping
* **openstack.cloud.federation_mapping_info** : Get the information about the available federation mappings
* **openstack.cloud.floating_ip** : Add/Remove floating IP from an instance
* **openstack.cloud.floating_ip_info** : Get information about floating ips
* **openstack.cloud.group_assignment** : Associate OpenStack Identity users and groups
* **openstack.cloud.host_aggregate** : Manage OpenStack host aggregates
* **openstack.cloud.identity_domain** : Manage OpenStack Identity Domains
* **openstack.cloud.identity_domain_info** : Retrieve information about one or more OpenStack domains
* **openstack.cloud.identity_group** : Manage OpenStack Identity Groups
* **openstack.cloud.identity_group_info** : Retrieve info about one or more OpenStack groups
* **openstack.cloud.identity_role** : Manage OpenStack Identity Roles
* **openstack.cloud.identity_role_info** : Retrieve information about roles
* **openstack.cloud.identity_user** : Manage OpenStack Identity Users
* **openstack.cloud.identity_user_info** : Retrieve information about one or more OpenStack users
* **openstack.cloud.image** : Add/Delete images from OpenStack Cloud
* **openstack.cloud.image_info** : Retrieve information about an image within OpenStack.
* **openstack.cloud.keypair** : Add/Delete a keypair from OpenStack
* **openstack.cloud.keypair_info** : Get information about keypairs from OpenStack
* **openstack.cloud.keystone_federation_protocol** : manage a federation Protocol
* **openstack.cloud.keystone_federation_protocol_info** : get information about federation Protocols
* **openstack.cloud.lb_health_monitor** : Add/Delete a health m nonitor to a pool in the load balancing service from OpenStack Cloud
* **openstack.cloud.lb_listener** : Add/Delete a listener for a load balancer from OpenStack Cloud
* **openstack.cloud.lb_member** : Add/Delete a member for a pool in load balancer from OpenStack Cloud
* **openstack.cloud.lb_pool** : Add/Delete a pool in the load balancing service from OpenStack Cloud
* **openstack.cloud.loadbalancer** : Add/Delete load balancer from OpenStack Cloud
* **openstack.cloud.network** : Creates/removes networks from OpenStack
* **openstack.cloud.networks_info** : Retrieve information about one or more OpenStack networks.
* **openstack.cloud.neutron_rbac_policies_info** : Fetch Neutron policies.
* **openstack.cloud.neutron_rbac_policy** : Create or delete a Neutron policy to apply a RBAC rule against an object.
* **openstack.cloud.object** : Create or Delete objects and containers from OpenStack
* **openstack.cloud.port** : Add/Update/Delete ports from an OpenStack cloud.
* **openstack.cloud.port_info** : Retrieve information about ports within OpenStack.
* **openstack.cloud.project** : Manage OpenStack Projects
* **openstack.cloud.project_access** : Manage OpenStack compute flavors access
* **openstack.cloud.project_info** : Retrieve information about one or more OpenStack projects
* **openstack.cloud.quota** : Manage OpenStack Quotas
* **openstack.cloud.recordset** : Manage OpenStack DNS recordsets
* **openstack.cloud.router** : Create or delete routers from OpenStack
* **openstack.cloud.routers_info** : Retrieve information about one or more OpenStack routers.
* **openstack.cloud.security_group** : Add/Delete security groups from an OpenStack cloud.
* **openstack.cloud.security_group_rule** : Add/Delete rule from an existing security group
* **openstack.cloud.server** : Create/Delete Compute Instances from OpenStack
* **openstack.cloud.server_action** : Perform actions on Compute Instances from OpenStack
* **openstack.cloud.server_group** : Manage OpenStack server groups
* **openstack.cloud.server_info** : Retrieve information about one or more compute instances
* **openstack.cloud.server_metadata** : Add/Update/Delete Metadata in Compute Instances from OpenStack
* **openstack.cloud.server_volume** : Attach/Detach Volumes from OpenStack VM&#39;s
* **openstack.cloud.stack** : Add/Remove Heat Stack
* **openstack.cloud.subnet** : Add/Remove subnet to an OpenStack network
* **openstack.cloud.subnets_info** : Retrieve information about one or more OpenStack subnets.
* **openstack.cloud.role_assignment** : Associate OpenStack Identity users and roles
* **openstack.cloud.volume** : Create/Delete Cinder Volumes
* **openstack.cloud.volume_snapshot** : Create/Delete Cinder Volume Snapshots
* **openstack.cloud.security_group_info** : Lists security groups
* **openstack.cloud.security_group_rule_info** : Querying security group rules
* **openstack.cloud.stack_info** : Retrive information about Heat stacks
* **openstack.cloud.subnet_pool** : Create or delete subnet pools from OpenStack
* **openstack.cloud.volume_backup** : Add/Delete Volume backup
* **openstack.cloud.volume_backup_info** : Get Backups
* **openstack.cloud.volume_info** : Retrive information about volumes
* **openstack.cloud.volume_snapshot_info** : Get volume snapshots

## `openvswitch.openvswitch` collection

* **openvswitch.openvswitch.openvswitch_bond** : Manage Open vSwitch bonds
* **openvswitch.openvswitch.openvswitch_bridge** : Manage Open vSwitch bridges
* **openvswitch.openvswitch.openvswitch_db** : Configure open vswitch database.
* **openvswitch.openvswitch.openvswitch_port** : Manage Open vSwitch ports

## `ovirt.ovirt` collection

* **ovirt.ovirt.ovirt_affinity_group** : Module to manage affinity groups in oVirt/RHV
* **ovirt.ovirt.ovirt_affinity_label** : Module to manage affinity labels in oVirt/RHV
* **ovirt.ovirt.ovirt_affinity_label_info** : Retrieve information about one or more oVirt/RHV affinity labels
* **ovirt.ovirt.ovirt_api_info** : Retrieve information about the oVirt/RHV API
* **ovirt.ovirt.ovirt_auth** : Module to manage authentication to oVirt/RHV
* **ovirt.ovirt.ovirt_cluster** : Module to manage clusters in oVirt/RHV
* **ovirt.ovirt.ovirt_cluster_info** : Retrieve information about one or more oVirt/RHV clusters
* **ovirt.ovirt.ovirt_datacenter** : Module to manage data centers in oVirt/RHV
* **ovirt.ovirt.ovirt_datacenter_info** : Retrieve information about one or more oVirt/RHV datacenters
* **ovirt.ovirt.ovirt_disk** : Module to manage Virtual Machine and floating disks in oVirt/RHV
* **ovirt.ovirt.ovirt_disk_info** : Retrieve information about one or more oVirt/RHV disks
* **ovirt.ovirt.ovirt_disk_profile** : Module to manage storage domain disk profiles in ovirt
* **ovirt.ovirt.ovirt_event** : Create or delete an event in oVirt/RHV
* **ovirt.ovirt.ovirt_event_info** : This module can be used to retrieve information about one or more oVirt/RHV events
* **ovirt.ovirt.ovirt_external_provider** : Module to manage external providers in oVirt/RHV
* **ovirt.ovirt.ovirt_external_provider_info** : Retrieve information about one or more oVirt/RHV external providers
* **ovirt.ovirt.ovirt_group** : Module to manage groups in oVirt/RHV
* **ovirt.ovirt.ovirt_group_info** : Retrieve information about one or more oVirt/RHV groups
* **ovirt.ovirt.ovirt_host** : Module to manage hosts in oVirt/RHV
* **ovirt.ovirt.ovirt_host_info** : Retrieve information about one or more oVirt/RHV hosts
* **ovirt.ovirt.ovirt_host_network** : Module to manage host networks in oVirt/RHV
* **ovirt.ovirt.ovirt_host_pm** : Module to manage power management of hosts in oVirt/RHV
* **ovirt.ovirt.ovirt_host_storage_info** : Retrieve information about one or more oVirt/RHV HostStorages (applicable only for block storage)
* **ovirt.ovirt.ovirt_instance_type** : Module to manage Instance Types in oVirt/RHV
* **ovirt.ovirt.ovirt_job** : Module to manage jobs in oVirt/RHV
* **ovirt.ovirt.ovirt_mac_pool** : Module to manage MAC pools in oVirt/RHV
* **ovirt.ovirt.ovirt_network** : Module to manage logical networks in oVirt/RHV
* **ovirt.ovirt.ovirt_network_info** : Retrieve information about one or more oVirt/RHV networks
* **ovirt.ovirt.ovirt_nic** : Module to manage network interfaces of Virtual Machines in oVirt/RHV
* **ovirt.ovirt.ovirt_nic_info** : Retrieve information about one or more oVirt/RHV virtual machine network interfaces
* **ovirt.ovirt.ovirt_permission** : Module to manage permissions of users/groups in oVirt/RHV
* **ovirt.ovirt.ovirt_permission_info** : Retrieve information about one or more oVirt/RHV permissions
* **ovirt.ovirt.ovirt_qos** : Module to manage QoS entries in ovirt
* **ovirt.ovirt.ovirt_quota** : Module to manage datacenter quotas in oVirt/RHV
* **ovirt.ovirt.ovirt_quota_info** : Retrieve information about one or more oVirt/RHV quotas
* **ovirt.ovirt.ovirt_role** : Module to manage roles in oVirt/RHV
* **ovirt.ovirt.ovirt_scheduling_policy_info** : Retrieve information about one or more oVirt scheduling policies
* **ovirt.ovirt.ovirt_snapshot** : Module to manage Virtual Machine Snapshots in oVirt/RHV
* **ovirt.ovirt.ovirt_snapshot_info** : Retrieve information about one or more oVirt/RHV virtual machine snapshots
* **ovirt.ovirt.ovirt_storage_connection** : Module to manage storage connections in oVirt
* **ovirt.ovirt.ovirt_storage_domain** : Module to manage storage domains in oVirt/RHV
* **ovirt.ovirt.ovirt_storage_domain_info** : Retrieve information about one or more oVirt/RHV storage domains
* **ovirt.ovirt.ovirt_storage_template_info** : Retrieve information about one or more oVirt/RHV templates relate to a storage domain.
* **ovirt.ovirt.ovirt_storage_vm_info** : Retrieve information about one or more oVirt/RHV virtual machines relate to a storage domain.
* **ovirt.ovirt.ovirt_system_option_info** : Retrieve information about one oVirt/RHV system options.
* **ovirt.ovirt.ovirt_tag** : Module to manage tags in oVirt/RHV
* **ovirt.ovirt.ovirt_tag_info** : Retrieve information about one or more oVirt/RHV tags
* **ovirt.ovirt.ovirt_template** : Module to manage virtual machine templates in oVirt/RHV
* **ovirt.ovirt.ovirt_template_info** : Retrieve information about one or more oVirt/RHV templates
* **ovirt.ovirt.ovirt_user** : Module to manage users in oVirt/RHV
* **ovirt.ovirt.ovirt_user_info** : Retrieve information about one or more oVirt/RHV users
* **ovirt.ovirt.ovirt_vm** : Module to manage Virtual Machines in oVirt/RHV
* **ovirt.ovirt.ovirt_vm_info** : Retrieve information about one or more oVirt/RHV virtual machines
* **ovirt.ovirt.ovirt_vm_os_info** : Retrieve information on all supported oVirt/RHV operating systems
* **ovirt.ovirt.ovirt_vmpool** : Module to manage VM pools in oVirt/RHV
* **ovirt.ovirt.ovirt_vmpool_info** : Retrieve information about one or more oVirt/RHV vmpools
* **ovirt.ovirt.ovirt_vnic_profile** : Module to manage vNIC profile of network in oVirt/RHV
* **ovirt.ovirt.ovirt_vnic_profile_info** : Retrieve information about one or more oVirt/RHV vnic profiles

## `purestorage.flasharray` collection

* **purestorage.flasharray.purefa_ad** : Manage FlashArray Active Directory Account
* **purestorage.flasharray.purefa_admin** : Configure Pure Storage FlashArray Global Admin settings
* **purestorage.flasharray.purefa_alert** : Configure Pure Storage FlashArray alert email settings
* **purestorage.flasharray.purefa_apiclient** : Manage FlashArray API Clients
* **purestorage.flasharray.purefa_arrayname** : Configure Pure Storage FlashArray array name
* **purestorage.flasharray.purefa_banner** : Configure Pure Storage FlashArray GUI and SSH MOTD message
* **purestorage.flasharray.purefa_certs** : Manage FlashArray SSL Certificates
* **purestorage.flasharray.purefa_connect** : Manage replication connections between two FlashArrays
* **purestorage.flasharray.purefa_console** : Enable or Disable Pure Storage FlashArray Console Lock
* **purestorage.flasharray.purefa_default_protection** : Manage SafeMode default protection for a Pure Storage FlashArray
* **purestorage.flasharray.purefa_directory** : Manage FlashArray File System Directories
* **purestorage.flasharray.purefa_dirsnap** : Manage FlashArray File System Directory Snapshots
* **purestorage.flasharray.purefa_dns** : Configure FlashArray DNS settings
* **purestorage.flasharray.purefa_ds** : Configure FlashArray Directory Service
* **purestorage.flasharray.purefa_dsrole** : Configure FlashArray Directory Service Roles
* **purestorage.flasharray.purefa_endpoint** : Manage VMware protocol-endpoints on Pure Storage FlashArrays
* **purestorage.flasharray.purefa_eradication** : Configure Pure Storage FlashArray Eradication Timer
* **purestorage.flasharray.purefa_eula** : Sign Pure Storage FlashArray EULA
* **purestorage.flasharray.purefa_export** : Manage FlashArray File System Exports
* **purestorage.flasharray.purefa_fs** : Manage FlashArray File Systems
* **purestorage.flasharray.purefa_hg** : Manage hostgroups on Pure Storage FlashArrays
* **purestorage.flasharray.purefa_host** : Manage hosts on Pure Storage FlashArrays
* **purestorage.flasharray.purefa_inventory** : Collect information from Pure Storage FlashArray
* **purestorage.flasharray.purefa_kmip** : Manage FlashArray KMIP server objects
* **purestorage.flasharray.purefa_maintenance** : Configure Pure Storage FlashArray Maintence Windows
* **purestorage.flasharray.purefa_messages** : List FlashArray Alert Messages
* **purestorage.flasharray.purefa_network** : Manage network interfaces in a Pure Storage FlashArray
* **purestorage.flasharray.purefa_ntp** : Configure Pure Storage FlashArray NTP settings
* **purestorage.flasharray.purefa_offload** : Create, modify and delete NFS, S3 or Azure offload targets
* **purestorage.flasharray.purefa_pg** : Manage protection groups on Pure Storage FlashArrays
* **purestorage.flasharray.purefa_pgsched** : Manage protection groups replication schedules on Pure Storage FlashArrays
* **purestorage.flasharray.purefa_pgsnap** : Manage protection group snapshots on Pure Storage FlashArrays
* **purestorage.flasharray.purefa_phonehome** : Enable or Disable Pure Storage FlashArray Phonehome
* **purestorage.flasharray.purefa_pod** : Manage AC pods in Pure Storage FlashArrays
* **purestorage.flasharray.purefa_pod_replica** : Manage ActiveDR pod replica links between Pure Storage FlashArrays
* **purestorage.flasharray.purefa_policy** : Manage FlashArray File System Policies
* **purestorage.flasharray.purefa_proxy** : Configure FlashArray phonehome HTTPs proxy settings
* **purestorage.flasharray.purefa_ra** : Enable or Disable Pure Storage FlashArray Remote Assist
* **purestorage.flasharray.purefa_saml** : Manage FlashArray SAML2 service and identity providers
* **purestorage.flasharray.purefa_smis** : Enable or disable FlashArray SMI-S features
* **purestorage.flasharray.purefa_smtp** : Configure FlashArray SMTP settings
* **purestorage.flasharray.purefa_snap** : Manage volume snapshots on Pure Storage FlashArrays
* **purestorage.flasharray.purefa_snmp** : Configure FlashArray SNMP Managers
* **purestorage.flasharray.purefa_snmp_agent** : Configure the FlashArray SNMP Agent
* **purestorage.flasharray.purefa_subnet** : Manage network subnets in a Pure Storage FlashArray
* **purestorage.flasharray.purefa_syslog** : Configure Pure Storage FlashArray syslog settings
* **purestorage.flasharray.purefa_syslog_settings** : Manage FlashArray syslog servers settings
* **purestorage.flasharray.purefa_timeout** : Configure Pure Storage FlashArray GUI idle timeout
* **purestorage.flasharray.purefa_user** : Create, modify or delete FlashArray local user account
* **purestorage.flasharray.purefa_vg** : Manage volume groups on Pure Storage FlashArrays
* **purestorage.flasharray.purefa_vlan** : Manage network VLAN interfaces in a Pure Storage FlashArray
* **purestorage.flasharray.purefa_vnc** : Enable or Disable VNC port for installed apps
* **purestorage.flasharray.purefa_volume** : Manage volumes on Pure Storage FlashArrays
* **purestorage.flasharray.purefa_volume_tags** : Manage volume tags on Pure Storage FlashArrays

## `purestorage.flashblade` collection

* **purestorage.flashblade.purefb_ad** : Manage FlashBlade Active Directory Account
* **purestorage.flashblade.purefb_admin** : Configure Pure Storage FlashBlade Global Admin settings
* **purestorage.flashblade.purefb_alert** : Configure Pure Storage FlashBlade alert email settings
* **purestorage.flashblade.purefb_apiclient** : Manage FlashBlade API Clients
* **purestorage.flashblade.purefb_banner** : Configure Pure Storage FlashBlade GUI and SSH MOTD message
* **purestorage.flashblade.purefb_bladename** : Configure Pure Storage FlashBlade name
* **purestorage.flashblade.purefb_bucket** : Manage Object Store Buckets on a  Pure Storage FlashBlade.
* **purestorage.flashblade.purefb_bucket_replica** : Manage bucket replica links between Pure Storage FlashBlades
* **purestorage.flashblade.purefb_certgrp** : Manage FlashBlade Certifcate Groups
* **purestorage.flashblade.purefb_certs** : Manage FlashBlade SSL Certificates
* **purestorage.flashblade.purefb_connect** : Manage replication connections between two FlashBlades
* **purestorage.flashblade.purefb_dns** : Configure Pure Storage FlashBlade DNS settings
* **purestorage.flashblade.purefb_ds** : Configure FlashBlade Directory Service
* **purestorage.flashblade.purefb_dsrole** : Configure FlashBlade  Management Directory Service Roles
* **purestorage.flashblade.purefb_eula** : Sign Pure Storage FlashBlade EULA
* **purestorage.flashblade.purefb_fs** : Manage filesystemon Pure Storage FlashBlade`
* **purestorage.flashblade.purefb_fs_replica** : Manage filesystem replica links between Pure Storage FlashBlades
* **purestorage.flashblade.purefb_groupquota** : Manage filesystem group quotas
* **purestorage.flashblade.purefb_inventory** : Collect information from Pure Storage FlashBlade
* **purestorage.flashblade.purefb_keytabs** : Manage FlashBlade Kerberos Keytabs
* **purestorage.flashblade.purefb_lag** : Manage FlashBlade Link Aggregation Groups
* **purestorage.flashblade.purefb_lifecycle** : Manage FlashBlade object lifecycles
* **purestorage.flashblade.purefb_messages** : List FlashBlade Alert Messages
* **purestorage.flashblade.purefb_network** : Manage network interfaces in a Pure Storage FlashBlade
* **purestorage.flashblade.purefb_ntp** : Configure Pure Storage FlashBlade NTP settings
* **purestorage.flashblade.purefb_phonehome** : Enable or Disable Pure Storage FlashBlade Phone Home
* **purestorage.flashblade.purefb_policy** : Manage FlashBlade policies
* **purestorage.flashblade.purefb_proxy** : Configure FlashBlade phonehome HTTPs proxy settings
* **purestorage.flashblade.purefb_ra** : Enable or Disable Pure Storage FlashBlade Remote Assist
* **purestorage.flashblade.purefb_remote_cred** : Create, modify and delete FlashBlade object store remote credentials
* **purestorage.flashblade.purefb_s3acc** : Create or delete FlashBlade Object Store accounts
* **purestorage.flashblade.purefb_s3user** : Create or delete FlashBlade Object Store account users
* **purestorage.flashblade.purefb_smtp** : Configure SMTP for Pure Storage FlashBlade
* **purestorage.flashblade.purefb_snap** : Manage filesystem snapshots on Pure Storage FlashBlades
* **purestorage.flashblade.purefb_snmp_agent** : Configure the FlashBlade SNMP Agent
* **purestorage.flashblade.purefb_snmp_mgr** : Configure FlashBlade SNMP Managers
* **purestorage.flashblade.purefb_subnet** : Manage network subnets in a Pure Storage FlashBlade
* **purestorage.flashblade.purefb_syslog** : Configure Pure Storage FlashBlade syslog settings
* **purestorage.flashblade.purefb_target** : Manage remote S3-capable targets for a FlashBlade
* **purestorage.flashblade.purefb_timeout** : Configure Pure Storage FlashBlade GUI idle timeout
* **purestorage.flashblade.purefb_tz** : Configure Pure Storage FlashBlade timezone
* **purestorage.flashblade.purefb_user** : Modify FlashBlade user accounts
* **purestorage.flashblade.purefb_userpolicy** : Manage FlashBlade Object Store User Access Policies
* **purestorage.flashblade.purefb_userquota** : Manage filesystem user quotas
* **purestorage.flashblade.purefb_virtualhost** : Manage FlashBlade Object Store Virtual Hosts

## `purestorage.fusion` collection

* **purestorage.fusion.fusion_api_client** : Manage API clients in Pure Storage Fusion
* **purestorage.fusion.fusion_array** : Manage arrays in Pure Storage Fusion
* **purestorage.fusion.fusion_az** : Create Availability Zones in Pure Storage Fusion
* **purestorage.fusion.fusion_hap** : Manage host access policies in Pure Storage Fusion
* **purestorage.fusion.fusion_hw** : Create hardware types in Pure Storage Fusion
* **purestorage.fusion.fusion_info** : Collect information from Pure Fusion
* **purestorage.fusion.fusion_nig** : Manage Network Interface Groups in Pure Storage Fusion
* **purestorage.fusion.fusion_pg** : Manage placement groups in Pure Storage Fusion
* **purestorage.fusion.fusion_pp** : Manage protection policies in Pure Storage Fusion
* **purestorage.fusion.fusion_ra** : Manage role assignments in Pure Storage Fusion
* **purestorage.fusion.fusion_region** : Manage Regions in Pure Storage Fusion
* **purestorage.fusion.fusion_sc** : Manage storage classes in Pure Storage Fusion
* **purestorage.fusion.fusion_ss** : Manage storage services in Pure Storage Fusion
* **purestorage.fusion.fusion_tenant** : Manage tenants in Pure Storage Fusion
* **purestorage.fusion.fusion_tn** : Manage tenant networks in Pure Storage Fusion
* **purestorage.fusion.fusion_ts** : Manage tenant spaces in Pure Storage Fusion
* **purestorage.fusion.fusion_volume** : Manage volumes in Pure Storage Fusion

## `sensu.sensu_go` collection

* **sensu.sensu_go.ad_auth_provider** : Manage Sensu AD authentication provider
* **sensu.sensu_go.asset** : Manage Sensu assets
* **sensu.sensu_go.asset_info** : List Sensu assets
* **sensu.sensu_go.auth_provider_info** : List Sensu authentication providers
* **sensu.sensu_go.bonsai_asset** : Add Sensu assets from Bonsai
* **sensu.sensu_go.check** : Manage Sensu checks
* **sensu.sensu_go.check_info** : List Sensu checks
* **sensu.sensu_go.cluster** : Manage Sensu Go clusters
* **sensu.sensu_go.cluster_info** : List available Sensu Go clusters
* **sensu.sensu_go.cluster_role** : Manage Sensu cluster roles
* **sensu.sensu_go.cluster_role_binding** : Manage Sensu cluster role bindings
* **sensu.sensu_go.cluster_role_binding_info** : List Sensu cluster role bindings
* **sensu.sensu_go.cluster_role_info** : List Sensu cluster roles
* **sensu.sensu_go.datastore** : Manage Sensu external datastore providers
* **sensu.sensu_go.datastore_info** : List external Sensu datastore providers
* **sensu.sensu_go.entity** : Manage Sensu entities
* **sensu.sensu_go.entity_info** : List Sensu entities
* **sensu.sensu_go.etcd_replicator** : Manage Sensu Go etcd replicators
* **sensu.sensu_go.etcd_replicator_info** : List available Sensu Go etcd replicators
* **sensu.sensu_go.event** : Manage Sensu events
* **sensu.sensu_go.event_info** : List Sensu events
* **sensu.sensu_go.filter** : Manage Sensu filters
* **sensu.sensu_go.filter_info** : List Sensu info
* **sensu.sensu_go.handler_info** : List Sensu handlers
* **sensu.sensu_go.handler_set** : Manage Sensu handler set
* **sensu.sensu_go.hook** : Manage Sensu hooks
* **sensu.sensu_go.hook_info** : List Sensu hooks
* **sensu.sensu_go.ldap_auth_provider** : Manage Sensu LDAP authentication provider
* **sensu.sensu_go.mutator** : Manage Sensu mutators
* **sensu.sensu_go.mutator_info** : List Sensu mutators
* **sensu.sensu_go.namespace** : Manage Sensu namespaces
* **sensu.sensu_go.namespace_info** : List Sensu namespaces
* **sensu.sensu_go.oidc_auth_provider** : Manage Sensu OIDC authentication provider
* **sensu.sensu_go.pipe_handler** : Manage Sensu pipe handler
* **sensu.sensu_go.role** : Manage Sensu roles
* **sensu.sensu_go.role_binding** : Manage Sensu role bindings
* **sensu.sensu_go.role_binding_info** : List Sensu role bindings
* **sensu.sensu_go.role_info** : List Sensu roles
* **sensu.sensu_go.secret** : Manage Sensu Go secrets
* **sensu.sensu_go.secret_info** : List available Sensu Go secrets
* **sensu.sensu_go.secrets_provider_env** : Manage Sensu Env secrets provider
* **sensu.sensu_go.secrets_provider_info** : List Sensu secrets providers
* **sensu.sensu_go.secrets_provider_vault** : Manage Sensu VaultProvider secrets providers
* **sensu.sensu_go.silence** : Manage Sensu silences
* **sensu.sensu_go.silence_info** : List Sensu silence entries
* **sensu.sensu_go.socket_handler** : Manage Sensu TCP/UDP handler
* **sensu.sensu_go.tessen** : Manage Sensu&#39;s Tessen configuration
* **sensu.sensu_go.user** : Manage Sensu users
* **sensu.sensu_go.user_info** : List Sensu users

## `splunk.es` collection

* **splunk.es.correlation_search_info** : Manage Splunk Enterprise Security Correlation Searches
* **splunk.es.splunk_adaptive_response_notable_events** : Manage Adaptive Responses notable events resource module
* **splunk.es.splunk_correlation_searches** : Splunk Enterprise Security Correlation searches resource module
* **splunk.es.splunk_data_inputs_monitor** : Splunk Data Inputs of type Monitor resource module
* **splunk.es.splunk_data_inputs_network** : Manage Splunk Data Inputs of type TCP or UDP resource module

## `t_systems_mms.icinga_director` collection

* **t_systems_mms.icinga_director.icinga_command** : Manage commands in Icinga2
* **t_systems_mms.icinga_director.icinga_command_info** : Query commands in Icinga2
* **t_systems_mms.icinga_director.icinga_command_template** : Manage command templates in Icinga2
* **t_systems_mms.icinga_director.icinga_command_template_info** : Query command templates in Icinga2
* **t_systems_mms.icinga_director.icinga_endpoint** : Manage endpoints in Icinga2
* **t_systems_mms.icinga_director.icinga_endpoint_info** : Query endpoints in Icinga2
* **t_systems_mms.icinga_director.icinga_host** : Manage hosts in Icinga2
* **t_systems_mms.icinga_director.icinga_host_info** : Query hosts in Icinga2
* **t_systems_mms.icinga_director.icinga_host_template** : Manage host templates in Icinga2
* **t_systems_mms.icinga_director.icinga_host_template_info** : Query host templates in Icinga2
* **t_systems_mms.icinga_director.icinga_hostgroup** : Manage hostgroups in Icinga2
* **t_systems_mms.icinga_director.icinga_hostgroup_info** : Query hostgroups in Icinga2
* **t_systems_mms.icinga_director.icinga_notification** : Manage notifications in Icinga2
* **t_systems_mms.icinga_director.icinga_notification_info** : Query notifications in Icinga2
* **t_systems_mms.icinga_director.icinga_notification_template** : Manage notification templates in Icinga2
* **t_systems_mms.icinga_director.icinga_notification_template_info** : Query notification templates in Icinga2
* **t_systems_mms.icinga_director.icinga_scheduled_downtime** : Manage downtimes in Icinga2
* **t_systems_mms.icinga_director.icinga_service** : Manage services in Icinga2
* **t_systems_mms.icinga_director.icinga_service_apply** : Manage service apply rules in Icinga2
* **t_systems_mms.icinga_director.icinga_service_apply_info** : Query service apply rules in Icinga2
* **t_systems_mms.icinga_director.icinga_service_info** : Query services in Icinga2
* **t_systems_mms.icinga_director.icinga_service_template** : Manage service templates in Icinga2
* **t_systems_mms.icinga_director.icinga_service_template_info** : Query service templates in Icinga2
* **t_systems_mms.icinga_director.icinga_servicegroup** : Manage servicegroups in Icinga2
* **t_systems_mms.icinga_director.icinga_servicegroup_info** : Query servicegroups in Icinga2
* **t_systems_mms.icinga_director.icinga_serviceset** : Manage servicesets in Icinga2
* **t_systems_mms.icinga_director.icinga_timeperiod** : Manage timeperiods in Icinga2
* **t_systems_mms.icinga_director.icinga_timeperiod_info** : Query timeperiods in Icinga2
* **t_systems_mms.icinga_director.icinga_timeperiod_template** : Manage timeperiod templates in Icinga2
* **t_systems_mms.icinga_director.icinga_timeperiod_template_info** : Query timeperiod templates in Icinga2
* **t_systems_mms.icinga_director.icinga_user** : Manage users in Icinga2
* **t_systems_mms.icinga_director.icinga_user_group** : Manage users groups in Icinga2
* **t_systems_mms.icinga_director.icinga_user_group_info** : Query user groups in Icinga2
* **t_systems_mms.icinga_director.icinga_user_info** : Query users in Icinga2
* **t_systems_mms.icinga_director.icinga_user_template** : Manage user templates in Icinga2
* **t_systems_mms.icinga_director.icinga_user_template_info** : Query user templates in Icinga2
* **t_systems_mms.icinga_director.icinga_zone** : Manage zones in Icinga2
* **t_systems_mms.icinga_director.icinga_zone_info** : Query zones in Icinga2

## `theforeman.foreman` collection

* **theforeman.foreman.activation_key** : Manage Activation Keys
* **theforeman.foreman.architecture** : Manage Architectures
* **theforeman.foreman.auth_source_ldap** : Manage LDAP Authentication Sources
* **theforeman.foreman.bookmark** : Manage Bookmarks
* **theforeman.foreman.compute_attribute** : Manage Compute Attributes
* **theforeman.foreman.compute_profile** : Manage Compute Profiles
* **theforeman.foreman.compute_resource** : Manage Compute Resources
* **theforeman.foreman.config_group** : Manage (Puppet) Config Groups
* **theforeman.foreman.content_credential** : Manage Content Credentials
* **theforeman.foreman.content_export_info** : List content exports
* **theforeman.foreman.content_export_library** : Manage library content exports
* **theforeman.foreman.content_export_repository** : Manage repository content exports
* **theforeman.foreman.content_export_version** : Manage content view version content exports
* **theforeman.foreman.content_upload** : Upload content to a repository
* **theforeman.foreman.content_view** : Manage Content Views
* **theforeman.foreman.content_view_filter** : Manage Content View Filters
* **theforeman.foreman.content_view_filter_info** : Fetch information about a Content View Filter
* **theforeman.foreman.content_view_filter_rule** : Manage content view filter rules
* **theforeman.foreman.content_view_filter_rule_info** : Fetch information about a Content View Filter Rule
* **theforeman.foreman.content_view_version_info** : Fetch information about Content Views
* **theforeman.foreman.content_view_version** : Manage Content View Versions
* **theforeman.foreman.discovery_rule** : Manage Host Discovery Rules
* **theforeman.foreman.domain** : Manage Domains
* **theforeman.foreman.domain_info** : Fetch information about Domains
* **theforeman.foreman.external_usergroup** : Manage External User Groups
* **theforeman.foreman.global_parameter** : Manage Global Parameters
* **theforeman.foreman.hardware_model** : Manage Hardware Models
* **theforeman.foreman.host** : Manage Hosts
* **theforeman.foreman.host_collection** : Manage Host Collections
* **theforeman.foreman.host_errata_info** : Fetch information about Host Errata
* **theforeman.foreman.host_info** : Fetch information about Hosts
* **theforeman.foreman.host_power** : Manage Power State of Hosts
* **theforeman.foreman.hostgroup** : Manage Hostgroups
* **theforeman.foreman.hostgroup_info** : Get information about hostgroup(s)
* **theforeman.foreman.http_proxy** : Manage HTTP Proxies
* **theforeman.foreman.image** : Manage Images
* **theforeman.foreman.installation_medium** : Manage Installation Media
* **theforeman.foreman.job_invocation** : Invoke Remote Execution Jobs
* **theforeman.foreman.job_template** : Manage Job Templates
* **theforeman.foreman.lifecycle_environment** : Manage Lifecycle Environments
* **theforeman.foreman.location** : Manage Locations
* **theforeman.foreman.operatingsystem** : Manage Operating Systems
* **theforeman.foreman.organization** : Manage Organizations
* **theforeman.foreman.organization_info** : Get information about organization(s)
* **theforeman.foreman.os_default_template** : Manage Default Template Associations To Operating Systems
* **theforeman.foreman.partition_table** : Manage Partition Table Templates
* **theforeman.foreman.product** : Manage Products
* **theforeman.foreman.provisioning_template** : Manage Provisioning Templates
* **theforeman.foreman.puppet_environment** : Manage Puppet Environments
* **theforeman.foreman.puppetclasses_import** : Import Puppet Classes from a Proxy
* **theforeman.foreman.realm** : Manage Realms
* **theforeman.foreman.redhat_manifest** : Interact with a Red Hat Satellite Subscription Manifest
* **theforeman.foreman.repository** : Manage Repositories
* **theforeman.foreman.repository_info** : Fetch information about Repositories
* **theforeman.foreman.repository_set** : Enable/disable Red Hat Repositories available through subscriptions
* **theforeman.foreman.repository_set_info** : Fetch information about Red Hat Repositories
* **theforeman.foreman.repository_sync** : Sync a Repository or Product
* **theforeman.foreman.resource_info** : Gather information about resources
* **theforeman.foreman.role** : Manage Roles
* **theforeman.foreman.scap_content** : Manage SCAP content
* **theforeman.foreman.scap_tailoring_file** : Manage SCAP Tailoring Files
* **theforeman.foreman.scc_account** : Manage SUSE Customer Center Accounts
* **theforeman.foreman.scc_product** : Subscribe SUSE Customer Center Account Products
* **theforeman.foreman.setting** : Manage Settings
* **theforeman.foreman.setting_info** : Fetch information about Settings
* **theforeman.foreman.smart_class_parameter** : Manage Smart Class Parameters
* **theforeman.foreman.smart_proxy** : Manage Smart Proxies
* **theforeman.foreman.snapshot** : Manage Snapshots
* **theforeman.foreman.snapshot_info** : Fetch information about Foreman Snapshots
* **theforeman.foreman.status_info** : Get status info
* **theforeman.foreman.subnet** : Manage Subnets
* **theforeman.foreman.subnet_info** : Fetch information about Subnets
* **theforeman.foreman.subscription_info** : Fetch information about Subscriptions
* **theforeman.foreman.subscription_manifest** : Manage Subscription Manifests
* **theforeman.foreman.sync_plan** : Manage Sync Plans
* **theforeman.foreman.templates_import** : Sync Templates from a repository
* **theforeman.foreman.user** : Manage Users
* **theforeman.foreman.usergroup** : Manage User Groups

## `vmware.vmware_rest` collection

* **vmware.vmware_rest.appliance_access_consolecli** : Set enabled state of the console-based controlled CLI (TTY1).
* **vmware.vmware_rest.appliance_access_consolecli_info** : Get enabled state of the console-based controlled CLI (TTY1).
* **vmware.vmware_rest.appliance_access_dcui** : Set enabled state of Direct Console User Interface (DCUI TTY2).
* **vmware.vmware_rest.appliance_access_dcui_info** : Get enabled state of Direct Console User Interface (DCUI TTY2).
* **vmware.vmware_rest.appliance_access_shell** : Set enabled state of BASH, that is, access to BASH from within the controlled CLI.
* **vmware.vmware_rest.appliance_access_shell_info** : Get enabled state of BASH, that is, access to BASH from within the controlled CLI.
* **vmware.vmware_rest.appliance_access_ssh** : Set enabled state of the SSH-based controlled CLI.
* **vmware.vmware_rest.appliance_access_ssh_info** : Get enabled state of the SSH-based controlled CLI.
* **vmware.vmware_rest.appliance_health_applmgmt_info** : Get health status of applmgmt services.
* **vmware.vmware_rest.appliance_health_database_info** : Returns the health status of the database.
* **vmware.vmware_rest.appliance_health_databasestorage_info** : Get database storage health.
* **vmware.vmware_rest.appliance_health_load_info** : Get load health.
* **vmware.vmware_rest.appliance_health_mem_info** : Get memory health.
* **vmware.vmware_rest.appliance_health_softwarepackages_info** : Get information on available software updates available in the remote vSphere Update Manager repository
* **vmware.vmware_rest.appliance_health_storage_info** : Get storage health.
* **vmware.vmware_rest.appliance_health_swap_info** : Get swap health.
* **vmware.vmware_rest.appliance_health_system_info** : Get overall health of system.
* **vmware.vmware_rest.appliance_infraprofile_configs** : Exports the desired profile specification.
* **vmware.vmware_rest.appliance_infraprofile_configs_info** : List all the profiles which are registered.
* **vmware.vmware_rest.appliance_localaccounts_globalpolicy** : Set the global password policy.
* **vmware.vmware_rest.appliance_localaccounts_globalpolicy_info** : Get the global password policy.
* **vmware.vmware_rest.appliance_localaccounts_info** : Get the local user account information.
* **vmware.vmware_rest.appliance_monitoring_info** : Get monitored item info
* **vmware.vmware_rest.appliance_monitoring_query** : Get monitoring data.
* **vmware.vmware_rest.appliance_networking** : Reset and restarts network configuration on all interfaces, also this will renew the DHCP lease for DHCP IP address.
* **vmware.vmware_rest.appliance_networking_dns_domains** : Set DNS search domains.
* **vmware.vmware_rest.appliance_networking_dns_domains_info** : Get list of DNS search domains.
* **vmware.vmware_rest.appliance_networking_dns_hostname** : Set the Fully Qualified Domain Name.
* **vmware.vmware_rest.appliance_networking_dns_hostname_info** : Get the Fully Qualified Doman Name.
* **vmware.vmware_rest.appliance_networking_dns_servers** : Set the DNS server configuration
* **vmware.vmware_rest.appliance_networking_dns_servers_info** : Get DNS server configuration.
* **vmware.vmware_rest.appliance_networking_firewall_inbound** : Set the ordered list of firewall rules to allow or deny traffic from one or more incoming IP addresses
* **vmware.vmware_rest.appliance_networking_firewall_inbound_info** : Get the ordered list of firewall rules
* **vmware.vmware_rest.appliance_networking_info** : Get Networking information for all configured interfaces.
* **vmware.vmware_rest.appliance_networking_interfaces_info** : Get information about a particular network interface.
* **vmware.vmware_rest.appliance_networking_interfaces_ipv4** : Set IPv4 network configuration for specific network interface.
* **vmware.vmware_rest.appliance_networking_interfaces_ipv4_info** : Get IPv4 network configuration for specific NIC.
* **vmware.vmware_rest.appliance_networking_interfaces_ipv6** : Set IPv6 network configuration for specific interface.
* **vmware.vmware_rest.appliance_networking_interfaces_ipv6_info** : Get IPv6 network configuration for specific interface.
* **vmware.vmware_rest.appliance_networking_noproxy** : Sets servers for which no proxy configuration should be applied
* **vmware.vmware_rest.appliance_networking_noproxy_info** : Returns servers for which no proxy configuration will be applied.
* **vmware.vmware_rest.appliance_networking_proxy** : Configures which proxy server to use for the specified protocol
* **vmware.vmware_rest.appliance_networking_proxy_info** : Gets the proxy configuration for a specific protocol.
* **vmware.vmware_rest.appliance_ntp** : Set NTP servers
* **vmware.vmware_rest.appliance_ntp_info** : Get the NTP configuration status
* **vmware.vmware_rest.appliance_services** : Restarts a service
* **vmware.vmware_rest.appliance_vmon_service_info** : Returns the state of a service.
* **vmware.vmware_rest.appliance_shutdown** : Cancel pending shutdown action.
* **vmware.vmware_rest.appliance_shutdown_info** : Get details about the pending shutdown action.
* **vmware.vmware_rest.appliance_system_globalfips** : Enable/Disable Global FIPS mode for the appliance
* **vmware.vmware_rest.appliance_system_globalfips_info** : Get current appliance FIPS settings.
* **vmware.vmware_rest.appliance_system_storage** : Resize all partitions to 100 percent of disk size.
* **vmware.vmware_rest.appliance_system_storage_info** : Get disk to partition mapping.
* **vmware.vmware_rest.appliance_system_time_info** : Get system time.
* **vmware.vmware_rest.appliance_system_time_timezone** : Set time zone.
* **vmware.vmware_rest.appliance_system_time_timezone_info** : Get time zone.
* **vmware.vmware_rest.appliance_system_version_info** : Get the version.
* **vmware.vmware_rest.appliance_timesync** : Set time synchronization mode.
* **vmware.vmware_rest.appliance_timesync_info** : Get time synchronization mode.
* **vmware.vmware_rest.appliance_update_info** : Gets the current status of the appliance update.
* **vmware.vmware_rest.appliance_vmon_service** : Lists details of services managed by vMon.
* **vmware.vmware_rest.content_configuration** : Updates the configuration
* **vmware.vmware_rest.content_configuration_info** : Retrieves the current configuration values.
* **vmware.vmware_rest.content_library_item_info** : Returns the {@link ItemModel} with the given identifier.
* **vmware.vmware_rest.content_locallibrary** : Creates a new local library.
* **vmware.vmware_rest.content_locallibrary_info** : Returns a given local library.
* **vmware.vmware_rest.content_subscribedlibrary** : Creates a new subscribed library
* **vmware.vmware_rest.content_subscribedlibrary_info** : Returns a given subscribed library.
* **vmware.vmware_rest.vcenter_cluster_info** : Retrieves information about the cluster corresponding to {@param.name cluster}.
* **vmware.vmware_rest.vcenter_datacenter** : Create a new datacenter in the vCenter inventory
* **vmware.vmware_rest.vcenter_datacenter_info** : Retrieves information about the datacenter corresponding to {@param.name datacenter}.
* **vmware.vmware_rest.vcenter_datastore_info** : Retrieves information about the datastore indicated by {@param.name datastore}.
* **vmware.vmware_rest.vcenter_folder_info** : Returns information about at most 1000 visible (subject to permission checks) folders in vCenter matching the {@link FilterSpec}.
* **vmware.vmware_rest.vcenter_host** : Add a new standalone host in the vCenter inventory
* **vmware.vmware_rest.vcenter_host_info** : Returns information about at most 2500 visible (subject to permission checks) hosts in vCenter matching the {@link FilterSpec}.
* **vmware.vmware_rest.vcenter_network_info** : Returns information about at most 1000 visible (subject to permission checks) networks in vCenter matching the {@link FilterSpec}.
* **vmware.vmware_rest.vcenter_ovf_libraryitem** : Creates a library item in content library from a virtual machine or virtual appliance
* **vmware.vmware_rest.vcenter_resourcepool** : Creates a resource pool.
* **vmware.vmware_rest.vcenter_resourcepool_info** : Retrieves information about the resource pool indicated by {@param.name resourcePool}.
* **vmware.vmware_rest.vcenter_storage_policies_info** : Returns information about at most 1024 visible (subject to permission checks) storage solicies availabe in vCenter
* **vmware.vmware_rest.vcenter_vm** : Creates a virtual machine.
* **vmware.vmware_rest.vcenter_vm_guest_customization** : Applies a customization specification on the virtual machine
* **vmware.vmware_rest.vcenter_vm_guest_filesystem_directories** : Creates a directory in the guest operating system
* **vmware.vmware_rest.vcenter_vm_guest_identity_info** : Return information about the guest.
* **vmware.vmware_rest.vcenter_vm_guest_localfilesystem_info** : Returns details of the local file systems in the guest operating system.
* **vmware.vmware_rest.vcenter_vm_guest_networking_info** : Returns information about the network configuration in the guest operating system.
* **vmware.vmware_rest.vcenter_vm_guest_networking_interfaces_info** : Returns information about the networking interfaces in the guest operating system.
* **vmware.vmware_rest.vcenter_vm_guest_networking_routes_info** : Returns information about network routing in the guest operating system.
* **vmware.vmware_rest.vcenter_vm_guest_operations_info** : Get information about the guest operation status.
* **vmware.vmware_rest.vcenter_vm_guest_power** : Issues a request to the guest operating system asking it to perform a soft shutdown, standby (suspend) or soft reboot
* **vmware.vmware_rest.vcenter_vm_guest_power_info** : Returns information about the guest operating system power state.
* **vmware.vmware_rest.vcenter_vm_hardware** : Updates the virtual hardware settings of a virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_adapter_sata** : Adds a virtual SATA adapter to the virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_adapter_sata_info** : Returns information about a virtual SATA adapter.
* **vmware.vmware_rest.vcenter_vm_hardware_adapter_scsi** : Adds a virtual SCSI adapter to the virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_adapter_scsi_info** : Returns information about a virtual SCSI adapter.
* **vmware.vmware_rest.vcenter_vm_hardware_boot** : Updates the boot-related settings of a virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_boot_device** : Sets the virtual devices that will be used to boot the virtual machine
* **vmware.vmware_rest.vcenter_vm_hardware_boot_device_info** : Returns an ordered list of boot devices for the virtual machine
* **vmware.vmware_rest.vcenter_vm_hardware_boot_info** : Returns the boot-related settings of a virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_cdrom** : Adds a virtual CD-ROM device to the virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_cdrom_info** : Returns information about a virtual CD-ROM device.
* **vmware.vmware_rest.vcenter_vm_hardware_cpu** : Updates the CPU-related settings of a virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_cpu_info** : Returns the CPU-related settings of a virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_disk** : Adds a virtual disk to the virtual machine
* **vmware.vmware_rest.vcenter_vm_hardware_disk_info** : Returns information about a virtual disk.
* **vmware.vmware_rest.vcenter_vm_hardware_ethernet** : Adds a virtual Ethernet adapter to the virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_ethernet_info** : Returns information about a virtual Ethernet adapter.
* **vmware.vmware_rest.vcenter_vm_hardware_floppy** : Adds a virtual floppy drive to the virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_floppy_info** : Returns information about a virtual floppy drive.
* **vmware.vmware_rest.vcenter_vm_hardware_info** : Returns the virtual hardware settings of a virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_memory** : Updates the memory-related settings of a virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_memory_info** : Returns the memory-related settings of a virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_parallel** : Adds a virtual parallel port to the virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_parallel_info** : Returns information about a virtual parallel port.
* **vmware.vmware_rest.vcenter_vm_hardware_serial** : Adds a virtual serial port to the virtual machine.
* **vmware.vmware_rest.vcenter_vm_hardware_serial_info** : Returns information about a virtual serial port.
* **vmware.vmware_rest.vcenter_vm_info** : Returns information about a virtual machine.
* **vmware.vmware_rest.vcenter_vm_libraryitem_info** : Returns the information about the library item associated with the virtual machine.
* **vmware.vmware_rest.vcenter_vm_power** : Operate a boot, hard shutdown, hard reset or hard suspend on a guest.
* **vmware.vmware_rest.vcenter_vm_power_info** : Returns the power state information of a virtual machine.
* **vmware.vmware_rest.vcenter_vm_storage_policy** : Updates the storage policy configuration of a virtual machine and/or its associated virtual hard disks.
* **vmware.vmware_rest.vcenter_vm_storage_policy_compliance** : Returns the storage policy Compliance {@link Info} of a virtual machine after explicitly re-computing compliance check.
* **vmware.vmware_rest.vcenter_vm_storage_policy_compliance_info** : Returns the cached storage policy compliance information of a virtual machine.
* **vmware.vmware_rest.vcenter_vm_storage_policy_info** : Returns Information about Storage Policy associated with a virtual machine&#39;s home directory and/or its virtual hard disks.
* **vmware.vmware_rest.vcenter_vm_tools** : Update the properties of VMware Tools.
* **vmware.vmware_rest.vcenter_vm_tools_info** : Get the properties of VMware Tools.
* **vmware.vmware_rest.vcenter_vm_tools_installer** : Connects the VMware Tools CD installer as a CD-ROM for the guest operating system
* **vmware.vmware_rest.vcenter_vm_tools_installer_info** : Get information about the VMware Tools installer.
* **vmware.vmware_rest.vcenter_vmtemplate_libraryitems** : Creates a library item in content library from a virtual machine
* **vmware.vmware_rest.vcenter_vmtemplate_libraryitems_info** : Returns information about a virtual machine template contained in the library item specified by {@param.name templateLibraryItem}

## `vultr.cloud` collection

* **vultr.cloud.account_info** : Get information about the Vultr account
* **vultr.cloud.block_storage** : Manages block storage volumes on Vultr
* **vultr.cloud.block_storage_info** : Get information about the Vultr block storage
* **vultr.cloud.dns_domain** : Manages DNS domains on Vultr
* **vultr.cloud.dns_domain_info** : Gather information about the Vultr DNS domains
* **vultr.cloud.dns_record** : Manages DNS records on Vultr
* **vultr.cloud.firewall_group** : Manages firewall groups on Vultr
* **vultr.cloud.firewall_group_info** : Gather information about the Vultr firewall groups
* **vultr.cloud.firewall_rule** : Manages firewall rules on Vultr
* **vultr.cloud.firewall_rule_info** : Gather information about the Vultr firewall rules
* **vultr.cloud.instance** : Manages server instances on Vultr.
* **vultr.cloud.instance_info** : Get information about the Vultr instances
* **vultr.cloud.os_info** : Get information about the Vultr operation systems
* **vultr.cloud.plan_info** : Gather information about the Vultr plans
* **vultr.cloud.plan_metal_info** : Gather information about the Vultr bare metal plans
* **vultr.cloud.region_info** : Gather information about the Vultr regions
* **vultr.cloud.reserved_ip** : Manages reserved IPs on Vultr
* **vultr.cloud.snapshot** : Manages snapshots on Vultr
* **vultr.cloud.snapshot_info** : Gather information about the Vultr snapshots
* **vultr.cloud.ssh_key** : Manages ssh keys on Vultr.
* **vultr.cloud.ssh_key_info** : Get information about the Vultr SSH keys
* **vultr.cloud.startup_script** : Manages startup scripts on Vultr
* **vultr.cloud.startup_script_info** : Gather information about the Vultr startup scripts
* **vultr.cloud.user** : Manages users on Vultr
* **vultr.cloud.user_info** : Get information about the Vultr users
* **vultr.cloud.vpc** : Manages VPCs on Vultr
* **vultr.cloud.vpc_info** : Gather information about the Vultr VPCs

## `vyos.vyos` collection

* **vyos.vyos.vyos_banner** : Manage multiline banners on VyOS devices
* **vyos.vyos.vyos_bgp_address_family** : BGP Address Family Resource Module.
* **vyos.vyos.vyos_bgp_global** : BGP Global Resource Module.
* **vyos.vyos.vyos_command** : Run one or more commands on VyOS devices
* **vyos.vyos.vyos_config** : Manage VyOS configuration on remote device
* **vyos.vyos.vyos_facts** : Get facts about vyos devices.
* **vyos.vyos.vyos_firewall_global** : FIREWALL global resource module
* **vyos.vyos.vyos_firewall_interfaces** : FIREWALL interfaces resource module
* **vyos.vyos.vyos_firewall_rules** : FIREWALL rules resource module
* **vyos.vyos.vyos_hostname** : Manages hostname resource module
* **vyos.vyos.vyos_interfaces** : Interfaces resource module
* **vyos.vyos.vyos_l3_interfaces** : L3 interfaces resource module
* **vyos.vyos.vyos_lag_interfaces** : LAG interfaces resource module
* **vyos.vyos.vyos_lldp_global** : LLDP global resource module
* **vyos.vyos.vyos_lldp_interfaces** : LLDP interfaces resource module
* **vyos.vyos.vyos_logging_global** : Logging resource module
* **vyos.vyos.vyos_ntp_global** : Manages ntp modules of Vyos network devices
* **vyos.vyos.vyos_ospf_interfaces** : OSPF Interfaces Resource Module.
* **vyos.vyos.vyos_ospfv2** : OSPFv2 resource module
* **vyos.vyos.vyos_ospfv3** : OSPFV3 resource module
* **vyos.vyos.vyos_ping** : Tests reachability using ping from VyOS network devices
* **vyos.vyos.vyos_prefix_lists** : Prefix-Lists resource module for VyOS
* **vyos.vyos.vyos_route_maps** : Route Map Resource Module.
* **vyos.vyos.vyos_snmp_server** : Manages snmp_server resource module
* **vyos.vyos.vyos_static_routes** : Static routes resource module
* **vyos.vyos.vyos_system** : Run `set system` commands on VyOS devices
* **vyos.vyos.vyos_user** : Manage the collection of local users on VyOS device
* **vyos.vyos.vyos_vlan** : Manage VLANs on VyOS network devices

## `wti.remote` collection

* **wti.remote.cpm_alarm_info** : Get alarm information from WTI OOB and PDU devices
* **wti.remote.cpm_config_backup** : Get parameters from WTI OOB and PDU devices
* **wti.remote.cpm_config_restore** : Send operational parameters to WTI OOB and PDU devices
* **wti.remote.cpm_current_info** : Get the Current Information of a WTI device
* **wti.remote.cpm_firmware_info** : Get firmware information from WTI OOB and PDU devices
* **wti.remote.cpm_serial_port_config** : Set Serial port parameters in WTI OOB and PDU devices
* **wti.remote.cpm_hostname_config** : Set Hostname (Site ID), Location, Asset Tag parameters in WTI OOB and PDU devices.
* **wti.remote.cpm_hostname_info** : Get Hostname (Site ID), Location, Asset Tag parameters in WTI OOB and PDU devices
* **wti.remote.cpm_interface_config** : Set network interface parameters in WTI OOB and PDU devices
* **wti.remote.cpm_interface_info** : Get network interface parameters from WTI OOB and PDU devices
* **wti.remote.cpm_snmp_config** : Set network IPTables parameters in WTI OOB and PDU devices
* **wti.remote.cpm_iptables_info** : Get network IPTABLES parameters from WTI OOB and PDU devices
* **wti.remote.cpm_plugconfig** : Get and Set Plug Parameters on WTI OOB and PDU power devices
* **wti.remote.cpm_plugcontrol** : Get and Set Plug actions on WTI OOB and PDU power devices
* **wti.remote.cpm_power_info** : Get the Power Information of a WTI device
* **wti.remote.cpm_serial_port_action_info** : Get Serial port connection status in WTI OOB and PDU devices
* **wti.remote.cpm_serial_port_action_set** : Set Serial port connection/disconnection commands in WTI OOB and PDU devices
* **wti.remote.cpm_serial_port_info** : Get Serial port parameters in WTI OOB and PDU devices
* **wti.remote.cpm_snmp_info** : Get network SNMP parameters from WTI OOB and PDU devices
* **wti.remote.cpm_status_info** : Get general status information from WTI OOB and PDU devices
* **wti.remote.cpm_syslog_client_config** : Set network SYSLOG Client parameters in WTI OOB and PDU devices
* **wti.remote.cpm_syslog_client_info** : Get network SYSLOG Client parameters from WTI OOB and PDU devices
* **wti.remote.cpm_syslog_server_config** : Set network SYSLOG Server parameters in WTI OOB and PDU devices
* **wti.remote.cpm_syslog_server_info** : Get network SYSLOG Server parameters from WTI OOB and PDU devices
* **wti.remote.cpm_temp_info** : Get temperature information from WTI OOB and PDU devices
* **wti.remote.cpm_time_config** : Set Time/Date parameters in WTI OOB and PDU devices.
* **wti.remote.cpm_time_info** : Get Time/Date parameters in WTI OOB and PDU devices
* **wti.remote.cpm_user** : Get various status and parameters from WTI OOB and PDU devices

