## Demo

1. Search something
2. Search on an embedding (character)
3. Search
4. Create

```bash
http http://localhost:8080/create?id=1&content=Hello%20Riviera%20Dev

http http://localhost:8080/search-full-text?term=Riviera
```

## Code

```java
@VectorField(name = "embedding",
dimension = EmbeddingModelBridge.DIMENSION,
vectorSimilarity = VectorSimilarity.COSINE,
valueBridge = @ValueBridgeRef(type = EmbeddingModelBridge.class))
```

* Search "greeting" (knn and )
* Search "magic"
* Add Riviera
* Add I love coding java 
