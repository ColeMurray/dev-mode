# Dev Mode

Dev Mode gives you the power to easily inspect designs and translate them into code—without changing the design file. This application bridges the gap between design and development by allowing you to inspect design files for layout, dimensions, and styles, then seamlessly convert these into production-ready code.

## Overview

The project is split into two main parts:

- **Frontend:** A Next.js application built with TypeScript that provides a rich, interactive interface for design inspection and code generation.
- **Backend:** A FastAPI service that handles API requests, design file processing, and code translation logic.

## Dev Mode Features

- **Design Inspection:** Easily inspect design files to extract element properties.
- **Automatic Code Translation:** Generate reusable code components directly from your design elements.
- **Real-time Preview:** Watch live previews and instantly see the impact of your design changes.
- **Seamless Integration:** Connect with popular design tools without altering the original design file.

## Technologies Used

### Frontend
- **Framework:** [Next.js](https://nextjs.org/)
- **Language:** TypeScript
- **Package Manager:** npm or Yarn

### Backend
- **Framework:** [FastAPI](https://fastapi.tiangolo.com/)
- **Language:** Python (3.8+ recommended)
- **Server:** Uvicorn

## Getting Started

Follow these steps to set up the project locally.

### Prerequisites

**For Frontend:**
- Node.js (v14 or newer)
- npm or Yarn

**For Backend:**
- Python 3.8 or newer
- pip (or Pipenv/virtualenv)

### Installation

#### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/dev-mode.git
cd dev-mode
```

#### 2. Setup Frontend

1. Navigate to the frontend directory:

   ```bash
   cd frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   # or if you're using Yarn
   yarn install
   ```

3. Run the development server:

   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. Open your browser and go to [http://localhost:3000](http://localhost:3000) to view the application.

#### 3. Setup Backend

1. Navigate to the backend directory:

   ```bash
   cd ../backend
   ```

2. Create and activate a virtual environment (optional but recommended):

   ```bash
   python3 -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Start the FastAPI server using Uvicorn:

   ```bash
   uvicorn main:app --reload
   ```

5. The backend is now running on [http://localhost:8000](http://localhost:8000).

### Project Structure

Below is a suggested project structure for clarity:

```
dev-mode/
├── frontend/
│   ├── pages/             # Next.js pages
│   ├── components/        # Reusable UI components
│   ├── public/            # Static assets
│   ├── styles/            # Global and component-specific styles
│   └── package.json
├── backend/
│   ├── app/
│   │   ├── main.py        # FastAPI app entry point
│   │   ├── routers/       # API route definitions
│   │   └── models/        # Data models and schemas
│   ├── requirements.txt   # Python dependencies
│   └── README.md          # Backend specific instructions (optional)
└── README.md              # This file
```

## Dev Mode Usage

- **Inspect Designs:** Upload or link a design file in supported formats.
- **Generate Code:** Choose design components to automatically generate corresponding code.
- **Real-time Integration:** Leverage the live update features for immediate feedback on your changes.

## Contributing to Dev Mode

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -am "Add new feature"
   ```
4. Push your branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.