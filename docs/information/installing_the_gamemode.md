## **Installation Tutorial**

Lilia is a versatile roleplaying framework for Garry's Mod. This tutorial will guide you through the process of installing Lilia on your Garry's Mod server, ensuring a smooth setup for your roleplaying environment.

---

## Prerequisites

Before you begin, ensure you have the following:

- **A Working Garry's Mod Server:** Make sure your server is properly set up and running without any issues.
- **Basic Knowledge of Server Administration:** Familiarity with managing a Garry's Mod server will be beneficial.
- **Command Line Proficiency:** Understanding how to use the command line is necessary for certain installation steps.
- **Admin Menu:** We recommend using [SAM](https://www.gmodstore.com/market/view/sam) for enhanced administrative capabilities.

---

## Step 1: Setting Up Your Garry's Mod Server

If you haven't already, set up your Garry's Mod server. Ensure it's running smoothly before proceeding with the installation of Lilia.

---

## Step 2: Downloading Lilia

1. **Visit the Lilia GitHub Repository:**

    Navigate to the [Lilia GitHub Repository](https://github.com/LiliaFramework/Lilia).

2. **Download the ZIP File:**

    - Click on the green "Code" button.
    - Select "Download ZIP."
    - Save the ZIP file to a convenient location on your computer.

    ```plaintext
    GitHub Repository: https://github.com/LiliaFramework/Lilia
    ```

---

## Step 3: Extracting Lilia

1. **Locate the Downloaded ZIP File:**

    Find the `Lilia-main.zip` file you downloaded.

2. **Extract the Contents:**

    - Right-click the ZIP file and select "Extract All."
    - Choose a temporary folder for extraction.

3. **Organize the Extracted Files:**

    - After extraction, you should see several files and a folder: `lilia`.
    - Move the `lilia` folder to a separate location for easy access during the upload process.

---

## Step 4: Uploading Lilia to Your Server

1. **Connect to Your Server:**

    Use an FTP or SFTP client (e.g., [FileZilla](https://filezilla-project.org/) or [WinSCP](https://winscp.net/eng/index.php)) to connect to your Garry's Mod server.

2. **Navigate to the Gamemodes Directory:**

    - Go to `garrysmod/gamemodes` within your server's file structure.

3. **Upload the Lilia Folder:**

    - Upload the `lilia` folder you extracted earlier into the `gamemodes` directory.

    ```plaintext
    Server Directory Path:
    garrysmod/gamemodes/lilia
    ```

---

## Step 5: Configuring Lilia

1. **Backup Default Configuration:**

    Before making any changes, create a backup of the default configuration files to prevent data loss.

2. **Edit the Configuration File:**

    - Locate the configuration file, typically found at `schema/config/Shared.lua`.
    - Open the file in a text editor.

3. **Override Default Values:**

    Modify the configuration to suit your server's needs. For example, you can change default settings, adjust gameplay mechanics, or set up custom options.

---

## Step 6: Starting Lilia on Your Server

1. **Restart the Server:**

    After uploading and configuring Lilia, restart your Garry's Mod server to apply the changes.

2. **Verify the Installation:**

    - Check the server console for any error messages related to Lilia.
    - Ensure that the server starts without issues and that Lilia is active.

    ```plaintext
    Console Output Example:
    [Lilia] Loaded after X seconds.
    ```

---

## Step 7: Installing Roleplay Schemas

To enhance your roleplaying experience, install a roleplay schema compatible with the Lilia framework. Follow these steps:

1. **Choose a Schema:**

    Select a schema that fits your server's theme from the available options:

    - [Skeleton Schema](https://github.com/LiliaFramework/Skeleton)
    - [MafiaRP Schema](https://github.com/LiliaFramework/MafiaRP)
    - [1942RP Schema](https://github.com/LiliaFramework/1942RP)
    - [HL2RP Schema](https://github.com/LiliaFramework/HL2RP)
    - [MetroRP Schema](https://github.com/LiliaFramework/MetroRP)
    - [SCPRP Schema](https://github.com/LiliaFramework/SCPRP)
    - [KaiserReichRP Schema](https://github.com/LiliaFramework/KaiserReichRP)
    - [FalloutRP Schema](https://github.com/LiliaFramework/FalloutRP)
    - [Public Modules](https://github.com/LiliaFramework/Modules)

2. **Download the Schema:**

    - Visit the chosen schema's GitHub repository.
    - Download the ZIP file or clone the repository.

3. **Extract and Upload:**

    - Extract the schema files to a temporary folder.
    - Upload the schema folder to your server's `garrysmod/gamemodes` directory.

    ```plaintext
    Server Directory Path:
    garrysmod/gamemodes/<SchemaName>
    ```

4. **Configure Factions, Items, and Modules:**

    - Navigate to the schema's configuration files (e.g., `schema/config/Shared.lua`).
    - Customize factions, items, and modules as required to match your server's gameplay mechanics.

5. **Set the Startup Gamemode:**

    - Edit your server's startup configuration to set the gamemode to the newly uploaded schema.
    - This is typically done in the server's launch parameters or configuration files.

    ```plaintext
    Example Server Launch Parameter:
    +gamemode <SchemaName>
    ```

6. **Restart the Server:**

    - Restart your Garry's Mod server to apply the new schema.
    - Verify that the schema loads correctly and that all configurations are active.

---

## Conclusion

Congratulations! You've successfully installed Lilia and set up a roleplaying schema on your Garry's Mod server. Lilia offers a wide range of features and customization options to enhance your roleplaying experience. Be sure to explore the [Lilia Documentation](https://github.com/LiliaFramework/Lilia/blob/main/docs/README.md) and community resources to maximize the potential of your server.

Enjoy your customized roleplaying environment!

---