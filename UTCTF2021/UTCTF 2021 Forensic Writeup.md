#Forensic
================
SHIFT
----------------------------
![Q](https://user-images.githubusercontent.com/20963122/111513537-422bac00-8794-11eb-9639-6b85ca5f4284.PNG)  
download it  
![SHIFT](https://user-images.githubusercontent.com/20963122/111513539-422bac00-8794-11eb-8bc5-e8af7080a134.png)  
I think the letters is tilted like italics. so use the photoshop distortion function.  
![a](https://user-images.githubusercontent.com/20963122/111513531-40fa7f00-8794-11eb-8f19-d8124d8ec479.PNG)  
utflag{not_when_i_shift_into_maximum_overdrive}  
  
-----------------------------
Doubly Deleted Data
------------------------------
![Q](https://user-images.githubusercontent.com/20963122/111514101-c3833e80-8794-11eb-8b65-df6e9c0c54a4.PNG)  
download it and open FTK Manager  
![r](https://user-images.githubusercontent.com/20963122/111514109-c4b46b80-8794-11eb-8aec-b924fc249594.PNG)  
search "utflag". fisrt result is not flag.  
![rr](https://user-images.githubusercontent.com/20963122/111514113-c4b46b80-8794-11eb-8e91-4d35674ad048.PNG)  
second result is flag.  
  
------------------------------
Sandwiched
------------------------------
![Q](https://user-images.githubusercontent.com/20963122/111514548-312f6a80-8795-11eb-947d-f8ed33f04887.PNG)  
![H](https://user-images.githubusercontent.com/20963122/111514562-3391c480-8795-11eb-830f-73c5ada2efbe.PNG)  
download it  
![binwalk](https://user-images.githubusercontent.com/20963122/111514554-32609780-8795-11eb-9a10-22593ec2917c.PNG)  
use binwalk. we can find JPEG File in offset 0x1E90 ~ 0x9387. extract it
```python
b = open("secret.pdf", "rb").read()[0x1e90:0x9387]
r = open("flag.jpg", "wb").write(b)
```  
![flag2](https://user-images.githubusercontent.com/20963122/111514559-32f92e00-8795-11eb-8fac-df2375e3b585.jpg)  
utflag{file_sandwich_artist}  

-------------------------
OSINT Part 1, 2
------------------------------
Part 1  
![Q](https://user-images.githubusercontent.com/20963122/111515141-ca5e8100-8795-11eb-952e-432a341dfb75.PNG)  
![H](https://user-images.githubusercontent.com/20963122/111515134-c92d5400-8795-11eb-886f-079bcdd0657c.PNG)  
![H2](https://user-images.githubusercontent.com/20963122/111515136-c92d5400-8795-11eb-80f9-bc29da8d2964.PNG)  
![H3](https://user-images.githubusercontent.com/20963122/111515138-c9c5ea80-8795-11eb-8980-e25ba9331eac.PNG)  
go to site.  
![p](https://user-images.githubusercontent.com/20963122/111515139-c9c5ea80-8795-11eb-84f1-468a9b411a10.PNG)  
we can find "consistently be found on social media". search on google   
![wade](https://user-images.githubusercontent.com/20963122/111515142-ca5e8100-8795-11eb-8686-c8cb31df152d.PNG)  
can find twitter account.  
![f](https://user-images.githubusercontent.com/20963122/111515103-c16daf80-8795-11eb-8a5c-210c26357caa.PNG)  
utflag{g0t_y0ur_b4dg3}  
  
Part 2  
![Q](https://user-images.githubusercontent.com/20963122/111515450-232e1980-8796-11eb-912e-5053b13ce02c.PNG)  
![H](https://user-images.githubusercontent.com/20963122/111515437-1f9a9280-8796-11eb-9737-9e943e0d3a6d.PNG)  
![H2](https://user-images.githubusercontent.com/20963122/111515439-1f9a9280-8796-11eb-9ac7-a55d44693d97.PNG)  
![g](https://user-images.githubusercontent.com/20963122/111515424-1c9fa200-8796-11eb-8757-53e70b979c3b.PNG)  
we can find a photo uploaded on google drive in twitter.  
![b](https://user-images.githubusercontent.com/20963122/111515419-1ad5de80-8796-11eb-9d9d-5031c748fb9f.PNG)  
google image search and find a blog.  
![bb](https://user-images.githubusercontent.com/20963122/111515422-1c070b80-8796-11eb-89b6-9e9c02ba62ea.PNG)  
utflag{r3v3rs3d_t0_0r1g1nal}  
