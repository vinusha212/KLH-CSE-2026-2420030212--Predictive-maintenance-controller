
# Edge AI Predictive Maintenance Controller for Industry 5.0

## Project Overview

The **Edge AI Predictive Maintenance Controller for Industry 5.0** is an RTOS-based, simulation-driven project designed to monitor industrial machine conditions in real time and predict possible machine failures before they occur.

The system uses simulated **temperature, vibration, and current** sensor data. Python and TensorFlow Lite are used/planned for data processing and AI/ML-based failure prediction. MQTT is used for transferring sensor data between system components, RT-Linux supports real-time processing, Docker provides a consistent software environment, and Grafana is used to display machine conditions and prediction results through a dashboard.

---

## Team Details

| Role          | Name                     | ID         |
| ------------- | ------------------------ | ---------- |
| Team Member   | A. Sharvani              | 2420090052 |
| Team Member   | K. Anjali                | 2420030170 |
| Team Member   | M. Vinusha               | 2420030212 |
| Project Guide | Dr. Srikanth Cherukuvada | —          |

### Project Guide

**Dr. Srikanth Cherukuvada**
Assistant Professor
Department of Computer Science and Engineering
KLH CSE Bowrampet Campus

> **Note:** The Review-1 PPT lists `2420030170` for both K. Anjali and M. Vinusha. Please verify M. Vinusha's ID before the final submission.

---

## GitHub Repository

**Repository Name:**

`KLH-CSE-2026-27-2420030170-PredictiveMaintenanceController`

**Repository Link:**

https://github.com/AnjaliKasarla/KLH-CSE-2026-27-2420030170-PredictiveMaintenanceController

---

## Team Member GitHub Links

The available project materials do not provide individual GitHub profile links. Add the actual profile links below:
---

## Project Guide

**Dr. Srikanth Cherukuvada**
Assistant Professor
Department of Computer Science and Engineering
KLH CSE Bowrampet Campus

---

## Problem Statement

In Industry 5.0, machines continuously generate data such as **temperature, vibration, and current**. If abnormal changes in these values are not detected in time, they can cause machine failures, production delays, and increased maintenance costs.

The **Edge AI Predictive Maintenance Controller** aims to solve this problem by monitoring machine data in real time and predicting possible failures before they happen.

Python and TensorFlow Lite are used for data processing and the AI model, while MQTT transfers sensor data between system components. RT-Linux supports real-time processing. Docker provides a consistent software environment, and Grafana displays machine conditions and prediction results through a dashboard.

---

## Objectives

* To simulate temperature, vibration, and current sensor data from industrial machines.
* To monitor machine conditions in real time using RTOS concepts.
* To implement task scheduling and prioritization for timely sensor-data processing.
* To use AI/ML techniques to detect abnormal machine behavior and predict possible failures.
* To use queues, semaphores, and mutexes for communication and synchronization between RTOS tasks.
* To generate early maintenance alerts to reduce machine failures, downtime, and maintenance costs.

---

## Technology Stack

| Technology      | Purpose                                  |
| --------------- | ---------------------------------------- |
| Python          | Data processing                          |
| TensorFlow Lite | AI/ML model                              |
| MQTT            | Sensor-data communication                |
| RT-Linux / RTOS | Real-time processing                     |
| Docker          | Consistent software environment          |
| Grafana         | Monitoring dashboard                     |
| AI/ML           | Failure prediction and anomaly detection |

---

## Research Gap

The project identifies the following research gaps:

* Most existing studies focus mainly on AI-based prediction but give less attention to real-time task handling.
* Only limited work combines Edge AI with RTOS for predictive maintenance.
* Many existing systems depend on cloud or edge-cloud processing, which can cause delays in quick maintenance decisions.
* There is limited research on predictive maintenance systems designed for resource-limited real-time environments.
* RTOS features such as task scheduling, priorities, queues, and synchronization are not widely explored in existing predictive maintenance solutions.
* Many studies use only single sensor data, while combining temperature, vibration, and current can provide a better view of machine health.

---

## Innovation, Creativity, and Novelty

* Combines **Edge AI and RTOS** to support faster and real-time machine condition monitoring.
* Uses **temperature, vibration, and current** data together instead of depending on a single sensor.
* Uses RTOS task scheduling and priorities to process sensor data within the required time.
* Uses local Edge AI processing to reduce dependence on cloud-based decision-making.
* Provides early maintenance alerts by detecting abnormal machine conditions before major failure.
* The system is software-based and simulation-driven, making it low-cost, safe, and easy to test without physical industrial equipment.

---

## Feasibility

### Technical Feasibility

* The project can be developed using RTOS concepts and a software simulation environment.
* Temperature, vibration, and current values can be simulated as sensor data.
* Python and AI/ML techniques can be used for data processing and failure prediction.
* The system can be tested without physical industrial hardware.

### Economic Feasibility

* No additional cost is required for physical sensors, motors, or microcontrollers.
* Open-source software and tools can be used for RTOS simulation and ML development.
* The project can be developed using an existing computer, making it low-cost.

---

## System Concept

