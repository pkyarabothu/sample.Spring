Spring/SpringMVC v3.2.1 Integration
==============

This open source integration demonstrates Spring and Spring MVC integration through a simple phonebook sample Web application deployed to Liberty.

This sample demonstrates Spring and Spring MVC integration through a simple phonebook Web application deployed to Liberty.

This sample can be installed onto runtime versions 8.5.5.0 and later.


## Running in Eclipse with Maven

1. Clone this project and import into Eclipse as an 'Existing Maven Project'.
2. Right-click the project and select **Run As > Maven Clean**.
3. Right-click the project and select **Run As > Maven Install**.
4. Right-click the project and select **Run As > Maven Build...** then run the goal `liberty:run-server`.
5. You should see the following in the console: `Application PhoneBookBySpringMVC started in XX.XX seconds.`

## Running with Maven

This project can be built with [Apache Maven](http://maven.apache.org/). The project uses [Liberty Maven Plug-in][] to automatically download and install Liberty profile runtime from the [Liberty repository](https://developer.ibm.com/wasdev/downloads/). Liberty Maven Plug-in is also used to create, configure, and run the application on the Liberty server. 

Use the following steps to run the application with Maven:

1. Execute full Maven build. This will cause Liberty Maven Plug-in to download and install Liberty profile server.
    ```bash
    $ mvn clean install
    ```
    
2. To run the server with the Servlet sample execute:
    ```bash
    $ mvn liberty:run-server
    ```

In your browser, enter the URL for the application: [http://localhost:9811/phonebook/](http://localhost:9811/phonebook/) (where port 9811 assumes the httpEndpoint provided in the sample server.xml has not been modified).
In your browser, you should see the phone book displayed.

# Notice

© Copyright IBM Corporation 2017.

# License

```text
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
````

[Liberty Maven Plug-in]: https://github.com/WASdev/ci.maven
