# Profile
* 🛩️ Blog https://blog.csdn.net/NP_hard
* 🔍 Interest: Database-Kernel & Cloud Native/DevOps & AI
* 📫 Contact me: hewen.deng@u.nus.edu

# Overview
![Anurag's GitHub stats](https://github-readme-stats-git-masterrstaa-rickstaa.vercel.app/api?username=David-deng-yeah&show_icons=true&theme=radical)

# Recent projects

## Operating System Engineering: MIT 6.S081
* **timeline**: Sep 2023  ~  Now
* **Project Description**: Read and use GDB tools to debug xv6 source code, understand the implementation of operating system-related technologies, and make modifications based on this to improve system performance.
* Speed up system calls: Add kernel page tables to user processes to speed up user-level and kernel-level message passing.
* Reducing lock contention: Reducing the lock granularity by performing CPU memory stealing and building hash tables, thus reducing the lock contention between the memory allocators and block caches, improving the system performance.
* Utilize lazy allocation and cow fork techniques to spread the time overhead of large chunks of memory and improve response time.
* Understand user-kernel communication and add several system calls such as mmap, munmap etc.

## PostgreSQL Source Code Retrofitting
* **timeline**: Jul 2023 ~ Sep 2023
* **Project description:** Deeply study the storage management, memory management, indexing, concurrency control and other technologies in PostgreSQL source code to realize the following functions:
* **Add new type IntSet:** Utilize plug-in mechanism to customize IntSet data types, write structures, IO functions and operators, and compile them into shared libraries for database loading. Handling large chunks of data by compressing and storing large field values in TOAST tables associated with user tables through TOAST technology;
* **Symmetric hash:** Improving the hash join process in PostgreSQL by adding symmetric hash algorithms to realize symmetric hash joins and avoid blocking in the hash table construction phase;
* **Dirty read plugin:** Implementing a dirty read plugin with the help of the MCCC mechanism to obtain visible tuples based on a given transaction number and to realize transaction execution history backtracking.

## Cloud-native high-performance video website 
* **timeline**: Apr 2023 ~ Jul 2023
* **Project Description:** Developed an online video website, with 3 microservice modules: user module, video module, comment module. Service registration and kv configuration acquisition between the modules is done through consul and k8s is used for container orchestration.
* **login authentication:** Unified authentication and single sign-on (SSO) based on grpc+jwt; implemented RBAC rights management model.
* **Log Monitoring and Alerting**: Use the logrus framework to encapsulate logs and use middleware to intercept log messages and send them to RabbitMQ for logging. Based on Prometheus and Grafana to achieve monitoring alerts and metrics visualization, such as CPU occupancy, QPS, and so on.
* **Automated Deployment:** project to automate build, test and deployment. With dependency format checking, code format checking, code static checking and so on.
* **Performance Optimization:** Using Jmeter and pprof tools, the video leaderboard on the home page of the website has been tested and iterated with three stress tests, from the sorting of videos based on MySQL and go Map to the final choice of redis Zset for implementation, the 95th percentile of the leaderboard response time with the Throughput is optimized from 2922ms and 47.47qps to 183ms and 73.607qps, which is an improvement of 93.73% and 55.06% respectively


![微信图片_20230908000144](https://github.com/David-deng-yeah/David-deng-yeah/assets/65102150/1e56e91f-53af-46a0-bc6d-e045aaed9301)





## Simple Tiktok - ByteDance Youth Training Camp
* **timeline**: Jan 2023 ~ Mar 2023
* **Project description:** Implemented a minimalist version of Tiktok backend, with video push, video submission, video likes, video comments and other functions.
* **Work content:** Use JWT for user token validation, Consul for service discovery and service registration, as well as KV reading of configuration files, and Gorm for ORM operations on MySQL.
* **Microservices Architecture Design:** Adopting the single-case pattern, a manager class is defined in each microservice to manage three resources: database, cache and object storage.
* Using Redis to cache hot data such as video like information, video URL.; Using MySQL to persist the cold data; add random offsets for the expiration time of the hot data to alleviate the cache avalanche problem

![4d365cb5e9ed565fc4112093e6f0f620 (2)](https://github.com/David-deng-yeah/David-deng-yeah/assets/65102150/18985327-2412-4bd7-89b9-92cedfda1dc4)

