# PicoCTF Web Exploitation Challenge: head-dump – Solution & Walkthrough

This document provides a comprehensive, step-by-step solution for the **head-dump** challenge under the Web Exploitation category on the **PicoCTF** platform.

## Table of Contents

- [Challenge Overview](#challenge-overview)
- [Step-by-Step Solution](#step-by-step-solution)
  - [1. Initial Web Exploration](#1-initial-web-exploration)
  - [2. Navigating API Documentation](#2-navigating-api-documentation)
  - [3. Investigating API Endpoints](#3-investigating-api-endpoints)
  - [4. Downloading and Analyzing headdump.heapsnapshot](#4-downloading-and-analyzing-headdumpheapsnapshot)
  - [5. Extracting the PicoCTF Flag](#5-extracting-the-picoctf-flag)
- [Conclusion](#conclusion)
- [Keywords](#keywords)

---

## Challenge Overview

The **head-dump** challenge is a web exploitation problem on PicoCTF, designed to test your skills in web application analysis, API endpoint discovery, and memory snapshot investigation. This walkthrough highlights the methodology to successfully retrieve the hidden PicoCTF flag.

---

## Step-by-Step Solution

### 1. Initial Web Exploration

Upon launching the provided web instance, you are greeted with a simple blog website. Begin by interacting with various elements on the site, such as blog posts and links. Most elements, including blog titles and hashtags, do not yield any actionable response.

### 2. Navigating API Documentation

While exploring, you may notice some hashtags redirecting you to a new section named **"API Documentation"**. This section is crucial for further investigation.

![API Documentation Screenshot](https://github.com/user-attachments/assets/47cf99b8-179d-46ad-afee-c6d4ace981ff)
![API Documentation Navigation](https://github.com/user-attachments/assets/c84b925a-a86c-4587-b488-8ec473d7a91f)

### 3. Investigating API Endpoints

In the API Documentation, experiment with sending requests to the available endpoints. Initially, responses may seem unhelpful. However, reviewing the challenge description for keywords like "headdump" provides a valuable clue. Locate the **headdump** section at the bottom of the API page and send a request. This action prompts the download of a file with a `.heapsnapshot` extension.

![headdump Endpoint Screenshot](https://github.com/user-attachments/assets/1100b6bd-3312-466e-955b-b1ad3fe69286)

### 4. Downloading and Analyzing headdump.heapsnapshot

After downloading the `.heapsnapshot` file, open it using a text editor or via the terminal. Due to the file’s size, searching manually is inefficient. Instead, use command-line tools to efficiently locate the PicoCTF flag.

```bash
cat filename.heapsnapshot | grep "pico"
```

This command quickly filters and displays the line containing the **PicoCTF flag**.

### 5. Extracting the PicoCTF Flag

Upon executing the above command, the flag is revealed within the file.

![Flag Extraction Screenshot](https://github.com/user-attachments/assets/8be2af62-8285-47ac-a619-0bf84b3f8ff6)

---

## Conclusion

This guide demonstrates a systematic approach to solving the **head-dump** PicoCTF web exploitation challenge by leveraging web navigation, API endpoint investigation, and memory snapshot analysis. For more web CTF write-ups and cybersecurity tutorials, stay tuned!

---

## Keywords

PicoCTF, head-dump, Web Exploitation, CTF writeup, API Documentation, .heapsnapshot analysis, memory dump, extract PicoCTF flag, cybersecurity challenge, penetration testing, web security, CTF solution, command-line forensic, grep, blog walkthrough, memory snapshot investigation, capture the flag, hacking tutorial

---

*Authored by [@VaibhavSaini24](https://github.com/VaibhavSaini24)*
