# Vertex AI Traininc Cluster (VTC)


``` VTC was previously known as Vertex Model Development Service (VMDS). ```

## Overview

Vertex AI Training Cluster is a fully managed compute infrastructure designed to streamline distributed machine learning workloads on Google Cloud. It enables the provisioning of scalable, high-performance clusters optimized for training complex models, allowing MLOps teams to execute large-scale jobs with minimal operational overhead and maximized resource efficiency.





Slurm (Simple Linux Utility for Resource Management) is an open-source workload manager and job scheduling system to manage Linux clusters, particularly in HPC (High-Performance Computing) environments.

> "Slurm is an industry standard known for optimized GPU scheduling, automated fault tolerance, and simplified parallel job launch."
> — Vertex AI Managed Training

## Infrastructure

### Supported Regions
Note: Issuing requests to any regions not on this list will cause an API error.

* us-central1
* us-east1
* us-east4
* us-east5
* us-south1
* us-west1
* us-west4
* asia-southeast1
* europe-west1
* europe-west4
* europe-north1

### Supported Machine Types
* A3 (H100/200) and A4 (B200) (with TPU v6e support coming soon)
* a4-highgpu-8g
* a3-ultragpu-8g
* a3-megagpu-8g
* n2 CPU family

### Standardized Framework Options
* NVIDIA NeMo
* NVIDIA NeMo-RL

## Storage Options

### Recommendations
| Options | Profile | Recommendations |
| :--- | :--- | :--- |
| Lustre | Highest Performance, Highest cost | Best for extreme I/O performance. |
| Filestore Zonal | High Performance, Higher Memory Ceilings | Best for demanding workloads needing high memory. |
| Filestore Basic SSD | Good Performance, Lowest Cost | Best for frequent simple jobs. |

### Filestore Service Tiers
| Service tier | Availability | Provisionable capacity | Scalability | Performance | Data protection |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Zonal | Zonal | 1 TiB to 9.75 TiB<br>10 TiB to 100 TiB | Up or down in 256 GiB units<br>Up or down in 2.5 TiB units | Configurable | Backups, Snapshots |
| Basic SSD | Regional | 2.5 TiB to 63.9 TiB | Up only in 1 GiB units | Premium fixed | Backups |

## Strategic Context
| Category | Details |
| :--- | :--- |
| Sales play | Build with Google AI |
| Scenarios | Generative AI, + Agents deck, Generative Media, Managed AI Platform |
| Horizontal pitches | Regionalization and Provisioned Throughput |

## Official Guide
Google Cloud > Doc. > AI and ML > Vertex AI
* [Vertex AI training clusters overview](https://docs.cloud.google.com/vertex-ai/docs/training/training-clusters/overview)
* [Get started with training clusters](https://docs.cloud.google.com/vertex-ai/docs/training/training-clusters/create-cluster)
* Deployment Considerations
  * [Compute resources](https://docs.cloud.google.com/vertex-ai/docs/training/training-clusters/compute-resources)
  * [Networking](https://docs.cloud.google.com/vertex-ai/docs/training/training-clusters/networking)
  * [Storage](https://docs.cloud.google.com/vertex-ai/docs/training/training-clusters/storage)
  * [Orchestration](https://docs.cloud.google.com/vertex-ai/docs/training/training-clusters/orchestration)
  * [Create cluster](https://docs.cloud.google.com/vertex-ai/docs/training/training-clusters/create-cluster)
* [Manage cluster](https://docs.cloud.google.com/vertex-ai/docs/training/training-clusters/manage-cluster)
* [Cluster resiliency](https://docs.cloud.google.com/vertex-ai/docs/training/training-clusters/cluster-resiliency)
* Run workload on cluster
  * [Run prebuilt workloads](https://docs.cloud.google.com/vertex-ai/docs/training/training-clusters/run-prebuilt-workloads)
  * [Visualizing jobs with Vertex AI TensorBoard](https://docs.cloud.google.com/vertex-ai/docs/experiments/tensorboard-overview)


* [Google Cloud Managed Lustre](https://cloud.google.com/products/managed-lustre)
