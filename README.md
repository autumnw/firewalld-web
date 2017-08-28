# FirewallD Web

## What is it?
This is the WebUI of firewallD. The purposes are:  
1. It is not a simply alternative of firewalld in CLI; It is a centralized 
iptable management which can manage iptables cross multiple servers;
2. It should support tags for each server, then do role based rule and 
access management.

## How it works?
There a two parts in this project:
1. FirewallD agent:  
   This is the agent which is installed in each server along with iptables.
   The agent register to server, accept the command requests from server side;
   Collect status data and send it back to server. 
   Agent communicates with server through REST API.
2. FirewallD web server:
   User access sevice through web browser to view/create/change servers, rules, tags,
   create segment by tags;  
   Server communicates with agents through REST API, collect information from agent,
   compute rules, then send commands to agent to manage the iptables.

## Install
### Server installation

### Agent installation

## Development