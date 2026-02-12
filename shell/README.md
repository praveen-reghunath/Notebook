#### Copy command ( `cp` )

##### copy a single file

```sh
cp /home/source/demo.txt /home/destination/demo1.text
```

##### copy multiple files

```sh
cp /home/source cp-demo.txt cp-demo-1.txt cp-demo-9.txt /home/destination/
```

##### copy a folder 

```sh
cp -r /home/source/demo-folder/ /home/destination/
```

##### copy multiple folders into a destination folder

```sh
cp -r /home/source/demo-folder/ /home/another_folder/public_html/ /home/destination_folder/test
```

##### copy all the files, including hidden files

```sh
cp -R /home/source/.* /home/destination/all-files/
```
