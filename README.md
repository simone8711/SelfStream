# Deploy SelfStream 🤌

All cloud deployments use a **pre-built Docker image** from DockerHub

Two image are now available:

`qwertyuiop8899/selfstream:warp`

`qwertyuiop8899/selfstream:latest`

---
## Hugging Face Spaces (Free) BEST OPTION

[📺 Video Guide](https://www.youtube.com/watch?v=Ti2BNDjm0ns)

1. Go to [huggingface.co/new-space](https://huggingface.co/new-space)
2. Choose **Docker** as SDK, **Blank** template
3. Under ***Create your Dockerfile:*** section click on ***create the Dockerfile***
4. Paste the ***Dockerfile.hf.warp*** and click **Commit new file to main**
5. When it's done, click on 3 dots on the right **Embed This Space** and use the **Direct URL** link
6. The Space runs on port `7860`

> AnimeUnity and Vixsrc working only with warp image

---


## Koyeb

1. Create an account on [Koyeb.com](https://www.koyeb.com/)
2. Click **"Create Service"** → select **Docker image**
3. Image: `docker.io/qwertyuiop8899/selfstream:warp`
4. Port: `8000`
5. Add env variable: `PORT` = `8000`
6. Click **Deploy**

---


## Render

1. Go to [Render.com](https://render.com/) → **New** → **Web Service**
2. Select **Deploy an existing image from a registry**
3. Image URL: `docker.io/qwertyuiop8899/selfstream:warp`
4. Select Free on **Instance Type**
5. Click **Deploy Web Service**
6. The addon will be available under **qwertyuiop8899 / selfstream latest** (purple link)
---



## VPS / Raspberry / NAS

no need for warp locally, but if it's not working replace latest with warp 
```bash
docker pull qwertyuiop8899/selfstream:latest
docker run -d -p 7000:7000 qwertyuiop8899/selfstream:latest
```


Addon available at `http://your-ip:7000/manifest.json`

---

