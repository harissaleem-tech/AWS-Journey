# AWS Cloud & DevOps Projects

## 🛠️ Real-Time Production AWS Project
This project shows how to securely deploy web applications inside AWS following production security standards. Instead of putting servers directly on the internet, everything is isolated to keep data safe.

### How the Setup Works
- **Secure Network:** Built a custom VPC split into public and private areas across two different data centers (Availability Zones). If one data center has an issue, the app stays online.
- **Hidden Servers:** Placed the application servers inside the private subnet. They have no public IP addresses, meaning nobody from the internet can access them directly.
- **Traffic Balancing:** Put an Application Load Balancer in the public subnet. When a user visits the app, the load balancer receives the request on Port 80 and passes it safely to the backend servers on Port 8000.
- **Safe Internet Access:** Deployed a NAT Gateway in the public subnet. This lets our private servers securely download software updates from the internet without exposing their real identity to the outside world.
- **Secure Maintenance:** Launched a Bastion Host (Jump Box) in the public subnet. This is the only entry point that allows me to SSH into the private servers securely using my terminal for updates or fixes.
- **Automated Deployment:** Used an Auto Scaling Group with a launch template to automatically keep two Ubuntu servers running and managing the application workload cleanly.
