
# Lab 4: Setup Connected Vehicle Solution and Simulator 

The AWS IoT Device Simulator uses the Automotive module to generate trip
data using the Connected Vehicle Reference Architecture.

Refer to the **Output** tab of the AWS IoT Simulator to get the website
endpoint (CloudFront URL), refer the key ‘Management Console’. First
time users need to register. Your special character in your email will
be replaced with underscore (\_) and act as user id.

Log into the AWS IoT Simulator and select the **Automotive** tab to
generate the vehicle data. For step by step guidance:

## Launch Simulated Vehicles

Use the following procedure to launch virtual connected vehicles.

On the IoT Device Simulator console page, in the navigation menu,
select **Automotive**.

Select + Add Vehicles.

In the **Create vehicles** window, specify the number of vehicles you
want to simulate. Enter a value between 1 and 100.

Select **Submit**.

More information:

<https://docs.aws.amazon.com/solutions/latest/iot-device-simulator/appendix-a.html>

After you start generating data, open **AWS IoT Core** -\> **Test** and
subscribe to connectedcar/telemetry/\<*VIN*\>. Simulated console will
have vehicle VIN which generated the data. You should be able to see the
message on AWS IoT test console.

You should also able to see telemetry data generated in the S3 bucket
named connected-vehicle-data-\<region\>-\<*AWS Account Number*\> (e.g.;
connected-vehicle-data-us-east-1-123456789123)

NEXT: [Lab 5](./Lab5.md)