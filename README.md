# KAC-Files (Kometa Anime Config Files)

Welcome to **KAC-Files**! This repository houses some of my personal anime config files with supporting assets for **[Kometa](https://kometa.wiki/)** to create collections for `Genres` and `Seasons`.
---

### 1. Configs
*   **Genres Config:** Builds collections based on anime genres. It also automatically curates collections for 4 MAL lists.
*   **Seasons Config:** Keeps track of and builds collections for anime by seasons and year (e.g., Summer Season 2015, Spring Season 2026). Also adds an `Anime This Season` that updates to the current anime airing.

### 2. Supporting Files (`/Covers`)
*   A dedicated folder containing all the custom collection covers used by the config files. Kometa will grab these.

---

### Setup & Installation

#### Option 1: Install via URL

By using the direct URL, Kometa automatically pulls the latest version of the config file every time it runs. If this repository is updated with new collections, seasons, or fixes, your setup will sync automatically—no manual re-downloading required.

Open your main Kometa `config.yml` file and register the raw URLs for the YAML file(s) under the `collection_files` section for your desired library. Replace the URL paths with the raw links to your files in this repository:

```yaml
libraries:
  Anime: # Replace with your library name (e.g., Anime, TV Shows, Movies)
    collection_files:
      - url: https://raw.githubusercontent.com/KenWeTech/KAC-Files/main/Genres.yml
      - url: https://raw.githubusercontent.com/KenWeTech/KAC-Files/main/Seasons.yml

```

_Run Kometa as usual, and it will pull the files and covers directly from the repository._

#### Option 2: Install via Local Files

1.  **Download the Config Files**
  
    -   Download one or both of the YAML files (`Genres.yml` / `Seasons.yml`) depending on which collections you want to use, and place them in your Kometa `config` directory.

2.  **Add to Kometa Config**

    -   Open your main Kometa `config.yml` file and register the new YAML file(s) under the `collection_files` section for your desired library. This works for any library type or name in your media server (e.g., Anime, TV Shows, Movies, etc.):

    ```yaml
    libraries:
      Anime: # Replace with your library name (e.g., Anime, TV Shows, Movies)
        collection_files:
          - file: config/Genres.yml   # Use if you downloaded the Genres config
          - file: config/Seasons.yml  # Use if you downloaded the Seasons config
    
    ```

3.  **Run Kometa**

    -   Execute Kometa as usual. It will read the new YAML files and handle everything automatically!
