# Jenkins Hello World Job

## Project Overview
This project demonstrates how to create and execute a simple Jenkins Freestyle job using a shell script stored in a GitHub repository.

## Objectives
- Create a shell script that prints a message.
- Store the source code in GitHub.
- Configure Jenkins to fetch code from GitHub.
- Execute the script using a Jenkins build job.
- Verify the build result using Console Output.

## Technologies Used
- **Jenkins** – Continuous Integration and build automation.
- **Git** – Version control.
- **GitHub** – Source code hosting.
- **VS Code** – Code editor.
- **Bash Shell Script** – Script execution.

## Project Structure

```text
devops-sample-code/
├── hello-world.sh
├── screenshots/
│   └── jenkins-build-success.png
└── README.md
```

## Shell Script

File: `hello-world.sh`

```bash
#!/bin/bash
echo "Hello, Jenkins!"
```

## Jenkins Job Configuration
1. Create a new Jenkins job named `HelloWorld`.
2. Select **Freestyle project**.
3. Configure Git under Source Code Management.
4. Enter the GitHub repository URL.
5. Select the `main` branch.
6. Add an **Execute shell** build step.
7. Execute the command:

```bash
sh hello-world.sh
```

8. Save the configuration and click **Build Now**.

## Expected Output

```text
Hello, Jenkins!
Finished: SUCCESS
```

## Result
The Jenkins Freestyle job successfully cloned the source code from GitHub, executed the shell script, and displayed the expected output in Console Output.

## Screenshot
The successful build screenshot is available in the `screenshots/` directory.

## Conclusion
This project demonstrates a basic Continuous Integration workflow using Jenkins and GitHub. It provides a foundation for automating builds and integrating more advanced DevOps workflows.
