[![JetBrains Plugin Version](https://img.shields.io/jetbrains/plugin/v/com.infradise.visualkube.jet)](https://plugins.jetbrains.com/plugin/29143-visualkube-jet)
[![JetBrains Plugin Downloads](https://img.shields.io/jetbrains/plugin/d/com.infradise.visualkube.jet)](https://plugins.jetbrains.com/plugin/29143-visualkube-jet)

# Visualkube Jet ⚡ 

<div align="center">
  <img src="https://packages.visualkube.com/jet/logo.png" alt="Visualkube Jet Logo" width="128" height="128">
  <br>
  
  <h1>The Native Kubernetes IDE for JetBrains</h1>
  <p>
    <b>Built exclusively for JetBrains IDEs</b><br>
    The native, lightweight Kubernetes management plugin for JetBrains IDEs.
  </p>

  <p>
    <a href="https://github.com/infradise/visualkube-jet/releases/latest">
      <img src="https://img.shields.io/badge/macOS-gray?logo=apple&style=for-the-badge" alt="macOS"></a>  
    <a href="https://github.com/infradise/visualkube-jet/releases/latest">
      <img src="https://img.shields.io/badge/Windows-blue?logo=windows&style=for-the-badge" alt="Windows"></a>
    <a href="https://github.com/infradise/visualkube-jet/releases/latest">
      <img src="https://img.shields.io/badge/Linux-green?logo=linux&style=for-the-badge" alt="Linux"></a>  
  </p>

  <p><img src="https://packages.visualkube.com/jet/screenshot/visualkube-jet-main-screenshot.png" alt="Visualkube Jet Main Screenshot"></p>
</div>


## Introduction

**Visualkube Jet** is a lightweight, high-performance Kubernetes management plugin built exclusively for the JetBrains ecosystem. Written in **Kotlin**, it leverages the native JetBrains UI components to provide a seamless, integrated experience that feels like a built-in part of your IDE.

Unlike the flagship [Visualkube Master](https://github.com/infradise/visualkube), which is a comprehensive cross-platform dashboard, **Visualkube Jet** is laser-focused on developer productivity within Android Studio, IntelliJ IDEA, and PyCharm.

## Why Visualkube Jet?

### Key Features (*Planned*)

* **Native Performance**
    * Built with **Kotlin** and the JetBrains SDK. No web views, no heavy frameworks, and no context switching. It is optimized for speed and minimal resource consumption.
* **Native Look & Feel**
    * We utilize the standard **JetBrains UI components**. Whether you are using the Darkula theme or the new UI, Visualkube Jet blends in perfectly, providing a consistent and comfortable user experience, and an interface designed for long coding sessions.
* **Focus on Essentials**
    * Designed for developers who need to manage Kubernetes clusters without leaving their code. View logs, edit YAMLs, and restart pods directly alongside your source code.

## Supported IDEs

Visualkube Jet is compatible with all IntelliJ Platform-based products (Version 2023.x and later):

* **Android Studio**
* **IntelliJ IDEA** (Community & Ultimate)
* **PyCharm** (Community & Professional)
* PhpStorm, GoLand, WebStorm, CLion, DataGrip, RubyMine, RustRover

> **Note:** This plugin is **NOT** available for VS Code or Eclipse. It is a specialized tool for the JetBrains family.

## Installation

1.  Open your IDE (Android Studio, IntelliJ IDEA, PyCharm, etc.).
2.  Go to **Settings/Preferences** → **Plugins** → **Marketplace**.
3.  Search for **"Visualkube Jet"**.
4.  Click **Install**.

## Getting Started

Follow these steps to test **Visualkube Jet** (0.1.0‑EAP):

### Prerequisites
- kubectl must be installed for version 0.1.0‑EAP.
- Ensure that the Kubernetes cluster is accessible and properly connected.

### Steps to Get Started
1. Click the **Visualkube Jet icon** in the top‑left corner of your IDE.  

2. In the **Visualkube Jet Tool Window**, open the **Cluster Manager** icon from the Visualkube Cluster toolbar.  
   - Verify the Kubernetes cluster list.  
   - The current cluster is marked with a star.  
   - **Note:** In version 0.1.0‑EAP, only the *Current Context* from `~/.kube/config` is accessible.  

3. In the Kubernetes resource tree, expand **Workloads** and click **Pods**.  

4. Use the **Toggle Namespace** icon in the Visualkube Cluster toolbar to filter the Pod list by namespace.  

5. On the right side of the IDE, click the **Visualkube Details icon** to open the YAML viewer.  
   - Select a Pod from the list to display its YAML definition.  

6. At the bottom of the IDE, click the **Visualkube Operations icon** to open the logs window.  
   - Right‑click a Pod in the list and choose **Show Log** from the popup menu to view its logs.

## Feedback & Support

Found a bug? Please let us know!

* **Bug Report:** [Open an Issue](https://github.com/infradise/visualkube-jet/issues/new)

---

## Legal Notices

© 2025 Infradise Inc. All rights reserved.  

**Visualkube**, **Visualkube Master**, and **Visualkube Jet** are products of Infradise Inc.  

We are **not affiliated with** The Linux Foundation, Microsoft Corporation, or JetBrains s.r.o.  

All other trademarks cited herein are the property of their respective owners.  
For full legal details and a comprehensive list of third-party trademarks, please visit our [Legal Notices](https://jet.visualkube.com/legal).