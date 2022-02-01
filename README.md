# Office Deployment Tool
To configure and perform deployments of volume licensed versions of Office 2019, including Project and Visio, for users in your organization, you use the Office Deployment Tool (ODT)

## configuration.xml
Example
```
<Configuration>
  <Add SourcePath="\\Server\Share" OfficeClientEdition="64" Channel="PerpetualVL2019">
      <Product ID="ProPlus2019Volume"  PIDKEY="#####-#####-#####-#####-#####" >
         <Language ID="en-us" />
      </Product>
      <Product ID="ProofingTools">
        <Language ID="de-de" />
        <Language ID="ja-jp" />
      </Product>
  </Add>
  <RemoveMSI />
  <Display Level="None" AcceptEULA="TRUE" />  
</Configuration>
```
## Download installation files
```
setup /download configuration.xml
```

## Install by using the ODT
```
setup /configure configuration.xml
```

[Link](https://docs.microsoft.com/en-us/deployoffice/office2019/deploy#deploy-languages-for-office-2019 "Deploy Office 2019 (for IT Pros)")

[GVLK](https://docs.microsoft.com/en-us/DeployOffice/vlactivation/gvlks "GVLKs for KMS")
