# Exercise 5: Build a Custom Copilot Agent for Project Nexus

### Estimated Duration: 45–60 Minutes

# Lab Overview

In this exercise, you will create a fully custom Microsoft 365 Copilot agent using Agent Builder.

The agent you create will support **Project Nexus executive decision-making**, helping leadership:

* Evaluate adoption metrics
* Assess risks
* Review financial alignment
* Generate rollout recommendations

You will build the agent from scratch (no template).

---

## Task 1: Create and Configure the Agent

1. Open **Microsoft Edge** and navigate to:

    ```
    https://www.microsoft365.com
    ```

2. Sign in and select **New agent**.

3. In the Describe box, enter the following one-line prompt:

    ```
    Create an agent named Project Nexus Governance Advisor that helps executive leaders evaluate adoption metrics, risks, financial alignment, and rollout readiness using internal Project Nexus documents.
    ```

4. Refine the description if prompted by Agent Builder until you are satisfied.

5. If prompted with follow-up questions, refine the description until satisfied.

1. After you enter a description and select the forward arrow, the **Agent Builder** form should appear for your new agent. At the top of the form is a **Describe** tab and a **Configure** tab.

    - The **Describe** tab enables you to carry on a conversation with Agent Builder. This tab is displayed by default.

    - The **Configure** tab enables you to define the detailed settings that drive the agent.

    Wait a minute or two for Agent Builder to create the agent, at which time it displays the agent’s name and description in the **Agent preview** pane.

1. If you didn't provide a name for your agent in the description that you just entered, then Agent Builder typically provides a suggested name and asks you to either confirm the name or provide a new one. You should reply accordingly.

1. At this point, Agent Builder typically prompts you to refine the description for your agent. It does so through a series of questions or suggested prompts. You can optionally respond to each question or select certain prompts until the agent's description is to your liking. 

   >**Note:** The beauty of the Agent Builder process is that it automatically translates your basic, natural language description into a complex set of instructions. This process saves you from creating this detailed instruction set on your own.

1. Once you're satisfied with the agent's description, select the **Configure** tab at the top of the form. Let’s see what Agent Builder did based on your finalized description.

1. On the **Configure** tab, ignore the **Template** and **Agent icon** options for now. In a real-world scenario, you can optionally select a template that you want to base your agent upon, and you can assign your agent a custom icon. Notice how the **Name** and **Description** fields are filled in based on your finalized description. 

1. Scroll down to the **Instructions** field. Agent Builder generated these instructions based on your initial description and the updates that you made to it on the **Describe** tab. Review the detailed level of instructions that Agent Builder generated.

1. If you wish to change the instructions, you can either manually edit them directly in the **Instructions** field, or you can ask Agent Builder to update the instructions for you.  

1. While the current instructions look good, you wonder if they could be improved upon. You aren't sure how to improve them, so you decide to ask Agent Builder what it thinks. To do so, select the **Describe** tab. In the **Describe** tab, enter a prompt that asks Agent Builder what other instructions it would recommend that could improve this ag

    ```
    What additional instructions would improve this agent’s ability to support executive decision-making and enterprise rollout planning?
    ```

7. Review Agent Builder’s recommendations.

8. If satisfied, enter:

    ```
    Add these recommendations to the agent instructions.
    ```

9. Once Agent Builder responds that it updated the instructions, select the **Configure** tab and scroll through the Instructions. Note the new items that Agent Builder added.

1. Now that you’re satisfied with the instructions, you’re ready to configure the agent’s knowledge sources and suggested prompts. On the **Configure** tab, scroll down to the **Knowledge** section. You should assign any relevant data sources, such as SharePoint sites, documents, or non-Microsoft integrations, that your agent should reference.

    > **Note:** If you don't add any public websites or work data to your agent, it might still be able to respond to your requests, but only using general capabilities of the underlying large language model (LLM), such as answering common knowledge questions, basic reasoning, or generating generalized text. As such, it's recommended that you ground your agents in specific work data or public websites; otherwise, the agent's responses might lack the context or relevance needed for business-specific tasks.

6. In the **Knowledge** section, add relevant Project Nexus documents from OneDrive (Adoption Report, Risk Log, Executive Notes, Change Plan, etc.).

7. If suggested prompts are automatically generated based on your agent description, review and use them as needed; otherwise, manually add the following suggested prompts in the **Suggested prompts** section.

    | **Title**                        | **Message**                                                                |
    | -------------------------------- | -------------------------------------------------------------------------- |
    | Executive Rollout Recommendation | Provide a go or no-go recommendation for Project Nexus enterprise rollout. **(1)** |
    | Adoption Summary                 | Summarize current adoption performance across all departments. **(2)**             |
    | Risk Overview                    | List open risks that could impact enterprise expansion. **(3)**                   |
    | Mitigation Plan                  | Generate a mitigation plan for low HR adoption and change resistance. **(4)**     |

1. In the **Agent preview** pane on the right side, test your agent by selecting one of the suggested prompts or entering a custom prompt such as `Provide a go or no-go recommendation for Project Nexus enterprise rollout.` 

1. Review the response and verify that it references information from your added Project Nexus knowledge documents (such as adoption metrics, risks, or financial details) rather than providing only generic guidance.

1. You can test your agent as long as you want and refine your configuration if it isn't working or responding as you intended. You can do so by either manually updating the **Instructions**, or by updating the **Description**, in which case Agent Builder automatically updates the **Instructions** based on the changes you made to the **Description**.

1. Once you feel the agent is configured properly and you're satisfied with the results of the suggested prompts, select the **Create** button at the top of the page.  

8. Select **Create** once configuration is complete.

1. Open your newly created agent.

2. Test it using the following one-line prompts:

    ```
    Provide an executive summary of Project Nexus readiness for enterprise rollout.
    ```

    ```
    Outline a phased expansion strategy based on current adoption and risks.
    ```

3. Verify that:

    * The agent references your uploaded Project Nexus documents
    * Responses are structured and decision-focused
    * Outputs are relevant to executive leadership

1. If responses are too generic, refine the **Instructions** or **Description**, then test again.

1. When you're done using the agent, select **All agents** in the navigation pane. In your **Agent Store** window that appears, note how your agent is displayed in the **Your agents** section. You can access this agent from the Agent Store, or you can select the pin icon that appears next to the agent in the navigation pane if you want the agent to always display under the list of agents in the pane. 

# Outcome

You have successfully:

* Designed a fully custom Copilot agent
* Grounded it in real business documents
* Configured knowledge sources
* Validated decision-focused outputs

---

### 🎉 Exercise Completed Successfully
