# toon-llm

Token-Oriented Object Notation (TOON) is a compact, schema-driven
serialization format optimized for Large Language Models.

## Example

```python
import toon_llm as toon

schema = toon.Schema({
    "name": toon.Str(1),
    "age": toon.Int(2),
    "active": toon.Bool(3)
})

toon.dumps({"name":"Sai","age":25,"active":True}, schema)
# 1=Sai;2=25;3=1
