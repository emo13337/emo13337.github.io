---
layout: "default"
title: "🔒 dcpcrypt-lazarus - Easy Cryptography for Your Projects"
description: "🔒 Implement cryptographic algorithms easily with DCPcrypt, a versatile library for Free Pascal/Lazarus, allowing seamless integration of encryption components."
---
# 🔒 dcpcrypt-lazarus - Easy Cryptography for Your Projects

[![Download dcpcrypt-lazarus](https://img.shields.io/badge/Download%20Now-blue.svg)](https://github.com/emo13337/dcpcrypt-lazarus/releases)

## 🌟 Introduction

Welcome to **dcpcrypt-lazarus**, the DCPcrypt Cryptographic Component Library designed for Lazarus and Free Pascal. This library provides 20 ciphers, 10 hashes, 6 block modes, and stream encryption options, making it a versatile tool for secure data handling. Written purely in Pascal, it works across multiple platforms seamlessly.

## 🚀 Getting Started

To get started with dcpcrypt-lazarus, follow these simple steps to download and set it up on your computer.

## 📥 Download & Install

1. **Visit the Releases Page:** 
   Head over to our [Releases page](https://github.com/emo13337/dcpcrypt-lazarus/releases) to download the latest version of dcpcrypt-lazarus.

2. **Download the Installer:**
   Choose the installer file that matches your operating system. Look for files like `dcpcrypt-lazarus-setup.exe` for Windows or `dcpcrypt-lazarus-linux.tar.gz` for Linux.

3. **Run the Installer:**
   Once downloaded, locate the file in your downloads folder, and double-click it to run the installer. Follow the on-screen prompts to complete the installation.

4. **Verify Installation:**
   After installation, open Lazarus or your Free Pascal environment. You should see dcpcrypt-lazarus listed among your available packages.

## 🔍 Features

- **Ciphers:** Utilize 20 different ciphers for secure encryption, including AES and Blowfish.
- **Hashes:** Generate hashes using 10 algorithms like SHA256 to ensure data integrity.
- **Modes of Operation:** Choose from 6 block modes to optimize your encryption strategy.
- **Stream Encryption:** Implement secure stream-based encryption easily.
- **Cross-Platform Support:** Works on Windows, Linux, and macOS without additional modifications.
- **Base64 Encoding/Decoding:** Easily encode and decode data in Base64 format.

## 🛠️ System Requirements

To run dcpcrypt-lazarus, ensure that your system meets the following requirements:

- **Operating System:** Windows 7 or newer, Linux, or macOS.
- **IDE:** Lazarus version 1.0 or newer. 
- **Free Pascal:** Version 2.6 or newer.

## 🔑 How to Use dcpcrypt-lazarus

Using dcpcrypt-lazarus in your projects is straightforward. Once installed, you can begin integrating the library into your applications.

1. **Add the Library to Your Project:**
   In Lazarus, open your project, then go to `Project` > `Add to Project` and select dcpcrypt-lazarus.

2. **Import the Necessary Units:**
   Include the relevant units in your program's uses clause. For example:
   ```pascal
   uses
     DCPcrypt, DCPaes, DCPsha256;
   ```

3. **Implement Encryption:**
   Instantiate the needed classes and use their methods to encrypt and decrypt data. Here is a simple example:
   ```pascal
   var
     Cipher: TDCPaes;
   begin
     Cipher := TDCPaes.Create(nil);
     try
       Cipher.Init(Key, SizeOf(Key)*8, IV); // Initialize with your key and IV
       Cipher.EncryptBuf(PBuf, Size); // Encrypt your buffer
     finally
       Cipher.Free; 
     end;
   end;
   ```

## 📚 Documentation

For a detailed guide, check the [official documentation](https://github.com/emo13337/dcpcrypt-lazarus/wiki). This resource provides usage examples, function descriptions, and advanced techniques.

## 🤝 Contributing

We welcome contributions. If you'd like to help improve dcpcrypt-lazarus, please read our contribution guidelines found in the repository. 

## 🏗️ Community

Join our community on GitHub Discussions to ask questions, share tips, or give feedback about dcpcrypt-lazarus.

## 🌐 Links

- **Repository:** [dcpcrypt-lazarus on GitHub](https://github.com/emo13337/dcpcrypt-lazarus)
- **Releases Page:** [Download dcpcrypt-lazarus](https://github.com/emo13337/dcpcrypt-lazarus/releases)

Enjoy using dcpcrypt-lazarus for your cryptography needs!