# ConnecTo: Graph-Based Social Network Analysis

**ConnecTo** is a graph-based social network analysis application that allows users to explore, analyze, and interact with their network of connections. The app provides features for discovering recommendations, visualizing connections, and managing profiles.

### Features:
- **User Authentication**: Login, sign up, and log out functionality.
- **Profile Management**: View and update your personal profile.
- **Network Management**: Follow and unfollow users to build your network.
- **Search**: Find users and view their profiles.
- **Connections Visualization**: Analyze connections between users, including direct and mutual connections.
- **Friend Recommendations**: Suggestions based on:
   - Mutual Friends
   - Interest-Based Matching
   - Most Influential Users
   - Most Active Users
- **Friend List**: View your list of followers and connections.
- **Trending Users**: Discover users with frequent posts and activity.
- **Shortest Path in Connections**: Find the shortest connection ties between users.

### Setup Instructions:
#### File Placement:
1. Place `graph.cpp`, `graph.h`, and `main.cpp` in the same directory.
2. Create two subfolders:
   - `include`: Contains `raylib.h` for the graphical user interface.
   - `lib`: Contains `libraylib.a` for the Raylib library.

#### Compilation:
Open your terminal in the project directory and run the following command:

```bash
g++ main.cpp graph.cpp -o main.exe -O1 -Wall -std=c99 -Wno-missing-braces -I include/ -L lib/ -lraylib -lopengl32 -lgdi32 -lwinmm
```

#### Explanation of Flags:
- `-o main.exe`: Specifies the output file name.
- `-O1`: Optimizes the build for performance.
- `-Wall`: Enables all compiler warnings.
- `-std=c99`: Uses the C99 standard (Raylib uses a C-based API).
- `-I include/`: Directory for Raylib header files.
- `-L lib/`: Directory for Raylib library files.
- `-lraylib`: Links Raylib.
- `-lopengl32 -lgdi32 -lwinmm`: Links system libraries necessary for Windows.

After compiling, run the program:

```bash
.\main
```

### Folder Structure:
- **include/**: Contains Raylib header (`raylib.h`).
- **lib/**: Contains Raylib library (`libraylib.a`).
- **main.cpp**: The main program file.
- **graph.cpp**: Contains the implementation of graph-related functionalities.
- **graph.h**: Header file for graph-related functions.
- **run.bat**: Script to execute the application.
- **users.txt**: Stores user data, including IDs, usernames, interests, posts, comments, likes, and friend connections.

### Technologies Used:
- **C++ Libraries**:
  - `<iostream>`, `<fstream>`, `<sstream>`, `<vector>`, `<map>`, `<set>`, `<queue>`, `<unordered_map>`, `<cstring>`, `<algorithm>`
- **Raylib**: A simple library for game and graphical applications.
- **IDE**: Visual Studio Code.

### Additional Setup:
1. **Raylib Setup**: Ensure you follow the setup guide [here](https://youtu.be/HPDLTQ4J_zQ?si=lt3rLL34TPG-l6AB) to correctly link Raylib in your project.
2. **Sample Graph**: For a general lookup of user connections, refer to the image below created in Python.

![Social Network Graph](https://github.com/user-attachments/assets/793300ff-be44-4c2c-9207-21e42b38557f)
