# ingMedium-nifi-customProcessor
This repository includes a custom Apache Nifi processor. Detail in [here](https://efecanahmetoglu.medium.com/what-is-the-effect-of-apache-nifi-on-data-transfer-and-monitoring-between-multiple-platforms-51799cd1d6d9).


[What is the effect of Apache Nifi on data transfer and monitoring between multiple platforms?](https://efecanahmetoglu.medium.com/what-is-the-effect-of-apache-nifi-on-data-transfer-and-monitoring-between-multiple-platforms-51799cd1d6d9)

![1_wIcYA-7avqFaqKlopBpSzw](https://user-images.githubusercontent.com/45664044/134812447-c8dfe3cd-a1e9-4425-8e94-faea5887ecdb.jpeg)


Firstly, add a new Archetype in IDE if this is your first processor development.


![1](https://user-images.githubusercontent.com/45664044/134812558-b2310d07-c96f-4d8c-94c2-dc4e25c4d66c.jpeg)


  -GroupId: org.apache.nifi
  -ArtifactId: nifi-processor-bundle-archetype
  -Version: 1.5.0

Don't forget the additional property for maven.

  -Name: artifactBaseName
  -Value: customProcessor
  
![2](https://user-images.githubusercontent.com/45664044/134812677-faf45102-3a57-4592-b7fc-867ea73896f8.jpeg)
 
  
After complete all setup properties, you will have a new project for custom processor development.

I will share the code below the article.

After coding, you should build your project to use “maven clean install”.

Your processor build result keeps in the “Target” folder in your “nar” module root.

![4](https://user-images.githubusercontent.com/45664044/134812708-bbdb0cd8-3d94-4d61-bc33-62ba8203b93c.png)

Copy this nar file from here to Nifi Root at the “lib” folder.

Also, you will see the other default processors in there.

Custom processor development and deployment processes ended successfully.

You can start the Apache Nifi and put your custom processor on your flow page.

![5](https://user-images.githubusercontent.com/45664044/134812770-f14c91ad-7df0-443f-b5c9-5ed78146576d.png)


