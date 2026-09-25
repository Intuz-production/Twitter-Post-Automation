*Intuz — Your automation partner, one workflow at a time.*

<p align="center">
  <picture>
    <img alt="Banner Image" src="https://github.com/user-attachments/assets/210f97fc-0fce-404a-b647-7dfe1302cd37" />
  </picture>
</p>

[Intuz](https://www.intuz.com) helps organizations orchestrate AI, automation, and enterprise systems through scalable workflows. Our repository showcases proven implementations across healthcare, operations, customer support, document processing, sales, and back-office functions, enabling teams to accelerate automation initiatives without starting from scratch.

[N8N Creator](https://n8n.io/creators/intuz/) · [Generative AI Development](https://www.intuz.com/generative-ai-development/) · [AI Chatbot Development](https://www.intuz.com/ai-agents-for-business-automation/) · [For Custom Workflow Automation](https://www.intuz.com/get-started/)

# Automate Twitter posting with GPT-4 content generation & Google Sheets tracking

This n8n template from Intuz provides a complete and automated solution for creating an autonomous social media manager.

This workflow uses an AI agent to intelligently generate unique, high-quality content, check for duplicates, and post it on a consistent schedule to automate your entire Twitter presence.

## Who’s this workflow for?

- Social Media Managers
- Marketing Teams & Agencies
- Startup Founders & Solopreneurs
- Content Creators

## How it works

1. **Runs on a Schedule:** The workflow automatically starts at a set interval (e.g., every 6 hours), ensuring a consistent posting schedule.

2. **AI Generates a New Tweet:** An advanced AI Agent, powered by OpenAI, uses a detailed prompt to craft a new, engaging tweet. The prompt defines the tone, topics, character limits, and hashtags.

3. **Checks for Duplicates:** Before finalizing the tweet, the AI Agent is equipped with a tool to read a Google Sheet containing a log of all previously published posts. This allows it to ensure the new content is always unique.

4. **Posts to Twitter (X):** The final, unique tweet is automatically posted to your connected Twitter account.

5. **Logs the New Post:** After posting, the workflow logs the new tweet back into the Google Sheet, updating the history for the next run. This completes the autonomous loop.

## Setup Instructions

1. **Schedule Your Posts:** In the **Start Workflow (Schedule Trigger)** node, set the frequency you want the workflow to run (e.g., every 6 hours).

2. **Connect OpenAI:**
   - Add your OpenAI API key in the **OpenAI Chat Model** node.
   - Customize the prompt in the **AI Agent** node to match your brand’s voice, target keywords, and specific URLs.

3. **Configure Google Sheets:**
   - Connect your Google Sheets account.
   - Create a sheet with two columns: `Tweet Content` and `Status`.
   - In both the **Get Data from Google Sheet** and **Add new Tweet to Google sheet** nodes, select your credentials and specify the Document ID and Sheet Name.

4. **Connect Twitter (X):**
   - In the **Create Tweet** node, connect the Twitter account where you want to post.

5. **Activate Workflow:**
   - Save the workflow and toggle the **Active** switch to ON. Your AI social media manager is now live!

## Key Requirements to Use This Template

Before you start, please ensure you have the following accounts and assets ready:

- **An n8n Instance:** An active n8n account (Cloud or self-hosted) where you can import and run this workflow.
- **OpenAI Account:** An active OpenAI account with an API Key. You will need to have billing enabled to use the language models for tweet generation.
- **Google Account & Sheet:** A Google account and a pre-made Google Sheet. The sheet must have two specific columns: `Tweet Content` and `Status`.
- **Twitter (X) Developer Account:** A Twitter (X) account with an approved Developer profile. You need an App created within the Developer Portal with the necessary permissions (v2 API access with Write scopes) to post tweets automatically.

## FAQ

**Is this template free to use?**
Yes. It's an open-source n8n workflow published by Intuz — copy the workflow JSON from this repo and import it into your own n8n instance at no cost.

**Do I need a paid n8n plan to run this?**
No. It runs on n8n's free self-hosted Community Edition or on n8n Cloud. You'll need your own credentials for OpenAI, Google Sheets, and Twitter (X), not a specific n8n pricing tier.

**Does it post tweets automatically, or just draft them?**
It posts automatically. On each scheduled run the AI generates a unique tweet, checks Google Sheets so it isn’t a duplicate, publishes it to Twitter (X), then logs the post back to the sheet.

## Related n8n templates from Intuz

- [Automate LinkedIn post creation with image using Google Gemini & DALL-E](https://github.com/Intuz-production/AI-Powered-LinkedIn-Post-Image-Generator)
- [Automate lead gen & email outreach with Apify, Apollo.io, GPT-4 & Google Sheets](https://github.com/Intuz-production/AI-Lead-Generation-Automation)
- [Hyper-personalize email outreach with AI, Gmail, and Google Sheets](https://github.com/Intuz-production/Cold-Email-Personalization-Automation)

[See all of Intuz's free n8n templates](https://www.intuz.com/n8n-workflow-automation-templates/)

## Connect with us

Intuz is a USA-based AI & workflow automation company with 16+ years of experience building custom AI-enabled workflow automations for SMBs and Enterprises, specializing in agentic AI, LLM integrations, and CRM/ERP sync across Healthcare, FinTech, eCommerce, Manufacturing, and Real Estate.

* **Website:** [https://www.intuz.com](https://www.intuz.com)
* **Email:** [getstarted@intuz.com](mailto:getstarted@intuz.com)
* **LinkedIn:** https://www.linkedin.com/company/intuz/
* **Get Started:** https://n8n.partnerlinks.io/intuz

## For Custom Workflow Automation

[Click here - Get Started](https://www.intuz.com/get-started/)
