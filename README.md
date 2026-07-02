GO NOTE TAKER APPLICATION
A robust, CLI-based utility built in Go designed for capturing, processing, and persisting structured user notes. This project demonstrates modular application architecture, strict input validation, data encapsulation, and file system serialization using native Go packages.
Structured Data Encapsulation: Utilizes Go struct types to model note objects with explicit fields for metadata management (Title, Content, and temporal tracking via time.Time).
Factory/Constructor Patterns: Implements a strict constructor function (New()) to instantiate objects, handling data integrity checks and returning explicit errors for invalid inputs.
Custom Method Implementation: Leverages custom receiver methods attached to data models to separate layout logic (Display()) from file-system persistence behaviors.
Streamlined Input Handling: Utilizes advanced buffer management (bufio.Scanner) to gracefully handle multi-word and long-string user inputs without breaking CLI execution.
JSON Serialization & Storage: Marshals local structural data into valid JSON formatting using the standard library encoding primitives, formatting strings safely before staging file output.
Fail-Safe File Persistence: Coordinates file creation operations utilizing os.WriteFile, explicitly managing UNIX file permissions (0644) to enforce systemic security baselines.
🛠️ Core Technologies & Packages
Language: Go (Golang)
Standard Libraries: fmt, os, strings, bufio, time, errors, encoding/json
⚙️ Local Setup Instructions
Prerequisites
Ensure you have Go installed on your machine.

Installation
Clone the repository to your workspace:
git clone [https://github.com/Joshua-codes0/YOUR_REPOSITORY_NAME.git](https://github.com/Joshua-codes0/go.Project 2.git)
