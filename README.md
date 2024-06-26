# Task Scheduling

This project is a React-based frontend designed to visualize task schedules and Application and Platform model. It interfaces with a backend server, with the configuration specified in `config.json`.



## Table of Contents
1. [Technologies Used](#technologies-used)
2. [Features](#features)
3. [Setup](#setup)
4. [Usage](#usage)
5. [To-do list](#to-do-list)


## Technologies Used
**Frontend:**
    - React
    - JavaScript
    - CSS

**Backend:**
    - Python
    - https://github.com/linem-davton/es-lab-task2.git



## Features
- **Upload JSON File**: Also, one can upload a JSON file to visualize a pre-defined Application model.
- **Add Nodes and Edges**: Users can create a graph of the Application model by adding nodes and edges interactively through the interface.
- **Graph Visualization**: The application provides a clear visualization of the Application model, making it easy to understand task dependencies.
- **Scheduling Algorithms**: The application can schedule the graph using five different algorithms, offering flexibility and multiple approaches.
- **Schedule Visualization**: Users can visualize the resulting schedules in a bar graph format, providing a clear overview of the task timeline.
- **Cross-Platform Compatibility**: The application works seamlessly across different devices and browsers.



## Usage

### For Users

1. **Accessing the Application**
   - Open the web browser and navigate to the application URL 'https://eslab2.pages.dev/'.

   - **Upload JSON File**: Click on the "Upload JSON" button to upload a pre-defined Application model. The  JSON file should follow the input schema defined at 'https://eslab2docs.pages.dev/README#api-input-schema-for-schedule-jobs'.
   
   - **Load Default Json file**: Clicking on the "Load Default Json" will load a default application model.

   - **Saving and Exporting**: Export the updated JSON file containing the Application and Platform model by clicking the "Download JSON" button. This will download the JSON file to your device, allowing you to save it locally or share it with others as needed.
   Alternatively, "Save Locally" button will save the models locally which can be accessed on later page visits by "Load Last Saved" button.

   
 2. **Create an Application Model**
    - **Add Tasks and Task Dependencies**: Create your own Application model by selecting the "Application model" on the screen. Use the "Add Tasks" button to create tasks individually and tasks dependencies using the "Add dependency" button.

    - **Sliders**: WCET and deadline for a task can be changed by clicking on the task and adjusting the respective sliders.

    - **Delete Mode**: The tasks and Edges can be deleted by first clicking on the "Delete Mode" button then selecting the task or edge you want to delete.

    - **Generate Random Application Model**: Generate a random application model by entering the number of tasks. 

    - **Visualizing the Application Model**:The Application model will be displayed as a directed acyclic graph. Nodes represent tasks, and edges represent dependencies between tasks.


3. **Create a Platform Model**
   
   - **Add Nodes and Links**: Create your own Platform model by selecting the "Platform model" on the screen. Use the "Add Node" button to create nodes individually and links using the "Add Link" button.

   - **Sliders**: delay and bandwidth for a node can be changed by clicking on the edge and adjusting the respective sliders.

   - **Delete Model**: The nodes and links can be deleted by first clicking on the "Delete Mode" button then selecting the node or link you want to delete.

   - **Generate Random Platform Model**: Generate a random platform model by entering the number of nodes. 

   - **Visualizing the Platform Model**:The Platform Model will be displayed as a graph. Nodes represent nodes, and edges represent links between the nodes.

4. **Shortcuts**

   - **Tab**: Switches between the Application and Platform model.
   - **When Application Model is selected**:
      - **'1'** will add a task.
      - **'2'** will add a dependency.
      - **'w'** will cycle through the tasks.
   - **When Platform Model is selected**:
      - **'1'** will add a node.
      - **'2'** will add a link.
      - **'w'** will cycle through the links.
 
5. **Visualizing the Schedules**

   - Along with the Application and Platform model, five different Schedules will be fetched from the backend, representing different algorithms.
   - The resulting schedules will be visualized in a bar graph format.
   - Users can compare the different schedules generated by the algorithms.
   - Any changes made in the application or platform model will be immediately reflected in the Schedules.



### For Developers

1. **Fork the front-end Repository**
   - Go to the project repositories
    - Front-end: https://github.com/linem-davton/graphdraw-frontend.git.
   - Click on the "Fork" button to create a copy of the repository in your GitHub account.

2. **Clone the Repository**
   - Clone the forked repository to your local machine:
     - Front-end: git clone https://github.com/linem-davton/graphdraw-frontend.git
    


3. **Navigate to the Project Directory**
   - Change to the project directory:
     cd your-repo


4. **Install Dependencies**
   - Install the necessary dependencies for the frontend:
     npm install
   

5. **Run the Application**
   - Start the backend server:
     python src/backend.py

   - Start the frontend development server:
     npm run dev
     
   - Open your browser and navigate to `http://localhost:5173/` to view the application.


7. **Understanding the Project Structure**
   - Familiarize yourself with the project structure. Key directories include:
     - `src/` - Contains the React components and application logic.
     
  

8. **Making Changes**
   - Create a new branch for your feature or bugfix:
     git checkout -b feature/your-feature-name
     
   - Make your changes in the codebase.

   - Commit your changes with a descriptive commit message:
     
     git commit -m "Add feature X"
     
   - Push your changes to your forked repository:
     git push origin feature/your-feature-name
     

10. **Submitting a Pull Request**
    - Go to the original repository on GitHub.
    - Click on the "New Pull Request" button.
    - Select your branch and submit the pull request for review.

By following these steps, you can set up the project locally, understand its structure, make contributions, and submit your changes for review. Your contributions are greatly appreciated!
