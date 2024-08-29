# NLX-Captcha
Captcha to identify "iPad kids". Useful for blocking 8 year olds from accessing your content.

(THIS COSTS MONEY! USES OPENAI API)
Uses GPT-4. One request per captcha completion.

# Installation
```
pip install nlxcaptcha
```

# Usage
```
import nlxcaptcha

result, certainty = nlxcaptcha.verify(difficulty=5, openaiapikey="your-openai-api-key")
print(f"Result: {result}, Certainty: {certainty}")
```

If result = 1 then this is an iPad kid.
Otherwise it's not.

Certainty is a string structured as "99%". How confident the AI is with it's answer.
