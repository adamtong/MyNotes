## Configure access key for AWS CLI

Configure the AWS CLI
```
PS C:\Users\xadaton> aws configure
AWS Access Key ID [None]: YOUR_ACCESS_KEY
AWS Secret Access Key [None]: YOUR_SECRET_ACCESS_KEY
Default region name [None]: YOUR_REGION
Default output format [None]: json
```

```
aws ec2 run-instances --image-id ami-0b8fd93c15b2c81ce --instance-type t3.micro --key-name lampserver-keypair --security-groups lampserver-sg
```

<details>
<summary>Comamnd Output</summary>

```json
{
    "Groups": [],
    "Instances": [
        {
            "AmiLaunchIndex": 0,
            "ImageId": "ami-0b8fd93c15b2c81ce",
            "InstanceId": "i-03a700b7ae55ecd6a",
            "InstanceType": "t3.micro",
            "KeyName": "lampserver-keypair",
            "LaunchTime": "2024-07-27T23:29:58+00:00",
            "Monitoring": {
                "State": "disabled"
            },
            "Placement": {
                "AvailabilityZone": "eu-north-1a",
                "GroupName": "",
                "Tenancy": "default"
            },
            "PrivateDnsName": "ip-172-31-16-134.eu-north-1.compute.internal",
            "PrivateIpAddress": "172.31.16.134",
            "ProductCodes": [],
            "PublicDnsName": "",
            "State": {
                "Code": 0,
                "Name": "pending"
            },
            "StateTransitionReason": "",
            "SubnetId": "subnet-090395d133e8904c2",
            "VpcId": "vpc-0e0a744efae004f66",
            "Architecture": "x86_64",
            "BlockDeviceMappings": [],
            "ClientToken": "fd830418-9fdf-449c-9451-3c6d91cd6adb",
            "EbsOptimized": false,
            "EnaSupport": true,
            "Hypervisor": "xen",
            "NetworkInterfaces": [
                {
                    "Attachment": {
                        "AttachTime": "2024-07-27T23:29:58+00:00",
                        "AttachmentId": "eni-attach-0494f399a7e138285",
                        "DeleteOnTermination": true,
                        "DeviceIndex": 0,
                        "Status": "attaching",
                        "NetworkCardIndex": 0
                    },
                    "Description": "",
                    "Groups": [
                        {
                            "GroupName": "lampserver-sg",
                            "GroupId": "sg-0c856a0aebce6debe"
                        }
                    ],
                    "Ipv6Addresses": [],
                    "MacAddress": "06:93:c5:5e:83:09",
                    "NetworkInterfaceId": "eni-01b88282dc1bcc991",
                    "OwnerId": "730335494606",
                    "PrivateDnsName": "ip-172-31-16-134.eu-north-1.compute.internal",
                    "PrivateIpAddress": "172.31.16.134",
                    "PrivateIpAddresses": [
                        {
                            "Primary": true,
                            "PrivateDnsName": "ip-172-31-16-134.eu-north-1.compute.internal",
                            "PrivateIpAddress": "172.31.16.134"
                        }
                    ],
                    "SourceDestCheck": true,
                    "Status": "in-use",
                    "SubnetId": "subnet-090395d133e8904c2",
                    "VpcId": "vpc-0e0a744efae004f66",
                    "InterfaceType": "interface"
                }
            ],
            "RootDeviceName": "/dev/xvda",
            "RootDeviceType": "ebs",
            "SecurityGroups": [
                {
                    "GroupName": "lampserver-sg",
                    "GroupId": "sg-0c856a0aebce6debe"
                }
            ],
            "SourceDestCheck": true,
            "StateReason": {
                "Code": "pending",
                "Message": "pending"
            },
            "VirtualizationType": "hvm",
            "CpuOptions": {
                "CoreCount": 1,
                "ThreadsPerCore": 2
            },
            "CapacityReservationSpecification": {
                "CapacityReservationPreference": "open"
            },
            "MetadataOptions": {
                "State": "pending",
                "HttpTokens": "required",
                "HttpPutResponseHopLimit": 2,
                "HttpEndpoint": "enabled",
                "HttpProtocolIpv6": "disabled",
                "InstanceMetadataTags": "disabled"
            },
            "EnclaveOptions": {
                "Enabled": false
            },
            "BootMode": "uefi-preferred",
            "PrivateDnsNameOptions": {
                "HostnameType": "ip-name",
                "EnableResourceNameDnsARecord": false,
                "EnableResourceNameDnsAAAARecord": false
            },
            "MaintenanceOptions": {
                "AutoRecovery": "default"
            },
            "CurrentInstanceBootMode": "uefi"
        }
    ],
    "OwnerId": "730335494606",
    "ReservationId": "r-00452a8ca31a692ff"
}
```
</details>
