# Projects

(See [Project Ideas](/projectideas) page for some ideas for projects.)

### Minimal TLS

[**Project Site**](https://github.com/cmalekpour/minimal-tls)  
Team members: <a href="https://github.com/FreddieJin">Tianyi Jin</a>, <a href="https://github.com/cmalekpour">Cyrus Malekpour</a>, <a href="https://github.com/bhuvanesh8">Bhuvanesh Murali</a>, <a href="https://github.com/drs5ma">Daniel Saha</a>  

**Problem.** In recent years, TLS implementations have been targeted with memory corruption or leakage issues, which they are vulnerable. Since they are implemented in C/C++, it is difficult to make these implementations resistant to such attacks. Many implementations also attempt to include a wide variety of cipher suites, which drastically increases the amount of crypto code that needs to be audited and written securely.

**Goal.** We plan to create a "minimal" implementation of TLS with the goal of 95% support of browser clients. To accomplish this, we will identify the least possible set of server features and cipher suites we can support to meet this goal, with a strong focus on security. We will implement only a few key TLS extensions (ex: SNI, OCSP) with fail-safes for other features. The project will be written in the Rust programming language to provide good performance while removing the risk of memory corruption attacks.