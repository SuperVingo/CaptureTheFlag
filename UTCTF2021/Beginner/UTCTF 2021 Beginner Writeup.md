Beginner
======================
Magic Bytes
----------------------
![Q](https://user-images.githubusercontent.com/20963122/111428954-97879f00-873b-11eb-88ec-fd4025ed07a1.PNG)
download out.txt file.
![notepad](https://user-images.githubusercontent.com/20963122/111428960-99e9f900-873b-11eb-92d5-f63c08a23442.PNG)
it's not looks just text. open hxd.
![png](https://user-images.githubusercontent.com/20963122/111429076-cef64b80-873b-11eb-80d5-ed6cf52a5d76.PNG)
we can find PNG file header. so change file extension.![out](https://user-images.githubusercontent.com/20963122/111428956-99516280-873b-11eb-972a-a7d9a63bd6d8.png)
utflag{file_extensions_mean_nothing}

-------------------------------------
Run-ELF
------------------------
![Q](https://user-images.githubusercontent.com/20963122/111429585-82f7d680-873c-11eb-9323-f3cacb1fd1c2.PNG)
download it.
![A](https://user-images.githubusercontent.com/20963122/111429583-81c6a980-873c-11eb-9c5a-def980044fd3.PNG)
just execute binary in linux

utflag{run_run_binary_9312854}

--------------------------
HTML
----------------------------
![Q](https://user-images.githubusercontent.com/20963122/111430305-88a1ec00-873d-11eb-983c-80f8736e8e9b.PNG)
go into UTCTF website.
![A](https://user-images.githubusercontent.com/20963122/111430304-88095580-873d-11eb-8f7a-dd077cdf76d4.PNG)
use the developer mode in web browser (maybe f12) and you can find flag in the source code.

utflag{you_found_me_0123959}

------------------
Cipher Gauntlet
--------------------

![Q](https://user-images.githubusercontent.com/20963122/111430541-dc143a00-873d-11eb-8c4a-fb7227a1f8bd.PNG)
![H](https://user-images.githubusercontent.com/20963122/111430539-db7ba380-873d-11eb-8872-2a2b5a523467.PNG)
download it
![f](https://user-images.githubusercontent.com/20963122/111430538-dae30d00-873d-11eb-9498-a3337cf9e043.PNG)
in text file, you can find binary strings. transform character with ascii.  
![r](https://user-images.githubusercontent.com/20963122/111430542-dc143a00-873d-11eb-8e35-6d71e8cc6987.PNG)

> Uh-oh, looks like we have another block of text, with some sort of special encoding. Can you figure out what this encoding is? (hint: if you look carefully, you'll notice that there only characters present are A-Z, a-z, 0-9, and sometimes / and +. See if you can find an encoding that looks like this one.) 
> TmV3IGNoYWxsZW5nZSEgQ~~~~~~~~

last line looks base64 encoding. decode it.
>New challenge! Can you figure out what's going on here? It looks like the letters are shifted by some constant. (hint: you might want to start looking up Roman people). 
>myxqbkdevkdsyxc! iye rkfo psxscron dro loqsxxob mbizdyqbkzri mrkvvoxqo. robo sc k pvkq pyb kvv iyeb rkbn oppybdc: edpvkq{xyg_iyebo_zvkisxq_gsdr_mbizdy}. iye gsvv psxn drkd k vyd yp mbizdyqbkzri sc lesvnsxq ypp drsc cybd yp lkcsm uxygvonqo, kxn sd bokvvi sc xyd cy lkn kpdob kvv. ryzo iye oxtyion dro mrkvvoxqo!

new challenge. this is substitution cipher. we use [quipquip](https://quipqiup.com/) site. we already know [edpvkq = utflag]

![rr](https://user-images.githubusercontent.com/20963122/111430543-dcacd080-873d-11eb-93e4-d2895c11d51e.PNG)
utflag{now_youre_playing_with_crypto}

-----------------------
Sizzling Bacon
---------------------
![Q](https://user-images.githubusercontent.com/20963122/111436085-ed147980-8744-11eb-9ac6-9c3a5d083b22.PNG)
``` python
a = "sSsSSsSSssSSsSsSsSssSSSSSSSssS{SSSsSsSSSsSsSSSsSSsSSssssssSSSSSSSsSSSSSSSSsSSsssSSssSsSSSsSSsSSSSssssSSsssSSsSSsSSSs}"\
 .replace("{","").replace("}","").replace("s", "0").replace("S", "1") 
s = ''  
for i in range(0, int(len(a)/5)): 
	print(a[i * 5 : i * 5 + 5], int(a[i * 5 : i * 5 + 5], 2)) 
	s += chr(128 - int(a[i * 5 : i * 5 + 5], 2)) 
print(s)
```

---------
Stringy Things
----------
![Q](https://user-images.githubusercontent.com/20963122/111511366-01cb2e80-8792-11eb-9d8b-0eb768032d72.PNG)
download it
![r](https://user-images.githubusercontent.com/20963122/111511370-0263c500-8792-11eb-9630-d8d888d89e7f.PNG)
"there's a string in this binary somewhere..." so search "utflag" in hex

utflag{strings_is_op}

------
Various Vernacular
----------

![Q](https://user-images.githubusercontent.com/20963122/111511613-46ef6080-8792-11eb-8ff7-95e18e442808.PNG)
![H](https://user-images.githubusercontent.com/20963122/111511609-45be3380-8792-11eb-93c3-8d093cf9e5f9.PNG)
![H2](https://user-images.githubusercontent.com/20963122/111511611-4656ca00-8792-11eb-9bab-a9ccb38c1d3a.PNG)
![rr](https://user-images.githubusercontent.com/20963122/111511616-46ef6080-8792-11eb-99a8-d28d9b584bc8.PNG)
we use [quipquip](https://quipqiup.com/) site again.

utflag{nicht_English}
