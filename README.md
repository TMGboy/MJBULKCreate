Here's the README formatted in Markdown:

# **MJ Bulk Creation Setup Guide**

This guide will walk you through setting up the environment and running the scripts for generating image prompts and creating images in Midjourney.

## **Step 1: Prepare the Environment**

### 1. **Download Python 3.10.6**

- Download the specific version of Python [from this link](https://www.python.org/downloads/release/python-3106/).
- Double-click the installer to begin the installation process (refer to the screenshots for a step-by-step guide).

### 2. **Installation Instructions**

1. **Tick the box** labeled **“Add Python to PATH”**, and click on **“Customize Installation”**.
![STEP 1](https://i.ibb.co/sQNsjnx/image.png "STEP 1")
2. **Unselect** the **“Documentation”** option, and **select all other options**. Then, click **Next**.
![STEP 2](https://i.ibb.co/W0nG9jf/image.png "STEP 2")
3. In the **Advanced Options**, **leave everything as is** and click **“Install”**.
![STEP 3](https://i.ibb.co/TTjXqwq/image.png "STEP 3")

### 3. **Verify Installation**

Once Python is successfully installed, confirm it by running the following command in your terminal:

```bash
py --version
```

---

## **Step 2: Setting Up the Project Files**

### 1. **Download the Source Files**

- Download the file named **“MJ Bulk Creation Source.zip”** and extract it to a folder of your choice.

### 2. **Run the Installer**

- Navigate to the extracted folder and double-click the file named **`install.bat`**.
- This script will set up the required environment for running the scripts.

---

## **Step 3: Running the Scripts**

### 1. **Open Command Prompt**

- Navigate to the folder where you have extracted the project files.
- In the **address bar** of the folder window, type **`cmd`** and hit **Enter**. This will open a command prompt window in that directory.

### 2. **Script Overview**

Below is a brief description of each script and how to use them:

#### 1. **`chatgpt_template.txt`**

- This file contains a **template** for generating image prompts, **one per each Category**.
- Modify this template as needed and follow the provided pattern to create similar templates for different categories.

#### 2. **`gen_prompts.py`**

- After generating image prompts using ChatGPT, **paste them into** the `prompts_input.txt` file (make sure this file is in the same directory).
- Run `gen_prompts.py`, and it will generate a new file named **`prompts.txt`** with the formatted prompts.

```bash
py gen_prompts.py
```

#### 3. **`app.py`**

- This script reads the **`prompts.txt`** file and processes each prompt sequentially.
- It will send the **`/imagine`** command in **Midjourney** to generate the images based on the prompts.

```bash
py app.py
```

---

## **You're All Set!**

Follow the steps above, and you'll be ready to generate image prompts and automate the image creation process using Midjourney.

If you encounter any issues, feel free to reach out for support. Enjoy creating stunning visuals with ease!
