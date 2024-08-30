# NLX-Captcha
Captcha to identify "iPad kids". Useful for blocking 8 year olds from accessing your content.

(THIS COSTS MONEY! USES OPENAI API)
Uses gpt-4 or gpt-3.5-turbo. One request per captcha completion.

# Installation
```
pip install nlxcaptcha
```

# Usage
```
import nlxcaptcha

result = nlxcaptcha.verify(difficulty=1.5, openaiapikey="your-openai-api-key", model="gpt-3.5-turbo") # You can change model to "gpt-4" for more accurate (but more expensive) results.
print(f"Result: {result}")
```

The result is a string, either 1 or 0. If the result is 1, then ChatGPT thinks it's an iPad Kid. If the result is 0, then ChatGPT doesn't think it's an iPad Kid.

# Pricing
One NLXCaptcha request:

GPT-4: ~$0.01

GPT-3.5-TURBO: ~$0.001
