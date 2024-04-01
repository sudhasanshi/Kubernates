

1.Nodeselector
We can set labels to nodes as shown below 

![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/b8f6a5e8-eb12-487b-8ce1-bc9bc4a0d628)
We can run pod on particular node(refer file nodeselector.yml)

![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/1f3fe32b-846c-4ca1-952f-44cb21556c9b)

2. Affinity
   a. nodeaffinity
      1. softrule-preffered (In operator)
         reference file- nodeaffinitysoftruleprefferedIn.yml
         ![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/7cece9ec-70e9-4fc7-bcdd-2cf2d12fa286)

      2. softrule-preffered (NotIn operator)
          reference file- nodeaffinitysoftruleprefferedNotIn.yml
          ![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/8151b219-763b-4403-a61b-84fcd98e2715)
   
      3. hardrule-required(In operator)
         reference file-nodeaffinityhardrulerequiredIn.yml
         ![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/48fb0a34-2efc-4eb4-af4d-91e614b80d2e)

      4. hardrule-required(In operator)
         reference file-nodeaffinityhardrulerequiredNotIn.yml
         ![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/ee147a47-ce1d-4821-9682-27fe0d06e452)
   b. podaffinity
      1. podaffinity (In operator)
         reference file -podaffinityIn.yml
         ![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/fd0e8deb-2ab2-4ea1-8e17-237b756b858a)

      2. podaffinity (NotIn operator)
         reference file -podaffinityNotIn.yml
         ![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/c7c26c0b-369b-4141-9a6c-b10ac2560027)

      4. podantiaffinity
         reference file -podantiaffinityIn.yml
         ![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/4f7eff1d-4c1b-4dcd-aab2-a8c7e673e29f)

      5. podantiaffinity
         reference file -podantiaffinityNotIn.yml
         ![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/13c2a745-6563-4ba8-a5c5-421aa231d7db)
3. taint
   a. taint with normal deployment(reference file taintexample.yml)
     - first we have to taint the node using below command
        kubectl taint node node-name(ip-10-0-0-120.ap-south-1.compute.internal) color=red:NoSchedule
     - that means pods will not run on that node. you can see in screenshot pods are running on other node
     - pods will run on others nodes except that node
     - to check node tainted or not use below command
        kubectl describe node node-name
       ![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/1b04fbb4-5ef6-4773-a5dc-2f23794a65d1)

  b. taint with NodeSelector deployment file(reference file taintnodeselector.yml)
   - pods will go into pending state because we mentioned nodeselector as worker1 in deployment file and we made same node as tainted
     ![image](https://github.com/sudhasanshi/Kubernates/assets/35460293/eed668b9-8f40-43eb-ad49-22f591af0033)
     
 4. toleration
     even though node is tainted we can run pods on that node by specifing toleration details in deployment file so that pods will run on that node
    - reference file (tolerationexample.yml)


 5.   ResourceQuota with namespace
    - referenc directory resourceQuota  
    

   





















   
