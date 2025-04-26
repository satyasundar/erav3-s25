# MCP Project

This project demonstrates the use of the Model Context Protocol (MCP) to create a math agent capable of solving problems iteratively using various tools. The project includes tools for mathematical operations, drawing, and email sending, among others.

## Project Structure

- **example2.py**: Defines the MCP server and tools for mathematical operations, drawing, and email sending.
- **talk2mcp-2.py**: Implements the client-side logic for interacting with the MCP server, including tool usage and iterative problem-solving.
- **pyproject.toml**: Configuration file for the project.
- **uv.lock**: Lock file for dependencies.

## Key Features

1. **Mathematical Tools**:

   - Addition, subtraction, multiplication, division, power, square root, cube root, factorial, logarithm, and trigonometric functions.
   - Special tools like `strings_to_chars_to_int` and `int_list_to_exponential_sum`.

2. **Drawing Tools**:

   - Draw rectangles and add text in Microsoft Paint.
   - Open and interact with Sketch.io for drawing and text addition.

3. **Email Sending**:

   - Send emails using the Gmail API with OAuth2 authentication.

4. **Iterative Problem Solving**:
   - The client iteratively solves problems by interacting with the MCP server and tools.

## Setup Instructions

1. Clone the repository.
2. Install required dependencies
3. Create a `.env` file and add your Gemini API key:
   ```
   GEMINI_API_KEY=your_api_key_here
   ```
4. For Gmail API, set up credentials and save them as `credentials.json` in the project root.
5. Run the MCP server:
   ```
   python example2.py
   ```
6. Run the client:
   ```
   python talk2mcp-2.py
   ```

## Usage

- The client interacts with the server to solve mathematical problems, draw shapes, and send emails.
- Modify the query in `talk2mcp-2.py` to test different scenarios.

## Dependencies

- Python 3.8+
- MCP library
- Google Generative AI library
- Gmail API client
- PyAutoGUI
- Pillow

## License

This project is licensed under the MIT License.
