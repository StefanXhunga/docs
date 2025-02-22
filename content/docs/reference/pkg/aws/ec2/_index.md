---
title: "ec2"
title_tag: "aws.ec2"
meta_desc: "Explore the resources and functions of the aws.ec2 module."
---

<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Explore the resources and functions of the aws.ec2 module.

<h2 id="resources">Resources</h2>
<ul class="api">
    <li><a href="ami" title="Ami"><span class="symbol resource"></span>Ami</a></li>
    <li><a href="amicopy" title="AmiCopy"><span class="symbol resource"></span>AmiCopy</a></li>
    <li><a href="amifrominstance" title="AmiFromInstance"><span class="symbol resource"></span>AmiFromInstance</a></li>
    <li><a href="amilaunchpermission" title="AmiLaunchPermission"><span class="symbol resource"></span>AmiLaunchPermission</a></li>
    <li><a href="availabilityzonegroup" title="AvailabilityZoneGroup"><span class="symbol resource"></span>AvailabilityZoneGroup</a></li>
    <li><a href="capacityreservation" title="CapacityReservation"><span class="symbol resource"></span>CapacityReservation</a></li>
    <li><a href="carriergateway" title="CarrierGateway"><span class="symbol resource"></span>CarrierGateway</a></li>
    <li><a href="customergateway" title="CustomerGateway"><span class="symbol resource"></span>CustomerGateway</a></li>
    <li><a href="dedicatedhost" title="DedicatedHost"><span class="symbol resource"></span>DedicatedHost</a></li>
    <li><a href="defaultnetworkacl" title="DefaultNetworkAcl"><span class="symbol resource"></span>DefaultNetworkAcl</a></li>
    <li><a href="defaultroutetable" title="DefaultRouteTable"><span class="symbol resource"></span>DefaultRouteTable</a></li>
    <li><a href="defaultsecuritygroup" title="DefaultSecurityGroup"><span class="symbol resource"></span>DefaultSecurityGroup</a></li>
    <li><a href="defaultsubnet" title="DefaultSubnet"><span class="symbol resource"></span>DefaultSubnet</a></li>
    <li><a href="defaultvpc" title="DefaultVpc"><span class="symbol resource"></span>DefaultVpc</a></li>
    <li><a href="defaultvpcdhcpoptions" title="DefaultVpcDhcpOptions"><span class="symbol resource"></span>DefaultVpcDhcpOptions</a></li>
    <li><a href="egressonlyinternetgateway" title="EgressOnlyInternetGateway"><span class="symbol resource"></span>EgressOnlyInternetGateway</a></li>
    <li><a href="eip" title="Eip"><span class="symbol resource"></span>Eip</a></li>
    <li><a href="eipassociation" title="EipAssociation"><span class="symbol resource"></span>EipAssociation</a></li>
    <li><a href="fleet" title="Fleet"><span class="symbol resource"></span>Fleet</a></li>
    <li><a href="flowlog" title="FlowLog"><span class="symbol resource"></span>FlowLog</a></li>
    <li><a href="instance" title="Instance"><span class="symbol resource"></span>Instance</a></li>
    <li><a href="internetgateway" title="InternetGateway"><span class="symbol resource"></span>InternetGateway</a></li>
    <li><a href="keypair" title="KeyPair"><span class="symbol resource"></span>KeyPair</a></li>
    <li><a href="launchconfiguration" title="LaunchConfiguration"><span class="symbol resource"></span>LaunchConfiguration</a></li>
    <li><a href="launchtemplate" title="LaunchTemplate"><span class="symbol resource"></span>LaunchTemplate</a></li>
    <li><a href="localgatewayroute" title="LocalGatewayRoute"><span class="symbol resource"></span>LocalGatewayRoute</a></li>
    <li><a href="localgatewayroutetablevpcassociation" title="LocalGatewayRouteTableVpcAssociation"><span class="symbol resource"></span>LocalGatewayRouteTableVpcAssociation</a></li>
    <li><a href="mainroutetableassociation" title="MainRouteTableAssociation"><span class="symbol resource"></span>MainRouteTableAssociation</a></li>
    <li><a href="managedprefixlist" title="ManagedPrefixList"><span class="symbol resource"></span>ManagedPrefixList</a></li>
    <li><a href="natgateway" title="NatGateway"><span class="symbol resource"></span>NatGateway</a></li>
    <li><a href="networkacl" title="NetworkAcl"><span class="symbol resource"></span>NetworkAcl</a></li>
    <li><a href="networkaclrule" title="NetworkAclRule"><span class="symbol resource"></span>NetworkAclRule</a></li>
    <li><a href="networkinterface" title="NetworkInterface"><span class="symbol resource"></span>NetworkInterface</a></li>
    <li><a href="networkinterfaceattachment" title="NetworkInterfaceAttachment"><span class="symbol resource"></span>NetworkInterfaceAttachment</a></li>
    <li><a href="networkinterfacesecuritygroupattachment" title="NetworkInterfaceSecurityGroupAttachment"><span class="symbol resource"></span>NetworkInterfaceSecurityGroupAttachment</a></li>
    <li><a href="peeringconnectionoptions" title="PeeringConnectionOptions"><span class="symbol resource"></span>PeeringConnectionOptions</a></li>
    <li><a href="placementgroup" title="PlacementGroup"><span class="symbol resource"></span>PlacementGroup</a></li>
    <li><a href="proxyprotocolpolicy" title="ProxyProtocolPolicy"><span class="symbol resource"></span>ProxyProtocolPolicy</a></li>
    <li><a href="route" title="Route"><span class="symbol resource"></span>Route</a></li>
    <li><a href="routetable" title="RouteTable"><span class="symbol resource"></span>RouteTable</a></li>
    <li><a href="routetableassociation" title="RouteTableAssociation"><span class="symbol resource"></span>RouteTableAssociation</a></li>
    <li><a href="securitygroup" title="SecurityGroup"><span class="symbol resource"></span>SecurityGroup</a></li>
    <li><a href="securitygrouprule" title="SecurityGroupRule"><span class="symbol resource"></span>SecurityGroupRule</a></li>
    <li><a href="snapshotcreatevolumepermission" title="SnapshotCreateVolumePermission"><span class="symbol resource"></span>SnapshotCreateVolumePermission</a></li>
    <li><a href="spotdatafeedsubscription" title="SpotDatafeedSubscription"><span class="symbol resource"></span>SpotDatafeedSubscription</a></li>
    <li><a href="spotfleetrequest" title="SpotFleetRequest"><span class="symbol resource"></span>SpotFleetRequest</a></li>
    <li><a href="spotinstancerequest" title="SpotInstanceRequest"><span class="symbol resource"></span>SpotInstanceRequest</a></li>
    <li><a href="subnet" title="Subnet"><span class="symbol resource"></span>Subnet</a></li>
    <li><a href="tag" title="Tag"><span class="symbol resource"></span>Tag</a></li>
    <li><a href="trafficmirrorfilter" title="TrafficMirrorFilter"><span class="symbol resource"></span>TrafficMirrorFilter</a></li>
    <li><a href="trafficmirrorfilterrule" title="TrafficMirrorFilterRule"><span class="symbol resource"></span>TrafficMirrorFilterRule</a></li>
    <li><a href="trafficmirrorsession" title="TrafficMirrorSession"><span class="symbol resource"></span>TrafficMirrorSession</a></li>
    <li><a href="trafficmirrortarget" title="TrafficMirrorTarget"><span class="symbol resource"></span>TrafficMirrorTarget</a></li>
    <li><a href="transitgatewaypeeringattachmentaccepter" title="TransitGatewayPeeringAttachmentAccepter"><span class="symbol resource"></span>TransitGatewayPeeringAttachmentAccepter</a></li>
    <li><a href="volumeattachment" title="VolumeAttachment"><span class="symbol resource"></span>VolumeAttachment</a></li>
    <li><a href="vpc" title="Vpc"><span class="symbol resource"></span>Vpc</a></li>
    <li><a href="vpcdhcpoptions" title="VpcDhcpOptions"><span class="symbol resource"></span>VpcDhcpOptions</a></li>
    <li><a href="vpcdhcpoptionsassociation" title="VpcDhcpOptionsAssociation"><span class="symbol resource"></span>VpcDhcpOptionsAssociation</a></li>
    <li><a href="vpcendpoint" title="VpcEndpoint"><span class="symbol resource"></span>VpcEndpoint</a></li>
    <li><a href="vpcendpointconnectionnotification" title="VpcEndpointConnectionNotification"><span class="symbol resource"></span>VpcEndpointConnectionNotification</a></li>
    <li><a href="vpcendpointroutetableassociation" title="VpcEndpointRouteTableAssociation"><span class="symbol resource"></span>VpcEndpointRouteTableAssociation</a></li>
    <li><a href="vpcendpointservice" title="VpcEndpointService"><span class="symbol resource"></span>VpcEndpointService</a></li>
    <li><a href="vpcendpointserviceallowedprinciple" title="VpcEndpointServiceAllowedPrinciple"><span class="symbol resource"></span>VpcEndpointServiceAllowedPrinciple</a></li>
    <li><a href="vpcendpointsubnetassociation" title="VpcEndpointSubnetAssociation"><span class="symbol resource"></span>VpcEndpointSubnetAssociation</a></li>
    <li><a href="vpcipv4cidrblockassociation" title="VpcIpv4CidrBlockAssociation"><span class="symbol resource"></span>VpcIpv4CidrBlockAssociation</a></li>
    <li><a href="vpcpeeringconnection" title="VpcPeeringConnection"><span class="symbol resource"></span>VpcPeeringConnection</a></li>
    <li><a href="vpcpeeringconnectionaccepter" title="VpcPeeringConnectionAccepter"><span class="symbol resource"></span>VpcPeeringConnectionAccepter</a></li>
    <li><a href="vpnconnection" title="VpnConnection"><span class="symbol resource"></span>VpnConnection</a></li>
    <li><a href="vpnconnectionroute" title="VpnConnectionRoute"><span class="symbol resource"></span>VpnConnectionRoute</a></li>
    <li><a href="vpngateway" title="VpnGateway"><span class="symbol resource"></span>VpnGateway</a></li>
    <li><a href="vpngatewayattachment" title="VpnGatewayAttachment"><span class="symbol resource"></span>VpnGatewayAttachment</a></li>
    <li><a href="vpngatewayroutepropagation" title="VpnGatewayRoutePropagation"><span class="symbol resource"></span>VpnGatewayRoutePropagation</a></li>
