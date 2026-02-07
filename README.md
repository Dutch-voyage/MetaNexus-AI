# MetaNexus-AI

## run demos
### Install Node.js 
visit https://nodejs.org/zh-cn/download

### Install dependencies

```
npm install lucide-react
```

### Run 

```
npm run dev
```

### swith to your API

See line 115-130 in demos/autodoc-demo/src/App.jsx

``` js
    const response = await fetch(
      "https://open.bigmodel.cn/api/paas/v4/chat/completions",
      {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
          'Authorization': `Bearer ${apiKey}`,
        },
        body: JSON.stringify({
          model: "glm-4.7",
          messages: messages,
          temperature: 1.0,
          stream: false
        }),
      }
    );

```

Swith to your own API format (url/headers/apiKey e.t.c.). 

