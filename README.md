# Nitc-Expos
The official nitc expos website has few flaws in its roadmap, here is the final code for the steps till task scheduling in the nitc website, you can implement basic 2 task scheduling , one being an idle task and the other can be set by us, follow the official nitc expos documentation and look at my code for any doubts 
I have fixde few flaws in the code for task scheduling, one being the use of the registers which are getting stored, when we switch task during task scheduling and use the genral purpose registers, it will corrupt the code as the values in the registers are changed before saving the state, so i have used the register expos uses as internal register to prevent this problem
This is one of the major problem which has stumpped me for days but finally could get past it after realising this mistake.


I have created a docker container containing nitc expos with the 2 taskschedulingcode implemented. just install and run this container and you are set to go

```

docker load -i nitcexpos.tar
docker exec -it <your_docker_Id> bash

```
