# Social Network Application

## Overview
A Flask-based Social Network Management System where users can manage connections, suggest friends, view the network, and find paths between users.

## Features

### Add User
- **Endpoint:** `/add_user` (POST)
- **Description:** Add a new user.
- **Params:** `user`

### Connect Users
- **Endpoint:** `/connect_users` (POST)
- **Description:** Connect two users.
- **Params:** `user1`, `user2`

### Remove User
- **Endpoint:** `/remove_user` (POST)
- **Description:** Remove a user and their connections.
- **Params:** `user`

### Suggest Friends
- **Endpoint:** `/suggest_friends` (POST)
- **Description:** Suggest friends based on friends-of-friends.
- **Params:** `user`

### Remove Connection
- **Endpoint:** `/remove_connection` (POST)
- **Description:** Remove a connection between users.
- **Params:** `user1`, `user2`

### View Network
- **Endpoint:** `/view_network` (GET)
- **Description:** View the entire network.

### Find Shortest Path
- **Endpoint:** `/find_path` (POST)
- **Description:** Find the shortest path between two users.
- **Params:** `user1`, `user2`

## Sample Data
- **Users:** Ayaan, Ishaan, Maya, Riya, Dev, Sanya, Tanya, Yash, Kiran, Mehul
- **Connections:** (Ayaan, Ishaan), (Ayaan, Dev), (Ishaan, Maya), (Ishaan, Riya), (Maya, Tanya), (Riya, Dev), (Dev, Yash), (Sanya, Kiran), (Tanya, Mehul), (Yash, Maya)

## How to Run
1. Install dependencies:
   ```bash
   pip install flask
   ```
2. Run the Flask app:
   ```bash
   python app.py
   ```
3. Open in your browser:
   ```
   http://127.0.0.1:5000/
   ```

## File Structure
- **`app.py`**: Backend logic and endpoints.
- **`templates/index.html`**: Home page template.

## Future Improvements
- Add database for persistent storage.
- User authentication.
- Graphical network visualization.
- Enhanced friend suggestion logic with ML.