The proposed system follows this general flow:

```text
Industrial Machine Sensor Data
            |
            v
  Temperature / Vibration / Current
            |
            v
       MQTT Communication
            |
            v
       RTOS / RT-Linux
            |
     +------+------+
     |             |
     v             v
Task Scheduling   Synchronization
     |          Queues/Semaphores/
     |             Mutexes
     +------+------+
            |
            v
       Edge AI / ML Model
            |
            v
   Abnormality Detection
            |
            v
   Failure Prediction
            |
            v
    Maintenance Alert
            |
            v
       Grafana Dashboard
```

---

## Project Phases

### 1. Requirement Analysis

Understand the problem, study RTOS and predictive maintenance, and decide what machine parameters to use.

### 2. System Design

Plan the system flow, RTOS tasks, task priorities, and AI model.

### 3. Data & AI Model

Generate sensor data, prepare normal and faulty data, and train the ML model.

### 4. RTOS Implementation

Create RTOS tasks, manage task priorities, and use queues and synchronization methods.

### 5. Integration & Testing

Connect the AI model with the RTOS tasks and test the system with different machine conditions.

### 6. Results & Documentation

Analyze the results, make improvements, prepare the documentation, and complete the final presentation.

---

## Repository Structure

The repository follows the required project structure:

```text
KLH-CSE-2026-27-2420030170-PredictiveMaintenanceController/
│
├── src/
│   └── Source code
│
├── docs/
│   └── Project documentation
│
├── data/
│   └── Sensor / dataset files
│
├── results/
│   └── Experimental results
│
├── reports/
│   └── Review reports and presentations
│
└── README.md
```

If a dataset cannot be committed because of licensing or size restrictions, a documented data-source reference should be provided instead.

---

## GitHub Contribution Guidelines

* Every team member must commit using their **own GitHub account**.
* Individual contributions should be verifiable from the Git commit history.
* Bulk uploads by a single team member should be avoided.
* Commits should be made progressively throughout the project.
* Maintain at least **one meaningful commit per week per team**.
* Each phase deliverable should be tagged appropriately.

Example tags:

```text
review-1
review-2
final
```

### Security

The following must **not** be committed to the repository:

* Passwords
* Credentials
* API keys
* Licensed datasets
* Confidential institutional data
* Other sensitive information

---

## Current Project Status

**Current Phase:** Review-1

**Project Review:** RTOS Project Review-1

**Review Date:** August 13, 2026

The current Review-1 presentation covers:

* Problem Statement
* Objectives
* Literature Survey
* Research Gap Identification
* Innovation, Creativity, and Novelty
* Feasibility
* Project Phases

---

## Literature Survey

The Review-1 presentation discusses the following research works:

### 1. N. Ong et al.

**Title:**
*Predictive Maintenance for Edge-Based Sensor Networks: A Deep Reinforcement Learning Approach*

**Key Idea:**
Edge-based sensor networks and deep learning can support real-time predictive maintenance and equipment failure detection.

**Future Work:**
Practical deployment on constrained RTOS-based controllers can be explored further.

### 2. M. K. et al.

**Title:**
*Resource-efficient Edge AI Solution for Predictive Maintenance*

**Key Idea:**
ML/DL models can operate on resource-constrained edge devices, and edge processing can reduce latency in maintenance decisions.

**Future Work:**
Further research is required for broader industrial equipment and more resource-constrained real-time environments.

### 3. J. Martinez-Gil et al.

**Title:**
*An Agentic Framework for Rapid Deployment of Edge AI Solutions in Industry 5.0*

**Key Idea:**
Edge AI, local AI inference, and modular architectures can support low-latency industrial decision-making.

**Future Work:**
Further validation is required across different industrial applications.

---

## Expected Outcome

The proposed system is expected to:

1. Generate simulated industrial sensor data.
2. Monitor temperature, vibration, and current in real time.
3. Process sensor data using RTOS task scheduling and prioritization.
4. Detect abnormal machine behavior using AI/ML.
5. Predict possible machine failures.
6. Generate early maintenance alerts.
7. Display machine conditions and prediction results using Grafana.
8. Demonstrate predictive maintenance in a low-cost software simulation environment.

---

## Team Information

### Team Members

**A. Sharvani**
ID: `2420090052`

**K. Anjali**
ID: `2420030170`
GitHub: https://github.com/AnjaliKasarla

**M. Vinusha**
ID: `2420030212`

### Instructor / Project Guide

**Dr. Srikanth Cherukuvada**
Assistant Professor
Department of Computer Science and Engineering
KLH CSE Bowrampet Campus

---

## Acknowledgement

We would like to express our sincere gratitude to **Dr. Srikanth Cherukuvada**, Assistant Professor, Department of Computer Science and Engineering, KLH CSE Bowrampet Campus, for his guidance and support throughout the development of this project.

---

## Project Title

**Edge AI Predictive Maintenance Controller for Industry 5.0**

**Institution:** KLH CSE Bowrampet Campus

**Academic Year:** 2026–2027

**Project Type:** RTOS Project

**Review:** Project Review-1
