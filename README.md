Cloud Formation Templates To Launch EC2 Instance and AWS Backuo 


You will need to specify AMI , Security Group and Key Pair 




    Type: AWS::EC2::Subnet::Id
    Default: <specify subnet >
    
  AMI:
    Description: The AMI ID for the image on the instances.
    Type: String
    Default: <specify AMI HERE > 
    Default: amises72637363837 # example 
    

    
  ServerSecurityGroup:
    Description: Select the security group that will be applied to the instances. 
    Type: AWS::EC2::SecurityGroup::Id
    Default: sg4349843343434434v # Example 
    
  KeyName:
    Description: EC2 KeyPair to enable SSH access to the Server
    Type: AWS::EC2::KeyPair::KeyName
    ConstraintDescription: KeyPair Must be created prior to adding it here .
    Default: mykeypair # example 
