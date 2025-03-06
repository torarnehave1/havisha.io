# Havisha.io

## Overview
Havisha.io is a structured process and workflow management application that allows users to create, view, edit, navigate, and manage workflows efficiently. It is built using **Node.js, JavaScript, MongoDB, and the Telegram API** to provide seamless interaction via a Telegram bot.

## Features
- **Process Creation:** Users can create structured workflows manually or using AI.
- **Process Navigation:** Move through workflow steps sequentially with options for branching and decision-making.
- **Process Editing:** Modify steps, reorder them, or update descriptions and prompts.
- **AI-Powered Workflow Generation:** Automatically generate steps using AI based on user-provided descriptions.
- **Process Categories & Answers:** Categorization of workflows and tracking user responses.
- **Telegram Bot Integration:** Interaction with workflows through a bot for easy access and real-time updates.
- **File Handling:** Upload and manage files within workflows.

## Technology Stack
- **Backend:** Node.js with Express
- **Database:** MongoDB with Mongoose ORM
- **Messaging & Interaction:** Telegram API using `node-telegram-bot-api`
- **AI Integration:** OpenAI API for AI-generated workflows

## Project Structure
```
📦 havisha.io
 ┣ 📂greenbot
 ┃ ┣ 📂edit
 ┃ ┃ ┣ 📜editHeader.js
 ┃ ┃ ┣ 📜editStep.js
 ┃ ┃ ┗ 📜reorderSteps.js
 ┃ ┣ 📂helpers
 ┃ ┃ ┣ 📜pdftomarkdown.js
 ┃ ┃ ┗ 📜processArchPublish.js
 ┃ ┣ 📂menus
 ┃ ┃ ┣ 📜createHeaderProcessMenu.js
 ┃ ┃ ┣ 📜editHeaderMenu.js
 ┃ ┃ ┣ 📜editMenu.js
 ┃ ┃ ┗ 📜viewProcessMenu.js
 ┃ ┣ 📂steps
 ┃ ┃ ┣ 📜callToActionProcess.js
 ┃ ┃ ┣ 📜choiceProcess.js
 ┃ ┃ ┣ 📜connectionProcess.js
 ┃ ┃ ┣ 📜connectProcess.js
 ┃ ┃ ┣ 📜fileProcess.js
 ┃ ┃ ┣ 📜index.js
 ┃ ┃ ┣ 📜infoProcess.js
 ┃ ┃ ┣ 📜soundProcess.js
 ┃ ┃ ┣ 📜textProcess.js
 ┃ ┃ ┗ 📜yesNoProcess.js
 ┃ ┣ 📜addStepService.js
 ┃ ┣ 📜answerService.js
 ┃ ┣ 📜createDescriptionAI.js
 ┃ ┣ 📜createProcessAI.js
 ┃ ┣ 📜deeplink.js
 ┃ ┣ 📜editProcessService.js
 ┃ ┣ 📜processInitializer.js
 ┃ ┣ 📜processNavigator.js
 ┃ ┗ 📜ViewProcessHeader.js
```

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/havisha.io.git
   ```
2. Navigate into the project directory:
   ```sh
   cd havisha.io
   ```
3. Install dependencies:
   ```sh
   npm install
   ```
4. Set up your `.env` file with required credentials:
   ```sh
   TELEGRAM_BOT_TOKEN=your-telegram-bot-token
   MONGO_URI=your-mongodb-connection-string
   OPENAI_API_KEY=your-openai-api-key
   ```
5. Start the application:
   ```sh
   npm start
   ```

## Usage
### Telegram Bot Commands
- `/start` - Begin interaction with the bot
- `/create` - Initiate a new process creation
- `/view` - View existing processes
- `/edit` - Modify an existing process
- `/restart` - Restart the bot

### Process Editing & AI Features
- Modify workflow steps using inline Telegram commands.
- Use AI to generate structured workflows automatically.
- Archive or delete processes as needed.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m 'Add feature'`
4. Push to the branch: `git push origin feature-name`
5. Open a Pull Request.

## License
This project is licensed under the MIT License. See `LICENSE` for more details.

## Contact
For issues and suggestions, reach out via GitHub Issues or contact the development team.

