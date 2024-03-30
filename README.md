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

