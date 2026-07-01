# portfolio1

Open `index.html` in your browser to run the portfolio locally.

If you want to serve it from a local web server, run:

```bash
cd /workspaces/portfolio1
python3 -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## Docker and Render

This repository includes a `Dockerfile` and `render.yaml` so it can be deployed on Render using Docker.

To build and test the Docker image locally:

```bash
cd /workspaces/portfolio1
docker build -t portfolio1 .
docker run -p 8000:8000 portfolio1
```

Then open `http://localhost:8000`.

To deploy on Render, connect the repository and use the `render.yaml` service definition. It will build the Docker image from `Dockerfile` and serve the static portfolio.
