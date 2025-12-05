[![JetBrains Plugin Version](https://img.shields.io/jetbrains/plugin/v/com.infradise.visualkube.jet)](https://plugins.jetbrains.com/plugin/29143-visualkube-jet)

# Visualkube Jet ⚡ 

<div align="center">
  <img src="https://packages.visualkube.com/jet/logo.png" alt="Visualkube Jet Logo" width="128" height="128">
  <br>
  
  <h1>The Native Kubernetes IDE for JetBrains</h1>
  <p>
    The native, high-performance, lightweight Kubernetes management plugin for JetBrains IDEs.<br>
    <b>Built exclusively for JetBrains IDEs</b>
  </p>

  <p>
    <a href="https://github.com/infradise/visualkube-jet/releases/latest">
      <img src="https://img.shields.io/badge/macOS-gray?logo=apple&style=for-the-badge" alt="macOS"></a>  
    <a href="https://github.com/infradise/visualkube-jet/releases/latest">
      <img src="https://img.shields.io/badge/Windows-blue?logo=windows&style=for-the-badge" alt="Windows"></a>
    <a href="https://github.com/infradise/visualkube-jet/releases/latest">
      <img src="https://img.shields.io/badge/Linux-green?logo=linux&style=for-the-badge" alt="Linux"></a>  
  </p>
  <p>
    #Multi-Cluster #Real-Time Watching #Automatic Reconnecting #True Cloud-Native IDE
  </p>

  <p><img src="https://packages.visualkube.com/jet/screenshot/visualkube-jet-multi-cluster-log-v060.png" alt="Visualkube Jet - Multi Cluster Screenshot"></p>

  ![Visualkube Jet Tutorial](https://packages.visualkube.com/jet/tutorial/visualkube-jet-tutorial.webp?raw=true)
</div>

## Introduction

**Visualkube Jet** is a lightweight, high-performance Kubernetes management plugin built exclusively for the JetBrains ecosystem. Written in **Kotlin**, it leverages the native JetBrains UI components to provide a seamless, integrated experience that feels like a built-in part of your IDE.

Unlike the flagship [Visualkube Master](https://github.com/infradise/visualkube), which is a comprehensive cross-platform dashboard, **Visualkube Jet** is laser-focused on developer productivity within Android Studio, IntelliJ IDEA, and PyCharm.

## Why Visualkube Jet?

* **Native Performance**
    * Built with **Kotlin** and the JetBrains SDK. No web views, no heavy frameworks, and no context switching. It is optimized for speed and minimal resource consumption.
* **Native Look & Feel**
    * We utilize the standard **JetBrains UI components**. Whether you are using the Darkula theme or the new UI, Visualkube Jet blends in perfectly, providing a consistent and comfortable user experience, and an interface designed for long coding sessions.
* **Focus on Essentials**
    * Designed for developers who need to manage Kubernetes clusters without leaving their code. View logs, edit YAMLs, and restart pods directly alongside your source code.

## Key Features

- **Architecture:** High‑performance design based on JetBrains Native UI (Swing/Kotlin) and Kubernetes Java Client.
- **Exploration:** Cluster tree view with real‑time namespace filtering via toggle UI.
- **Operations:** Cluster Manager integrated with `~/.kube/config` and reactive Pod list display.
- **Details:** YAML editor that opens automatically on click, with syntax highlighting and scrolling support.
- **Runtime:** Real‑time log streaming through right‑click context menu and automatic popup window.
- **Multi-Cluster** support (clusters are connected and added when double-clicked in the Cluster Manager)
- **Automatic Reconnection** to the most recently connected multi-clusters (if no previously connected cluster exists, the current context in `~/.kube/config` is used)
- **Shell Auto-Close:** The shell tab automatically closes when the user types "exit"
- **True Cloud-Native IDE:** Smooth updates for thousands of resources via transition from static on-demand pulling to reactive event-driven architecture, enabling real-time watching.
- **Real-time Resource Watch:** Live monitoring of key Kubernetes (K8s) resources like Workloads (Pods, Deployments), Network (Services, Ingresses), and Config (Secrets, ConfigMaps).
- **Kubectl-Independent Logs:** Log viewing without kubectl dependency, working out-of-the-box for seamless runtime access.
- **Upcoming Kubectl-Independent Shell:** Planned elimination of kubectl exec dependency in future releases for enhanced shell operations.

## K8s Resource Expansion

New resources are introduced in every version update:

- Cluster: 
  - Nodes, Namespaces, Events, API Services, Component Statuses, Cluster CIDR
- Workloads:  
  - Pods, Deployments, Daemon Sets, Stateful Sets, Replica Sets, Replication Controllers, Jobs, Cron Jobs, Controller Revisions, Pod Templates
- Network:  
  - Services, Ingresses, Endpoint Slices, Endpoints, Ingress Classes, Network Policies
  - (Under review: Port Forwarding)
- Config:  
  - Secrets, ConfigMaps, Horizontal Pod Autoscalers, Limit Ranges, Resource Quotas, Pod Disruption Budgets, Leases, Flow Schemas, Priority Level Configurations
  - (Under review: Vertical Pod Autoscalers)
- Admin:
  - Custom Resource Definitions, Priority Classes, Runtime Classes, Mutating Webhook Configurations, Validating Webhook Configurations
- Storage:
  - Persistent Volumes, Persistent Volume Claims, Volume Attachments, Storage Classes, CSI Drivers, CSI Nodes, CSI Storage Capacities
- Access Control:
  - Service Accounts, Cluster Roles, Cluster Role Bindings, Roles, Role Bindings, Certificate Signing Requests
  - (Under review: Pod Security Policies, Pod Security Admission)
- Metric:
  - (Under review: Node Metrics, Pod Metrics)
- Helm:
  - (Under review: Charts, Releases)

## Supported IDEs

Visualkube Jet is compatible with all IntelliJ Platform-based products (versions 2023.x and later):

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

1. Click the **Visualkube Jet icon** in the top‑left corner of your IDE.

2. The **Cluster Manager** opens automatically by default. (If you closed it, click the **Cluster Manager** icon in the **Visualkube Cluster toolbar**.)
  - In the **Cluster Manager**, multi-cluster lists are added or removed when you double‑click a cluster in the Kubernetes cluster list.
  - The current context is marked with a star.
  - **Note:** Currently, only `~/.kube/config` is accessible.

3. In the **Kubernetes resource tree**, click **Pods** in the **Workloads** group. Then you can watch real-time events (e.g., status changes and latest updates) on the pods.

4. Use the **Toggle Namespace** icon in the **Visualkube Cluster toolbar** to filter the Pod list by namespace.

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