
### Function Calling

**Function calling** is a core capability that allows Large Language Models (LLMs) to **interact with external tools, data, and other systems**. Its main purpose is to **overcome the limitations of an LLM's context window**, which, when filled, prevents the LLM from understanding the ongoing conversation. By using function calling, the LLM gains the ability to "talk to other things".

Here's how function calling significantly extends an LLM's capabilities:

*   **Extending Modality**: While some LLMs are inherently multi-modal, meaning they can process text, pictures, audio, and video, an LLM does **not need to be natively multi-modal to handle these data types**. It can achieve this through function calling. For example, Gemini models use function calling to **generate videos** directly within their app by performing function calling to Vo. Function calling also enables **audio input and output**, allowing users to speak to ChatGPT and have it respond audibly. When asking for news about Apple, function calling is performed to a text-to-speech model directly from OpenAI.
*   **Web Browsing and Information Retrieval**: LLMs can **browse the internet via function calling** by connecting to a browser through an API. For instance, when asked "What is the Bitcoin price today?", the LLM searches the web, querying sites like Coin Market Cap, TradingView, and Crypto.com via function calling to provide an answer.
*   **Tool Integration for Calculations**: LLMs are not inherently strong at mathematical computations. However, through function calling, they can **utilize external tools** such as a calculator, a Python interpreter, or terminals to perform complex calculations. An example demonstrates ChatGPT creating Python code to generate a pie chart from financial data, showcasing this capability. These are referred to as "software 1.0 tools".
*   **Retrieval Augmented Generation (RAG) Technology**: This is highlighted as **one of the most important applications of function calling**. LLMs can perform **function calling to a file system with embeddings**, which is essentially a vector database. This allows the LLM to **insert new data and browse existing data** that it was not originally trained on. For instance, a user can upload company-specific files, and then ChatGPT can query content within those files (e.g., "how many hours a day works the company I with Ani"), demonstrating how the LLM searches its "vector database" for specific information. A significant amount of work in building RAG applications is done via function calling. The simple picture analogy shows the LLM (brain) searching a database after documents are fed in.
*   **Image Generation**: LLMs can **generate pictures** by performing function calling to a diffusion model (or an autoregressive model). An example shows ChatGPT creating an image related to RAG technology by calling an image generation model.
*   **Inter-LLM Communication (Agents)**: LLMs can **communicate with other LLMs (referred to as agents)** via APIs.

In essence, function calling transforms an LLM into an **orchestrator**, capable of connecting to and leveraging various external services and tools to expand its functionalities far beyond its initial training data.

### LLM as an Operating System Analogy

![LLM OS]Images/LLMOS.png

Andrew Karpathy proposes a compelling analogy where an **LLM is viewed as our new operating system**, much like a traditional computer. This analogy provides a helpful framework for understanding how LLMs can integrate and manage diverse functionalities:

*   **LLM as the Computer**: The **LLM itself is likened to the computer**.
*   **Context Window as RAM**: The **context window of the LLM is analogous to the RAM** (Random Access Memory) in a computer. Just as RAM holds data for immediate processing, the context window holds the current conversational context.
*   **Function Calling as Communication Mechanism**: The LLM uses **function calling to "talk to other things,"** acting as the fundamental mechanism for interacting with external components. This is similar to how an operating system manages communication between different hardware and software components.
*   **File System with Embeddings (Vector Database) as Disk**: A **file system containing embeddings**, often implemented as a vector database (which underpins RAG technology), is compared to the **computer's disk**. This is where new or external data can be stored and retrieved for long-term access, much like how a disk provides persistent storage.
*   **Python Interpreter/Calculator as Software 1.0 Tools**: Tools like a Python interpreter or a calculator are described as "**software 1.0 tools**". These are akin to traditional software applications that can be installed and run on a computer.
*   **Audio and Video as Peripheral Devices**: **Audio and video capabilities** are likened to **peripheral devices**, which are external components (like microphones or webcams) connected to a computer to extend its input and output functionalities.
*   **Browser as Ethernet**: A **browser is compared to Ethernet**, representing the network interface that allows the computer (LLM) to connect to the internet.
*   **Communication with Other LLMs as Agents**: The ability of LLMs to communicate with other LLMs is referred to as **agents**. This implies autonomous entities that can perform tasks, similar to how different programs or services might interact within an operating system environment.

