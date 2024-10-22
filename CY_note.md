1. genrate concepts with LLMs
used prompt: weaver/specs/relations_default.json`
```
{
        "id": "TYPEOF",
        "tag": "has subtype",
        "description": {
            "text": "is a type of",
            "position": "second"
        },
        "prompt": "List {N} types of {topic}."
    },
    {
        "id": "PARTOF",
        "tag": "has part",
        "description": {
            "text": "is a part of",
            "position": "second"
        },
        "prompt": "List {N} parts or aspects of {topic}."
    },
```

2. genrate test input for concept
prompt: `weaver/specs/generators.json`
```
Write one comment on the topic '{topic}' relevant to '{seed}' in an online platform.
```


3. generte expected output values for test inputs
* use AdaTest, and manually decide the expected values.