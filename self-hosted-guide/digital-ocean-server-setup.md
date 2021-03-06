# Digital Ocean Server Setup

## Creating a new Droplet

Login to your Digital Ocean account and click create then select Droplet. 

![](../.gitbook/assets/image%20%2818%29.png)

Choose an Image. BTCP is currently optimized to run on Ubuntu with 2 GB of memory for $10/month. 

![](../.gitbook/assets/image%20%2812%29.png)

  
Choose the location closest to where most of your clients are from.

![](../.gitbook/assets/image%20%2821%29.png)

  
Select IPv6 and Monitoring. 

![](../.gitbook/assets/image%20%2822%29.png)

## Add your SSH Key to allow remote login to this server. 

If you don't have a public SSH key on your computer you can generate one using the following tools: 

{% tabs %}
{% tab title="Linux" %}
```text
ssh-keygen
```
{% endtab %}

{% tab title="Windows" %}
Download Git  
  
 "**Git bash** " is a msys shell included in "Git for Windows" software. It will allow you to generate pairs of public and private keys to be used to login to your Droplet. 

Download GIT from here:

{% embed data="{\"url\":\"https://git-scm.com/downloads\",\"type\":\"link\",\"title\":\"Git - Downloads\",\"icon\":{\"type\":\"icon\",\"url\":\"https://git-scm.com/favicon.ico\",\"aspectRatio\":0}}" %}

## RUNNING PUTTYGEN

 Go to Windows **Start menu**  type Git Bash

![](../.gitbook/assets/image%20%2823%29.png)

  
Run the following command and follow the prompts

```text
 ssh-keygen
```

![](../.gitbook/assets/image%20%282%29.png)

Enter a name for your keys, then enter a passphrase, they will be saved on your user folder  ~/  by default. Its a good practice to move them to  ~/.ssh

Copy the Public key \(The file that ends in .pub\) will be required for the next step. 

{% hint style="info" %}
Public key is the shorter one. Starts with ssh-rsa
{% endhint %}
{% endtab %}

{% tab title="Max" %}

{% endtab %}
{% endtabs %}

## Add your SSH Key

Add your SSH key from the previous step. 

![](../.gitbook/assets/addkey.gif)

## Finalize

Enter a name and create click create

![](../.gitbook/assets/image%20%2816%29.png)

{% hint style="success" %}
You have now set up your own droplet, now we need to connect to the server and set up BitCore.
{% endhint %}



