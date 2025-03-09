# .openaiao
Open AIAO is an open standard that enables AI agents to interact with websites through structured metadata, similar to how SEO optimizes for search engines.

# Open AIAO - AI Agent Optimization

## The Open Standard for AI Agent Optimization
AIAO (AI Agent Optimization) is a revolutionary open standard that enables AI agents to seamlessly interact with websites and services using structured metadata. Just like SEO helps search engines understand web content, AIAO makes the internet AI-friendly by providing a standardized protocol for AI-driven automation.

## Why AIAO?
AIAO creates an AI-ready internet by making web content machine-readable, reducing automation overhead for businesses and developers. It is an open and extensible standard designed to support multiple industries.

## What is AIAO?
AIAO defines a structured metadata format (JSON-LD) that allows AI agents to:
- Retrieve business information such as hours, services, and contact details.
- Automate tasks like booking appointments and placing orders.
- Interact with industry-specific services, including e-commerce, healthcare, and finance.

## How It Works
1. AIAO-optimized websites expose structured metadata at `/aiao/metadata`.
2. AI agents query this metadata to discover available actions.
3. Automation happens as AI agents execute tasks via defined AIAO endpoints.

### Example AIAO Metadata (JSON-LD)
```json
{
    "@context": "https://aiao.org/context",
    "@type": "AIAOEntity",
    "name": "TechGizmo Repair Shop",
    "description": "An AI-friendly tech repair shop",
    "contact": {
        "phone": "+1-555-123-4567",
        "email": "support@techgizmo.com",
        "website": "https://techgizmo.com"
    },
    "services": [
        {
            "@type": "AIAction",
            "name": "Get Business Hours",
            "endpoint": "/aiao/hours",
            "methods": ["GET"]
        }
    ]
}
```

## Get Started
### Implement AIAO on Your Website (Coming Soon)
Add an `/aiao/metadata` endpoint with structured JSON-LD data. Refer to the [AIAO API Starter Guide](https://github.com/OpenAIAO/docs) for setup instructions.

### Build an AI Agent that Uses AIAO (Coming Soon)
Develop an AI assistant that reads AIAO metadata and automates tasks. Refer to the [Python AI Agent Example](https://github.com/OpenAIAO/ai-agent) for guidance.

### Contribute to the Open Standard
AIAO is a community-driven initiative. Join the discussion and contribute to improving the standard on GitHub.

## Join the Movement
Website: [https://openaiao.org](https://openaiao.org)  
GitHub: [https://github.com/OpenAIAO](https://github.com/OpenAIAO)  
X (coming soon): [https://x.com/openaiao](https://x.com/openaiao)  

## License
AIAO is open-source under the Apache 2.0 License. Contributions are welcome.

---
Open AIAO - Making the web AI-friendly, one website at a time.
