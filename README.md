# Video Search
This is a small exploration of the capabilities of Aleph Alphas Luminous model. I tried to build a video search with text queries POC. 

The approach starts by taking frames from a video with a given frame rate. In a second step, the frames and the query get embedded with luminous tuned for semantic embeddings. Later, the cosine similarity between the query and every frame is calculated.

For the first video, I searched for "ball in the air" and the approach found the two moments where the woman is throwing the ball with the highest similarity.
For the second video I searched for different types of fruit. As can be seen down below, the prompt design is a big factor of finding the right frames. But it seems like the similarity between a frame with a watermelon is close to a wide range of queries, including queries like "no watermelon".

## Ball Throwing Video
https://user-images.githubusercontent.com/17069602/193403442-62db7dbc-f936-4717-9e3c-99ca4dce7dc7.mp4
### Query: ball in the air
- Cosine Similarity per Frame
![newplot](https://user-images.githubusercontent.com/17069602/193403438-f43e2367-a9c3-4bae-930e-cad7164de1a9.png)
- Frame with Highest Cosine Similarity
![image](https://user-images.githubusercontent.com/17069602/193403759-88a61951-cb6a-45c3-ae64-8735da79cc94.jpeg)


## Fruit Video

https://user-images.githubusercontent.com/17069602/193403528-999cf1f0-afaf-4dc3-808f-3f9978b200c7.mp4

### Query: pineapple
- Cosine Similarity per Frame
![newplot-5](https://user-images.githubusercontent.com/17069602/193404001-12a91b6c-be97-4b2d-825c-a6a5dd0d9860.png)

- Frame with Highest Cosine Similarity
![image](https://user-images.githubusercontent.com/17069602/193404007-4b36307f-3769-4912-935d-c8288ae5bb35.jpeg)

### Query: pineapple in the middle
- Cosine Similarity per Frame
![newplot-6](https://user-images.githubusercontent.com/17069602/193404028-854be470-0c77-450e-a1d7-aa6329c45a71.png)

- Frame with Highest Cosine Similarity
![image](https://user-images.githubusercontent.com/17069602/193404033-cfe86d40-75be-4344-9794-06eb380da391.jpeg)

### Query: kumquats
- Cosine Similarity per Frame
![newplot-3](https://user-images.githubusercontent.com/17069602/193403556-835c4e76-de28-44a4-9af3-5ea88d6db8a9.png)
- Frame with Highest Cosine Similarity
![Bildschirmfoto 2022-10-01 um 11 55 17](https://user-images.githubusercontent.com/17069602/193403836-c05b81cb-029c-4ca8-81d1-f06a15c93fbb.png)

### Query: kumquats and no watermelon
- Cosine Similarity per Frame
![newplot-4](https://user-images.githubusercontent.com/17069602/193403565-ee178355-b1f3-4eef-84c7-6a1e90b81334.png)
- Frame with Highest Cosine Similarity
![Bildschirmfoto 2022-10-01 um 11 55 54](https://user-images.githubusercontent.com/17069602/193403856-bef69081-91db-4de5-9296-17eb481434fc.png)
