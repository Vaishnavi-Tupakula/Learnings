<h1>Why Docker?</h1>
<hr>
<br>

<p>Let's consider a software Development Team working on an application with some dependencies.
<br>

<b>What are these dependencies?</b><br>
<p>If the team is working on a MERN application, one of the developers might be using a Linux machine and node.js with version 16, reddis cache with version 6 to set up his local dev environment. These can be termed as dependencies since the application requires them for execution.</p>
<br>
<b>What happens if we want the application to be run in a different environment?
</b><br>

<p>Let's say a new developer joins the team using Mac book air. To run the application or to work on it, the new developer must install all the dependencies.</p>
<br>

<b>Issues</b><br>
<ul>An application can have multiple dependencies, manually installing all the dependencies is tiresome</ul>
<ul>Some applications might run only on specific versions, so it's important that right version of dependencies are installed</ul>
<ul>If the application uses CLI commands for linux, the same cannot be applied in a Windows system or Mac</ul>
<ul>If it is confined to a single development team with few members we can still choose to replicate local environment across all the machines even though its tiresome and prone to error, but doing it across thousands of developer machines and replicating the same in the production server is quite challenging!</ul>
<br>
</p>

<h1>What is Docker?</h1><hr><br>
<p>Docker is a platform that allows to create, destroy and update containers.
<br>


<b>What is a Container?</b><br>
<p>It can be termed as the packaging of the application code and it's dependencies together as a single bundle which can be shared with other developers and platforms.<br>
This containers can run the same way on any OS without making any changes to the machine.
<br>
Features
<ul>Portable</ul>
<ul>Lightweight(Easily creatable, updatable, destroyable)</ul>
<ul>Allows us to add new dependencies to the existing container.</ul>
<ul>Generally, if 2 applications are running on the system with node.js 16 installed, both of them would run on the same version, but containers can allow us to use different versions for different applications in the same local machine using 2 different containers.</ul>
</p>
<br>


<b>What is Docker Image?<b><br>
<p>Docker image is an executable that contains instructions on creation of Container.
A Docker image can be used to create multiple containers. When we talk about sharing containers, we actually mean sharing these docker images that allows us to create containers locally.<br>
Docker image is a static snapshot of how exactly the code and its dependencies look like.
</p>

<b>Understanding the concept with classes and Objects<b><br>
<p>Docker image can be considered as Class, which acts like a blueprint for building containers. Container can be viewed as an object which actually interacts with the system like an object which actually resides in the memory.</p>

</p>


<h1>VM Vs Docker</h1><hr><br>
<p>
VM's
<ul>Virtualises OS kernel and application layer of the system</ul>
<ul>Relatively heavy weight</ul>
<ul>Compatible with any kind of OS and systems</ul>
</p>

<p>
Docker
<ul>Virtualises Application layer alone.</ul>
<ul>Runs on the same OS kernel as host</ul>
<ul>Light weight</ul>
<ul>Compatible with linux based systems majoritily. So we use Docker Desktop that adds a lightweight hypervisor to the system that uses lightweight linux based distribution to run containers on windows or macs for a linux based docker image and vice versa.</ul>
</p>