How a Backend App REALLY Runs (Concept – 15 min)

When you run:

npm run start


What actually happens:

OS assigns a process

App binds to a port

App loads env variables

App starts listening for requests

-> DevOps job = make sure this never breaks in production

CI/CD = Continuous Integration + Continuous Delivery/Deployment:
-----------------------------------------------------------------
It is an automated pipeline that takes your code:

Code → Test → Build → Deploy


without manual effort.

CI – Continuous Integration
------------------------------
What it means

Developers continuously merge code into a shared branch (usually main).

Each time code is pushed:

Code is built

Tests are run

Errors are caught early

CD – Continuous Delivery / Deployment
-------------------------------------------
CD has TWO meanings 👇
1️⃣ Continuous Delivery

Code is always ready to deploy

Deployment needs manual approval

Flow:

CI passed → ready → click deploy


Used when:

Banking

Enterprise apps

Production safety needed

2️⃣ Continuous Deployment

Code is automatically deployed

No manual approval

Flow:

CI passed → auto deploy 🚀


Used when:

Startups

Fast-moving products