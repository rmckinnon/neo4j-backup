# neo4j backup and restore
Neo4j utility scripts for backing up and restoring neo4j databases both locally and
remote.

### Motivation
After looking through the documentation for the community version of Neo4j, it 
became apparent that there was no good way to easily backup and restore data. 
This small project is to help fill that gap.

### Technology
The scripts are written in NodeJS. Version 9.10.1 at the time 

### Dependencies
"neo4j-driver": "^1.6.1"

`npm install -g neo4j-driver` 

### Example Usage neo4j-backup.js
```bash
node neo4j-backup.js --help
node neo4j-backup.js -a bolt://localhost:7687 -u neo4j -p changeme -d backup
```