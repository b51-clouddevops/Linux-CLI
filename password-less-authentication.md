# Linux Password Less Authentication:

### Procedure to connect to linux machine using SSH-KEYS (Procedure is based on xShell as SSH Client )

`Note :` Ensure you pay more attention while you do copy paste with keys

Video Ref `https://youtu.be/IdTUwLgUu5k`

1) Create the directory named batch49
```
 mkdir batch51
```

2) cd batch51 ( move to that folder )

3) Command to create a SSH Key Pair
``` 
ssh-keygen -f b51  ( -f is the file name to be generated)
```

4) Rename the b51 file to b51.pem ( Pem is the private key format file accepted by xSHELL )
```
mv b51 b51.pem
```

5) Open your xShell ---> Tools ---> USer Key manager ---> Import your b51.pem Key 
   On your AWS Cloud ---> EC2  --> KeyPairs ---> Import Your PublicKey b51.pub


6) Connect to linux machine

```
ssh centos@publicIPAddress
```
