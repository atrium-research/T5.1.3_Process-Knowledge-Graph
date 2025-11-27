# 📦 Importing Data into a Local Neo4j Community Edition Instance

## ✅ Requirements
- **[Neo4j Community Edition](https://neo4j.com/deployment-center/?gdb-selfmanaged&community)**
- **[Java 17 or higher](https://www.oracle.com/java/technologies/downloads/)**

---

# 🪟 Windows Installation Guide

## 1. Download Required Files
- Download the `ATRIUM_jstor_data.dump` file from this repository.
- Download the **Neo4j Community Edition `.zip`** from:  
  👉 https://neo4j.com/deployment-center/?gdb-selfmanaged&community

## 2. Extract & Navigate
- Extract the `.zip` file.
- Open the **terminal inside the `bin` folder**.

## 3. Load the Database
Run:

```bash
neo4j-admin database load neo4j --from-path=/path/to/ATRIUM_jstor_data.dump --overwrite-destination=true
```

## 4. Start Neo4j
```bash
neo4j start
```

## 5. Access Your Database
- Open your browser and go to:  
  👉 **http://localhost:7474**
- Default credentials:
  - **Username:** `neo4j`
  - **Password:** `neo4j`

🔧 For more help:  
https://neo4j.com/docs/operations-manual/current/installation/windows/

---

# 🍏🐧 macOS / Linux Installation Guide

## 1. Download Required Files
- Download the `ATRIUM_jstor_data.dump` file from this repository.
- Download the **Neo4j Community Edition `.tar` file** from:  
  👉 https://neo4j.com/deployment-center/?gdb-selfmanaged&community

## 2. Extract & Set Environment Variable
Extract the `.tar` and set your Neo4j home directory:

```bash
export NEO4J_HOME=/path/to/<NEO4J_HOME>
```

## 3. Load the Database
Run:

```bash
neo4j-admin database load neo4j --from-path=/path/to/ATRIUM_jstor_data.dump --overwrite-destination=true
```

## 4. Start Neo4j
```bash
neo4j start
```

## 5. Access Your Database
- Open your browser and go to:  
  👉 **http://localhost:7474**
- Default credentials:
  - **Username:** `neo4j`
  - **Password:** `neo4j`

🔧 For more help:  
https://neo4j.com/docs/operations-manual/current/installation/osx/

---

## 🎉 You're all set!
Your local Neo4j instance should now be running with your imported data.
