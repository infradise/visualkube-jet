# Change Log

## 0.10.0
### Added
- **K8s Resource Expansion**
  - Network: Port Forwarding  
  - Access Control: Pod Security Admissions  
  - Metric: Node Metrics, Pod Metrics  
  - Helm: Charts, Releases

## 0.9.0
### Added
- **K8s Resource Expansion**
  - Access Control: Service Accounts, Cluster Roles, Cluster Role Bindings, Roles, Role Bindings, Certificate Signing Requests

## 0.8.0
### Added
- **K8s Resource Expansion**
  - Admin: Custom Resource Definitions, Priority Classes, Runtime Classes, Mutating Webhook Configurations, Validating Webhook Configurations
  - Storage: Persistent Volumes, Persistent Volume Claims, Volume Attachments, Storage Classes, CSI Drivers, CSI Nodes, CSI Storage Capacities

## 0.7.0
### Added
- **K8s Resource Expansion**
  - Network: Endpoint Slices, Endpoints, Ingress Classes, Network Policies
  - Config: HPA, Limit Ranges, Resource Quotas, Pod Disruption Budgets, Leases, Flow Schemas, Priority Level Configurations

## 0.6.0
### Added
- **K8s Resource Expansion**  
  - Cluster: Nodes, Namespaces, Events, API Services, Component Statuses, Cluster CIDR, Cluster Network  
  - Workloads: Daemon Sets, Stateful Sets, Replica Sets, Controller Revisions, Replication Controllers, Jobs, Cron Jobs, Pod Templates
- **Realtime Watch**: All supported Kubernetes resources now include realtime watch functionality.

## 0.5.0
### Added
- **True Cloud-Native IDE**  
  Smooth updates even with thousands of resources. Transitioned from static on-demand pulling to a **Reactive event-driven architecture**, enabling real-time resource watching.
- **Real-time Resource Watch**  
  Introduced live monitoring for key Kubernetes (K8s) resources:
  - Workloads: Pods, Deployments  
  - Network: Services, Ingresses  
  - Config: Secrets, ConfigMaps
- **K8s Resource Expansion**  
  Expanded supported resources:
  - Network: Ingresses  
  - Config: Secrets, ConfigMaps
- **K8s Navigation Tree**  
  Now fully expands by default.  
  Enables unified management of **Deployments**, **Services/Ingresses**, and **ConfigMaps/Secrets**.

### Removed
- **Kubectl Dependency**  
  - Log: No longer requires kubectl to use the log command. Works out-of-the-box.

### Planned
- **Kubectl Dependency**  
  - Shell: Upcoming releases will eliminate the dependency on kubectl exec command.

## 0.4.0
### Added
- **Shell**: Interactive Shell (Terminal) with PTY (Pseudo Terminal) support
- **Shell Auto-Close**: The shell tab automatically closes when the user types "exit"
- **UI Enhancements**
  - **Pod Status**
    - **Status Icons & Text**: Displays colored icons for status: Running (Green), Pending (Orange), Error (Red) to improve readability. Text color is also updated accordingly.
    - **QoS Column**: Added a QoS header to the Pod column.
    - **Table Styling**: Adjusted row height and spacing to provide a more native look and feel.
  - **Resources**
    - **Asynchronous Loading**: Applied async loading to prevent UI freezing while fetching data. Displays a "Loading..." state during data retrieval and also when switching namespaces.
- **K8s Resource Expansion**: New resource introduced — Deployments, Services

## 0.3.0
### Added
- Popup Menu & Mouse Events
  - Right-click on a K8s resource item in the Tree View now provides options:
    - **Open in Existing Tab**: Opens the resource in the dedicated **K8s Resource** tab.
    - **Open in New Tab**: Opens the resource in a new tab, with the tab name set to the resource type (e.g., *Pods*, *Deployments*).
  - Single-click on a resource item replaces the content in the existing **K8s Resource** tab.
  - Double-click on a resource item opens it in a new tab with the resource name.
- Tab Separation
  - **Cluster Manager** now uses its own dedicated tab.
  - **K8s Resources** are displayed in separate tabs, independent of the Cluster Manager.
- Tab Naming for Resources
  - When opened in a new tab, the tab title reflects the resource type (e.g., *Pods*, *Deployments*).
### Fixed
- Improved tab handling logic for resource navigation.
- Resolved (from 0.2.0 Known Issues): Tabs did not automatically refresh; users previously had to close tabs manually. This issue has been resolved.

## 0.2.0
### Added
- Multi-Cluster support (clusters are connected and added when double-clicked in the Cluster Manager)
- Automatic reconnection to the most recently connected multi-clusters (if no previously connected cluster exists, the current context in '~/.kube/config' is used)
### Known Issues
- Tabs are not automatically refreshed, so they must be closed manually

## 0.1.0
### Added
- Initial release