# kubeconfig
#Sequence for setting up sensor simulator deployment
(1) Load postgres-storage.yaml   #creates local volumes for postgres data
(2) Load simulator-support-stack.yaml #creates postgres databases for pressure and temperature sensor data and active mq instance
(3) Load simulator-stack.yaml #creates simulator app to generate temperature and pressure data, datareceiver instance for processing temp and presdatareceiver for processing pres data
