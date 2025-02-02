# AWS::KinesisAnalyticsV2::ApplicationReferenceDataSource ReferenceDataSource<a name="aws-properties-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource"></a>

For a SQL\-based Managed Service for Apache Flink application, describes the reference data source by providing the source information \(Amazon S3 bucket name and object key name\), the resulting in\-application table name that is created, and the necessary schema to map the data elements in the Amazon S3 object to the in\-application table\.

## Syntax<a name="aws-properties-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-syntax.json"></a>

```
{
  "[ReferenceSchema](#cfn-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-referenceschema)" : ReferenceSchema,
  "[S3ReferenceDataSource](#cfn-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-s3referencedatasource)" : S3ReferenceDataSource,
  "[TableName](#cfn-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-tablename)" : String
}
```

### YAML<a name="aws-properties-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-syntax.yaml"></a>

```
  [ReferenceSchema](#cfn-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-referenceschema): 
    ReferenceSchema
  [S3ReferenceDataSource](#cfn-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-s3referencedatasource): 
    S3ReferenceDataSource
  [TableName](#cfn-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-tablename): String
```

## Properties<a name="aws-properties-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-properties"></a>

`ReferenceSchema`  <a name="cfn-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-referenceschema"></a>
Describes the format of the data in the streaming source, and how each data element maps to corresponding columns created in the in\-application stream\.  
*Required*: Yes  
*Type*: [ReferenceSchema](aws-properties-kinesisanalyticsv2-applicationreferencedatasource-referenceschema.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`S3ReferenceDataSource`  <a name="cfn-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-s3referencedatasource"></a>
Identifies the S3 bucket and object that contains the reference data\. A Kinesis Data Analytics application loads reference data only once\. If the data changes, you call the [UpdateApplication](https://docs.aws.amazon.com/kinesisanalytics/latest/apiv2/API_UpdateApplication.html) operation to trigger reloading of data into your application\.   
*Required*: No  
*Type*: [S3ReferenceDataSource](aws-properties-kinesisanalyticsv2-applicationreferencedatasource-s3referencedatasource.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`TableName`  <a name="cfn-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource-tablename"></a>
The name of the in\-application table to create\.  
*Required*: No  
*Type*: String  
*Minimum*: `1`  
*Maximum*: `32`  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

## See also<a name="aws-properties-kinesisanalyticsv2-applicationreferencedatasource-referencedatasource--seealso"></a>
+  [ReferenceDataSource](https://docs.aws.amazon.com/kinesisanalytics/latest/apiv2/API_ReferenceDataSource.html) in the *Amazon Kinesis Data Analytics API Reference* 

