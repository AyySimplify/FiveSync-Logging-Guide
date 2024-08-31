# **FiveSync Logging Obfuscated Package Setup Guide**

Welcome to the **FiveSync Logging** setup guide! This guide will walk you through the simple steps to get the logging system up and running on your FiveM server.

## **Step 1: Download the Package**

1. **Download** the **FiveSync Logging Obfuscated Package** from the provided link.
2. **Extract** the contents of the downloaded ZIP file to a location on your computer.

## **Step 2: Drag and Drop**

1. **Drag and drop** the extracted folder into your server's `resources` directory.
   - Your `resources` directory is typically located in the main folder where your server files are stored.

## **Step 3: Configure the Webhooks**

1. Navigate to the **`config.lua`** file within the **FiveSync Logging** folder you just added to your server.
   - This file contains all the necessary configuration settings for the logging system.

2. **Open** the `config.lua` file using a text editor (such as Notepad++ or Visual Studio Code).

3. Locate the section where you need to configure your **Discord Webhooks**.
   - You will see lines similar to the following:
   
   ```lua
   Config = {}

   Config.WebhookURL = "YOUR_DISCORD_WEBHOOK_URL_HERE"
   ```

4. **Replace** `"YOUR_DISCORD_WEBHOOK_URL_HERE"` with the actual URL of the Discord webhook you want to use for logging.
   - To create a webhook, go to your Discord server, navigate to the channel you want the logs to be sent to, click on "Edit Channel," then go to "Integrations" and click "Create Webhook."
   - Copy the webhook URL and paste it into the `config.lua` file.

5. **Save** the changes to the `config.lua` file.

## **Step 4: Start the Resource**

1. Open your server’s **`server.cfg`** file (found in the main directory of your server).

2. **Add** the following line to ensure the logging resource starts when your server is launched:

   ```cfg
   ensure fivesync_logging
   ```

3. **Save** the changes to the `server.cfg` file.

## **Step 5: Start Your Server**

1. **Restart** your FiveM server or **start** it if it’s not running.
2. The **FiveSync Logging** should now be active and start logging events directly to the configured Discord channel.

## **You're All Set!**

That's it! The **FiveSync Logging** is now set up and running on your server. If you encounter any issues or need further assistance, feel free to reach out to our support team or community.

Thank you for choosing **FiveSync Logging**!
