# OpenAI Image Generation with Node.js

This Node.js project uses the OpenAI API to generate an image based on a user-provided prompt. It connects to OpenAI’s DALL-E model to create an image and logs the URL of the generated image to the console.

## Prerequisites

- Node.js (v12 or higher)
- An OpenAI API Key
- A `.env` file in your project root to store environment variables

## Installation

1. **Clone the Repository**

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Install Dependencies**

   ```bash
   npm install
   ```

3. **Configure Environment Variables**

   - Create a `.env` file in the root directory of the project.
   - Add your OpenAI API key to the `.env` file:

     ```
     OPEN_AI_KEY=your_openai_api_key_here
     ```

## Usage

1. **Run the Project**

   To generate an image, simply run:

   ```bash
   node index.js
   ```

2. **Change the Prompt**

   The prompt for image generation is defined in the `generateImage` function. Modify the string argument within `generateImage()` to create images based on different prompts.

   ```javascript
   generateImage('Your desired prompt here')
   ```

3. **Output**

   Upon success, the URL of the generated image will be printed to the console. If an error occurs, it will be logged in the console.

## Project Structure

- **index.js**: Main script to generate images using the OpenAI API.
- **.env**: Environment file containing the API key (not included in the repository).

## Example

By default, the `index.js` file will generate an image based on the prompt: "YouTube video screen with a duck and a dinosaur." The generated image URL will be logged to the console.

## Dependencies

- `openai`: Official OpenAI Node.js SDK for interfacing with OpenAI’s APIs.
- `dotenv`: Loads environment variables from a `.env` file.

## License

This project is open-source and available under the [MIT License](LICENSE).
