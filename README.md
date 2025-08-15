# Simple Java Maven Build in Jenkins

## Objective
Run a basic Java Maven build job in Jenkins.

## Steps

### 1. Prepare Java Project

/opt/hello-java-maven
├── src/main/java/com/example/HelloWorld.java
└── pom.xml

### 2. Configure Maven in Jenkins

Go to Manage Jenkins → Tools.

Add Maven → Name it Maven3 → Install automatically.

### 3. Create Jenkins Freestyle Job

New Item → Freestyle Project.

Source Code Management → Git → point to your project folder or repo.

Build → Invoke top-level Maven targets → Goals: clean package

Save and Build the Job

### 4. Verify

Check console output for BUILD SUCCESS.

----------------------------------------------
