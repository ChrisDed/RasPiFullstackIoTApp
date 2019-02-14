# RasPiFullstackIoTApp
Raspberry Pi device that has a temperature and humidity sensor. Device receives readings from sensor, and using a text-to-speech service, notifies the user the temperature and humidity of the room. Then, an MQTT message is published to a specific AWS IoT topic, which triggers an AWS Lambda function, and adds the temperature, humidity, and time telemetry data into a DynamoDB table. Also a basic web UI that requests an API endpoint, that triggers a Lambda function, which then queries the DynamDB table for all data, and lastly responds with the IoT telemetry data and gets displayed on a basic dashboard.

This is a basic Full Stack IoT application I developed on my first week at TensorIoT to train myself how to build IoT solutions before hopping on client projects.

UI Dashboard URL: http://chris-iot-temp-ui.s3-website-us-east-1.amazonaws.com/
