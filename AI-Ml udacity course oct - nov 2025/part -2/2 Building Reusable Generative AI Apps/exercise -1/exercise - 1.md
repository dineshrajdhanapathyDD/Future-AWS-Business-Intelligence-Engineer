Now it’s your turn to build a simple Amazon Q App. This app will help automate one of the tasks a customer service agent might encounter on the phone with a customer who needs assistance.

## Exercise Scenario

-   XYZ Corporation has been struggling to help new call center employees respond to customer requests in a way that meets company communication standards.
-   In this exercise, you’ll use Amazon Q Business to build an app that suggests communication for employees handling customer service questions.

## High Level Steps

1.  Open Amazon Q Business and Navigate to Your Q Business Application Web Experience
2.  Create a Simple Q Business App that Uses General Knowledge

## Detailed Instructions

## Section 1: Setting Up the Environment

This is only needed if you didn't set up the environment in Lesson 1 or if too much time has passed and the environment has reset.

Finally, in Amazon Q Business in the AWS portal click on "Admin Controls and Guardrails". Then click "Edit" under Global Controls. Make sure that "Allow end users to send queries directly to the LLM" is enabled and click "Save at the bottom right corner of page.

**Section 2: Creating a Simple Q Business App that Uses General Knowledge**

1.  Select the Apps button in the navigation area to the left.
2.  In the Amazon Q Apps Creator window, in "Describe what you want your app to do", enter the following prompt:
    1.  "_Create a customer service app to help customer service rep to generate a first response based two inputs: Input 1/ product description; Input 2/ customer's request or complaint; Output card: a response based on company's guideline as followed: Response Structure: 1. Acknowledge & Apologize - Show you understand their concern and apologize for the experience 2. Address Safety - Prioritize safety concerns and advise immediate discontinuation if necessary 3. Take Ownership - Don't make excuses; focus on solutions 4. Provide Clear Next Steps - Offer specific resolution options (replacement, refund, repair) 5. Set Expectations - Give realistic timelines and follow-up commitments 6. Professional Tone - Remain calm, empathetic, and solution-focused Key Guidelines:_  Start with safety - if there's a safety concern, address it immediately  _Offer multiple resolution options when possible_  Be specific about timelines and next steps  _Include direct contact information for follow-up_  Thank them for bringing the issue to your attention  _Use their name and reference their specific situation"._  "
3.  Select the Generate button
4.  In the new app, edit the Output - Response card, confirming that the output uses product detail and complaint detail inputs. In the Source dropdown, choose General Knowledge, and then Save the changes to the card.
5.  Respond to a sample complaint, by entering the description of a product and of a complaint in the input boxes, and selecting the Run button.
    1.  **Customer Service Test Data**
        1.  **Product Description**  ProCut X7 Circular Saw The ProCut X7 is a professional-grade 15-amp circular saw designed for heavy-duty cutting applications. Features include a 7¼" carbide-tipped blade, electronic brake system, LED cut line indicator, and ergonomic grip handle. The saw delivers 5,300 RPM for clean, precise cuts through lumber, plywood, and composite materials. Includes a 2-year manufacturer warranty and comes with a durable carrying case. MSRP: $249.99.
6.  **Customer Complaint**
    1.  **Subject: ProCut X7 Saw - Blade Guard Malfunction - Safety Concern**  Customer: Sarah Martinez
 Order #: PCX7-8842-3301
 Purchase Date: March 15, 2025
 Complaint Date: May 28, 2025 "I purchased the ProCut X7 circular saw two months ago for my home renovation project. After about 20 hours of use, the blade guard started sticking and won't retract properly when I try to make cuts. Sometimes it gets completely stuck and I have to manually force it back, which is really dangerous. Yesterday the guard got jammed mid-cut and caused the saw to kick back - I nearly lost control of it. This is a serious safety issue and I'm worried someone could get seriously hurt. I've tried cleaning it and checking for debris but the problem persists. I expected much better quality from ProCut given the price point. I need this fixed immediately or I want a full refund. I can't use the saw in this condition and I have a deadline to finish my deck project. This has cost me time and money, and I'm honestly questioning whether I can trust ProCut tools anymore. Please contact me ASAP at  [sarah.martinez.home@email.com(opens in a new tab)](mailto:sarah.martinez.home@email.com)  or 555-0892."
