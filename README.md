Hi everyone, my name is Advika Thakur, and I’m a Summer Analyst in the Windows Engineering team here at Goldman Sachs.

Over the past few weeks, I’ve had the opportunity to work on a project that touches something very fundamental — how we manage and migrate desktops across the firm.

Today, I’ll walk you through my work on the Desktop Admin Portal which will  simplify and streamline desktop migrations, especially as we move towards NDS.next and Windows 11.

Before we jump into the portal itself, let’s first go through —what exactly is a desktop migration?

Desktop migrations are the planned transfer of an entire desktop environment—including its operating system, installed applications, and user data—from a current platform to a target platform.

• At Goldman Sachs this covers three main scenarios:

Datacenter realignment – moving virtual desktops  between physical sites.

Operating-system upgrades – for example, Windows 10 to Windows 11.

Platform shift from on-prem NDS to cloud-hosted NDS.next on Azure.

Now that we understand what are desktop migrations 
here comes  Desktop Admin Portal where vision is to have a consolidated interface that orchestrates every phase of Desktop NDS migration

Together, these  modules will give stakeholders a single source of truth and a single point of control.

In the broader vision for the Desktop Admin Portal, my mandate was to kick-start the project and productionize the migration-scheduling workflow that drives every NDS move.


Before diving deeper into the new solution, let’s first answer

Why are we building another portal when we already have one?


Now Coming to how I was able to convert raw feedback into an approve UI.
I began by listing every friction point that surfaced during  migrations scheduling

Next, I built low-fidelity wireframes . The goal was to validate layout and flow before any colour or styling distracted the conversation

then I conducted user walk-throughs to get their feedbacks on the wireframes

Where I refined the wireframes based on their feedbacks and got it approved 


Let me zoom out for a moment and place DAP within our broader strategy.
Last year we launched Windows Central with a single flagship module—Windows Wellness. That component focused on real-time health: patch levels, disk encryption, AV status, all surfaced in one pane of glass.

Riding on that success, Phase 2 of Windows Central starts this year. We’re adding the Desktop Admin Portal—the migration engine you’ve just seen. It slots right next to Windows Wellness, 



In short, Windows Central is a host; each product is a plug-in. That keeps us agile today and future-proof for new modules tomorrow.
Inside that shell we surface two tiles today—Windows Wellness and Desktop Admin Portal—but we can add more over time.

Micro-Frontend UIs

“Each tile loads its own React bundle at runtime. dedicated back-end service. No shared database, no cross-service joins.