</ul>

<h2 id="functions">Functions</h2>
<ul class="api">
    <li><a href="getami" title="GetAmi"><span class="symbol function"></span>GetAmi</a></li>
    <li><a href="getamiids" title="GetAmiIds"><span class="symbol function"></span>GetAmiIds</a></li>
    <li><a href="getcoippool" title="GetCoipPool"><span class="symbol function"></span>GetCoipPool</a></li>
    <li><a href="getcoippools" title="GetCoipPools"><span class="symbol function"></span>GetCoipPools</a></li>
    <li><a href="getcustomergateway" title="GetCustomerGateway"><span class="symbol function"></span>GetCustomerGateway</a></li>
    <li><a href="getdedicatedhost" title="GetDedicatedHost"><span class="symbol function"></span>GetDedicatedHost</a></li>
    <li><a href="getelasticip" title="GetElasticIp"><span class="symbol function"></span>GetElasticIp</a></li>
    <li><a href="getinstance" title="GetInstance"><span class="symbol function"></span>GetInstance</a></li>
    <li><a href="getinstancetype" title="GetInstanceType"><span class="symbol function"></span>GetInstanceType</a></li>
    <li><a href="getinstancetypeoffering" title="GetInstanceTypeOffering"><span class="symbol function"></span>GetInstanceTypeOffering</a></li>
    <li><a href="getinstancetypeofferings" title="GetInstanceTypeOfferings"><span class="symbol function"></span>GetInstanceTypeOfferings</a></li>
    <li><a href="getinstances" title="GetInstances"><span class="symbol function"></span>GetInstances</a></li>
    <li><a href="getinternetgateway" title="GetInternetGateway"><span class="symbol function"></span>GetInternetGateway</a></li>
    <li><a href="getlaunchconfiguration" title="GetLaunchConfiguration"><span class="symbol function"></span>GetLaunchConfiguration</a></li>
    <li><a href="getlaunchtemplate" title="GetLaunchTemplate"><span class="symbol function"></span>GetLaunchTemplate</a></li>
    <li><a href="getlocalgateway" title="GetLocalGateway"><span class="symbol function"></span>GetLocalGateway</a></li>
    <li><a href="getlocalgatewayroutetable" title="GetLocalGatewayRouteTable"><span class="symbol function"></span>GetLocalGatewayRouteTable</a></li>
    <li><a href="getlocalgatewayroutetables" title="GetLocalGatewayRouteTables"><span class="symbol function"></span>GetLocalGatewayRouteTables</a></li>
    <li><a href="getlocalgatewayvirtualinterface" title="GetLocalGatewayVirtualInterface"><span class="symbol function"></span>GetLocalGatewayVirtualInterface</a></li>
    <li><a href="getlocalgatewayvirtualinterfacegroup" title="GetLocalGatewayVirtualInterfaceGroup"><span class="symbol function"></span>GetLocalGatewayVirtualInterfaceGroup</a></li>
    <li><a href="getlocalgatewayvirtualinterfacegroups" title="GetLocalGatewayVirtualInterfaceGroups"><span class="symbol function"></span>GetLocalGatewayVirtualInterfaceGroups</a></li>
    <li><a href="getlocalgateways" title="GetLocalGateways"><span class="symbol function"></span>GetLocalGateways</a></li>
    <li><a href="getmanagedprefixlist" title="GetManagedPrefixList"><span class="symbol function"></span>GetManagedPrefixList</a></li>
    <li><a href="getnatgateway" title="GetNatGateway"><span class="symbol function"></span>GetNatGateway</a></li>
    <li><a href="getnetworkacls" title="GetNetworkAcls"><span class="symbol function"></span>GetNetworkAcls</a></li>
    <li><a href="getnetworkinterface" title="GetNetworkInterface"><span class="symbol function"></span>GetNetworkInterface</a></li>
    <li><a href="getnetworkinterfaces" title="GetNetworkInterfaces"><span class="symbol function"></span>GetNetworkInterfaces</a></li>
    <li><a href="getprefixlist" title="GetPrefixList"><span class="symbol function"></span>GetPrefixList</a></li>
    <li><a href="getroute" title="GetRoute"><span class="symbol function"></span>GetRoute</a></li>
    <li><a href="getroutetable" title="GetRouteTable"><span class="symbol function"></span>GetRouteTable</a></li>
    <li><a href="getroutetables" title="GetRouteTables"><span class="symbol function"></span>GetRouteTables</a></li>
    <li><a href="getsecuritygroup" title="GetSecurityGroup"><span class="symbol function"></span>GetSecurityGroup</a></li>
    <li><a href="getsecuritygroups" title="GetSecurityGroups"><span class="symbol function"></span>GetSecurityGroups</a></li>
    <li><a href="getspotprice" title="GetSpotPrice"><span class="symbol function"></span>GetSpotPrice</a></li>
    <li><a href="getsubnet" title="GetSubnet"><span class="symbol function"></span>GetSubnet</a></li>
    <li><a href="getsubnetids" title="GetSubnetIds"><span class="symbol function"></span>GetSubnetIds</a></li>
    <li><a href="gettransitgatewayroutetables" title="GetTransitGatewayRouteTables"><span class="symbol function"></span>GetTransitGatewayRouteTables</a></li>
    <li><a href="getvpc" title="GetVpc"><span class="symbol function"></span>GetVpc</a></li>
    <li><a href="getvpcdhcpoptions" title="GetVpcDhcpOptions"><span class="symbol function"></span>GetVpcDhcpOptions</a></li>
    <li><a href="getvpcendpoint" title="GetVpcEndpoint"><span class="symbol function"></span>GetVpcEndpoint</a></li>
    <li><a href="getvpcendpointservice" title="GetVpcEndpointService"><span class="symbol function"></span>GetVpcEndpointService</a></li>
    <li><a href="getvpcpeeringconnection" title="GetVpcPeeringConnection"><span class="symbol function"></span>GetVpcPeeringConnection</a></li>
    <li><a href="getvpcpeeringconnections" title="GetVpcPeeringConnections"><span class="symbol function"></span>GetVpcPeeringConnections</a></li>
    <li><a href="getvpcs" title="GetVpcs"><span class="symbol function"></span>GetVpcs</a></li>
    <li><a href="getvpngateway" title="GetVpnGateway"><span class="symbol function"></span>GetVpnGateway</a></li>
</ul>

<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-aws">https://github.com/pulumi/pulumi-aws</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>{{% md %}}This Pulumi package is based on the [`aws` Terraform Provider](https://github.com/terraform-providers/terraform-provider-aws).{{% /md %}}</dd>
	<dt>Version</dt>
	<dd>3.35.0</dd>
</dl>

