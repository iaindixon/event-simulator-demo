This demo takes only the IoT simulator part of Jens Reimann's hono-demo-1 demo and modifies it for a specified workload. 

This simulator presents three demo options, 
1. Only telemetry messages
2. Only event messages
3. Both telemetry and event messages

## Deploy the demo

Create a new project for the simulator and deploy it:

~~~sh
oc new-project iot-simulator --display-name='IoT simulator'
oc process -f src/openshift/event_demo.yml | oc create -f -
~~~
