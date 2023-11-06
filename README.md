# OpenAI Chatbot Integration with LINE Messaging API

This repository contains a Python-based FastAPI application that integrates OpenAI's ChatGPT with the LINE Messaging API.

## Overview

The application uses the OpenAI API to generate responses to user messages sent via LINE. The integration is done using FastAPI and the LINE Messaging API.

## Prerequisites

To run this application, you will need:

- Python 3.6 or later
- An OpenAI account with API key
- LINE Messaging API Channel with a Channel Secret and Channel Access Token

## Installation

1. Clone this repository:

```bash
git clone https://github.com/your-repository.git
```

2. Navigate to the project directory:

```bash
cd your-repository
```

3. Install the required packages:

```bash
pip install -r requirements.txt
```

## Configuration

Create a `.env` file in the project root directory with the following variables:

```env
OPENAI_API_KEY=your_openai_api_key
ChannelSecret=your_line_channel_secret
ChannelAccessToken=your_line_channel_access_token
```

Replace `your_openai_api_key`, `your_line_channel_secret`, and `your_line_channel_access_token` with your actual OpenAI API key, LINE Channel Secret, and LINE Channel Access Token respectively.

## Usage

Run the FastAPI application:

```bash
uvicorn main:app --reload
```

The application will start on `http://localhost:8000/`.

## API Endpoints

- POST `/callback`: Handles incoming requests from the LINE Messaging API.

## Deploy this on Web Platform

You can choose [Heroku](https://www.heroku.com/) or [Render](http://render.com/)

### Deploy this on Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

- Input `Channel Secret` and `Channel Access Token`.
- Input [OpenAI API Key](https://platform.openai.com/account/api-keys) in `OPENAI_API_KEY`.
- Remember your heroku, ID

### Deploy this on Render.com

[![Deploy to Render](http://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)

## License

This project is licensed under the Apache License, Version 2.0. For more information, see the [LICENSE](https://www.apache.org/licenses/LICENSE-2.0) file.
