# Travel-Destination-app
# Travel Destination App

## Objective
The **Travel Destination App** is an Android application designed to help users manage a list of places they want to visit and mark places as "visited." The app demonstrates the usage of core Android components, including `ListView`, `Fragment`, `SharedPreferences`, file writing, and menu integration.

---

## Features
### 1. **ListView**
- Dynamically displays a list of destinations.
- Allows users to mark destinations as "visited" by long-pressing a list item.
- Visited destinations are visually distinguished with a color change.

### 2. **Fragments**
- **AddDestinationFragment**: Provides a user interface with an `EditText` and a button for adding new destinations.
- **DestinationListFragment**: Displays the list of destinations using a `ListView`.

### 3. **SharedPreferences**
- Saves user preferences, such as filtering to display only visited destinations.
- Retains preferences across app restarts.

### 4. **File Writing**
- Saves the list of destinations (including their visited status) to a file in internal storage.
- Reads the file on startup to restore the list.

### 5. **Menu Options**
- **Reset List**: Clears all saved destinations.
- **Toggle View**: Allows users to toggle between showing all destinations and only visited destinations.

---

## Project Structure
```plaintext
TravelDestinationApp/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/traveldestinationapp/
│   │   │   │   ├── MainActivity.java
│   │   │   │   ├── AddDestinationFragment.java
│   │   │   │   ├── DestinationListFragment.java
│   │   │   │   ├── DestinationAdapter.java
│   │   │   │   ├── Destination.java
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   ├── activity_main.xml
│   │   │   │   │   ├── fragment_add_destination.xml
│   │   │   │   │   ├── fragment_destination_list.xml
│   │   │   │   │   ├── list_item_destination.xml
│   │   │   │   ├── menu/
│   │   │   │   │   ├── main_menu.xml
│   │   │   │   ├── values/
│   │   │   │   │   ├── strings.xml
│   │   │   │   │   ├── colors.xml
│   │   │   │   │   ├── styles.xml