7.  Confirm that Q Business produces an appropriate response to this customer issue.
    1.  **Customer Service Response Prompt**  PROMPT FOR CUSTOMER SERVICE REPRESENTATIVE: You are responding to a customer complaint about a product safety issue. Use this framework to draft your response: Response Structure:
    2.  Acknowledge & Apologize - Show you understand their concern and apologize for the experience
    3.  Address Safety - Prioritize safety concerns and advise immediate discontinuation if necessary
    4.  Take Ownership - Don't make excuses; focus on solutions
    5.  Provide Clear Next Steps - Offer specific resolution options (replacement, refund, repair)
    6.  Set Expectations - Give realistic timelines and follow-up commitments
    7.  Professional Tone - Remain calm, empathetic, and solution-focused
    8.  **Key Guidelines:**
        1.  Start with safety - if there's a safety concern, address it immediately
        2.  Offer multiple resolution options when possible
        3.  Be specific about timelines and next steps
        4.  Include direct contact information for follow-up
        5.  Thank them for bringing the issue to your attention
        6.  Use their name and reference their specific situation Escalation Triggers:
    9.  Safety concerns (immediate escalation)
    10.  Requests for refunds over $200
    11.  Mentions of injury or legal action
    12.  Multiple previous complaints from same customer
8.  **Sample Opening:**  "Dear [Customer Name], Thank you for contacting us about the blade guard issue with your ProCut X7. Your safety is our top priority, and I sincerely apologize for this concerning experience..."
\


my local system output 

```
Customer Service Response

# Subject: RE: ProCut X7 Saw - Blade Guard Malfunction - Safety Concern

Dear Ms. Martinez,

Thank you for bringing this serious safety concern to our attention regarding your ProCut X7 circular saw. I sincerely apologize for the blade guard malfunction you've experienced and the dangerous situation it created. Your safety is our absolute highest priority, and I'm deeply concerned about the kickback incident you described.

**IMPORTANT SAFETY NOTICE:**  Please discontinue use of the saw immediately. The symptoms you've described indicate a significant safety hazard that requires immediate attention.

On behalf of ProCut Tools, I take full responsibility for this manufacturing defect. The blade guard sticking issue you've described is unacceptable, especially for a professional-grade tool designed for heavy-duty applications. This falls well short of our quality standards, and I understand how this has impacted your renovation timeline and your trust in our products.

I would like to offer you the following resolution options:

1.  **Immediate Replacement:**  We can ship a new ProCut X7 circular saw to you via expedited shipping (1-2 business days) at no cost.
    
2.  **Full Refund:**  We can process a complete refund of your purchase price ($249.99) within 24-48 hours to your original payment method.
    
3.  **Replacement + Compensation:**  In addition to a replacement saw, we can provide a $50 ProCut store credit and extend your warranty to 3 years in recognition of the inconvenience and safety risk you experienced.
    

Given the nature of this issue and your upcoming deck project deadline, I've already initiated the replacement process. Our quality assurance team will personally inspect your replacement saw before shipping to ensure the blade guard functions perfectly.

A prepaid return shipping label will be emailed to you within the next hour for the return of the defective unit. Your replacement saw will ship as soon as we receive confirmation of your preferred resolution option, regardless of whether we've received the defective unit.

I'll personally follow up with you by phone tomorrow to confirm your preference and answer any questions. In the meantime, please feel free to contact me directly at  [customer.care@procuttools.com](mailto:customer.care@procuttools.com)  or 1-800-555-7233 (ext. 215).

Thank you for your patience and for giving us the opportunity to make this right. We value your business and are committed to restoring your confidence in ProCut Tools.

Sincerely,

[Customer Service Representative Name] Customer Resolution Specialist ProCut Tools Customer Care 1-800-555-7233 (ext. 215)
```