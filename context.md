I want to find my next job but im not sure what to look for or what to do, asssist me by asking questions breaking down and
exposing my gaps as to fill them in. let's start, currently im a "operational mananger" for a startup crypto ATM company. My job
consist of ensuring machines are always online without any problems and if there are i use contractors through fieldnation to
troubleshoot the machine. Recently i started to use VS code/cursor to "vibe code" automating and enhancing my workflow to increase productivity for not just myself by knowing when an issue occurs but also helped finance team so cashflow tracking can be easily
documented, have created projects to gather more google reviews using sophisicated programs that are used to send notifications to clients who got their funds within a "acceptable time frame" with a google review link an entire dashboard made to track when
clicks are done and mark completed reviews for clients to not spam with them reviews and much more. I 'm also Comptia A+ and
Security+ certified.

i mainly use Nodejs as i find it clean to work with, second up would be Python 2) I manage over 500 machines, on a typical daywe can have between 5 to 15 issues requiring techs from all over the country. 3) some complex projects:  Node.js application that:

Monitors Bitcoin ATM transactions
Verifies blockchain confirmations
Manages customer review requests
Sends notifications via Telegram and email
Tracks review submission status
Key Features
Automated transaction monitoring
Multi-cryptocurrency support (BTC, ETH, USDC, USDT, LTC)
Blockchain confirmation checks
Review request management
Telegram and email notifications
Google My Business review tracking
link click tracking Kiosk Monitoring Dashboard
A real-time monitoring system for tracking kiosk statuses, issues, and analytics.

Key Components
Ops.js: Background workflow that:

Monitors kiosk statuses via API
Detects offline kiosks and hardware issues
Updates offlineKiosks.json with current status
Sends Telegram notifications for critical issues
Runs every 10 minutes (scheduled)
dashboard.js: Express.js server that:

Serves the frontend web dashboard
Provides REST API endpoints for data
Uses Socket.IO for real-time updates
Watches offlineKiosks.json for changes
Maintains historical issue data in SQLite
Frontend Dashboard:

Real-time status overview
Interactive map and charts
Issue tracker and analytics
Notification system. I love solving problems, but i love even more is optimzing people's workflow with the use of software using AIcoding agents (i have little coding knowledge) the operaiontal stuff is pretty okay but not something i love, don't get me wrong
it's great to see something get fixed. im currenly more of my own but there is a team behind me. But because im the only one with
knowledge of coding/AI/automation im on my own in that regards, i setup all the optimization,troubleshooting on codes on my own. imopen to other industries where your ops + automation skills would be valuable?

i use cursor, github copilot (recently), Gemini CLI (claude alterantive), vs code. for my monitoring system everything is local, since the company doesn't pay for hosting i come up with ways to solve that solution for example using loca.lt tunnel to push a
port to the public and share that dashboard with others. I use SQLite3 for tracking purposes but haven't found much more use
outside of it and probably really basic. no experiance with Grafana or Prometheus. I use APIs for almost all my projects even tho i

don't got offical API documents i kind of reverse enginnered it by going through the frontend listning to the network and creating a API breakdown to make request/pushes etc that i could with the auth token given, with a flow to reauthenticate once it's expired to carry on. I don't mind joining a team of becoming an automation expert.


im currently making 65k after a recent bump from 55k. I was hired as a support desk tech, moved onto operationals basically
became a manager on there than started to "vibe code" and found myself being requested to make a bunch of thigns for the company to

drive sales, automation, reviews etc. I want to leave and find something over 90k i'm also currently still in school working on AAS

(1 class left) than starting my BS. I'd like to transition within the next 3 months. I want Fast-track into a role and learn on the

job. Open to remove work or local doesn't matter.

Project Title: ATM Transaction Monitoring & Customer Review Automation System

1. Problem Solved & Business Impact

Problem: A manual and inconsistent process for collecting customer feedback post-transaction for Bitcoin ATM services, leading to
missed opportunities for service improvement and reputation management.
Solution: An automated system that monitors ATM transactions, verifies their completion (including blockchain confirmations), and
proactively solicits customer reviews via integrated communication channels (Telegram, Email using Zendesk). It tracks the entire
review lifecycle, from request initiation to submission, storing all data in local SQLite databases.
Business Impact:
Increased Review Volume: Automates outreach to customers, leading to higher numbers of collected reviews.
Enhanced Customer Engagement: Provides a timely touchpoint with customers immediately after a transaction.
Data-Driven Service Improvement: Gathers direct feedback to identify and address operational issues or service gaps.
Reputation Management: Boosts online presence and customer trust through consistent feedback collection and positive reviews.
Operational Efficiency: Automates manual processes, reducing operational overhead.
2. Technologies Used

Core Language/Runtime: Node.js
Web Framework: Express.js, EJS (for templating the dashboard)
Databases: SQLite3 (utilized for database.db for kiosk information and review_system.db for tracking review requests and statuses) HTTP Requests: fetch API, Axios
Configuration: dotenv (for managing environment variables like API keys and tokens)
Utility: uuid (for generating unique identifiers)
Link Shortening & Tracking: Dub.co, Bitly
Notifications: Telegram Bot API, Zendesk API (for sending email feedback requests)
Blockchain Interaction: Node-fetch, integration with various blockchain explorer APIs (e.g., Mempool.space for BTC, Etherscan.io
for ETH/ERC20, Blockchair.com for LTC) to verify transaction confirmations.
Web Scraping (Implied): Puppeteer (or a similar headless browser automation tool) is used for scraping Google Maps review pages as a fallback or supplement to the GMB API.
3. Architecture Overview

The system is architected as a monolithic Node.js application that orchestrates various tasks. It integrates with external APIs for

transaction data, confirmations, notifications, and link shortening, while also managing local SQLite databases for internal state and kiosk information. i don't got much on github

remember, i didn't code any of this. All AI. i just walk through with it and came up with the entire system.

location Portland, OR. let's update my linkedin with current skill. a complete rebanding.