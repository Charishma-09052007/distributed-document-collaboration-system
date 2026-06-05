# Distributed Document Collaboration System

## Overview

Distributed Document Collaboration System is a distributed file management and collaboration platform that enables multiple clients to access, edit, and manage shared documents across multiple storage servers through a centralized name server.

The system supports concurrent access, document synchronization, access control, caching, and persistence while maintaining consistency across distributed components.

## Features

### Distributed Architecture

* Centralized Name Server
* Multiple Storage Servers
* Multi-client support
* Distributed file management

### Document Operations

* Create documents
* Read documents
* Update document content
* Delete documents
* Document synchronization

### Concurrency Control

* Multi-client access support
* Concurrent document editing
* Lock-based synchronization
* Consistency management

### Access Control

* User authorization
* Permission management
* Secure document access

### Caching

* Frequently accessed document caching
* Reduced storage server load
* Improved response times

### Persistence

* Persistent document storage
* Data recovery support
* Reliable file management

## System Architecture

```text
                +----------------+
                |   Name Server  |
                +----------------+
                        |
        ---------------------------------
        |               |               |
        ▼               ▼               ▼
+----------------+ +----------------+ +----------------+
| Storage Server | | Storage Server | | Storage Server |
+----------------+ +----------------+ +----------------+
        ▲               ▲               ▲
        |               |               |
        ---------------------------------
                        |
                Multiple Clients
```

## Technologies Used

* C
* Socket Programming
* POSIX Threads
* File Systems
* Linux System Calls
* TCP/IP Networking

## Key Components

### Name Server

Responsibilities:

* Client request routing
* Metadata management
* Storage server coordination
* Access control management

### Storage Servers

Responsibilities:

* Document storage
* File operations
* Data persistence
* Client request handling

### Client

Responsibilities:

* Document access
* File operations
* Collaboration requests
* Communication with distributed services

## Core Concepts Implemented

* Distributed Systems
* Client-Server Architecture
* Concurrency Control
* Synchronization Mechanisms
* Distributed Storage
* Access Control
* Caching Strategies
* Fault-Tolerant Design Principles

## How to Build

Compile the project:

```bash
make
```

or

```bash
gcc *.c -o distributed_docs -lpthread
```

## How to Run

### Start Name Server

```bash
./nameserver
```

### Start Storage Servers

```bash
./storage_server
```

### Start Client

```bash
./client
```

## Results

The system demonstrates the design and implementation of a distributed document management platform capable of handling multiple clients, concurrent document access, distributed storage coordination, caching, and persistent data management.

## Highlights

* Distributed Systems Project
* Multi-Server Architecture
* Concurrent Client Support
* Lock-Based Synchronization
* Access Control Mechanisms
* Caching and Persistence
* Socket Programming
* Systems-Level Development
