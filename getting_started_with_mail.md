### Getting Started with Mail

On Dimension you have an email address of `yourusername@dimension.sh`. This can be accessed in one of the following ways:

* Via an email client on `dimension.sh`
* Via an IMAP client (like Outlook, or Thunderbird)
* Forwarded to another email address.

#### Accessing via Dimension

We have two email clients installed on Dimension, which are configured by default to access your email account:

* `mutt`
* `alpine`

Which you use is a matter of personal preference, `alpine` has a gentler learning curve, but `mutt` is a fully-featured and configurable client. Many guides are available online on how to use both of these clients.

#### Accessing via IMAP

Accessing your Dimension mail from a full email client is quite easy. All the details that you need to connect to the mail server are available on the [[Accessing your email via IMAP]]. Configuration of the client varies from client to client, so please search for a guide for your client. If you have any issues, then contact the admins at [root@dimension.sh](mailto:root@dimension.sh).

#### Forward to another address

To forward your Dimension email to another address, all you need to do is created a file named `.forward` in your home directory with the email address you want the mails redirected to. 

If wanted to have all your emails forwarded to `myawesomeemail@gmail.com` you can run the following command:

```
# echo "myawesomeemail@gmail.com" > ~/.forward
```

Note: some email servers don't take kindly to this type of forwarding and may mark the mail as spam. 


#### Techie Stuff

For the techies, here is the configuration we use:

* Postfix, with DKIM outbound.
* TLS, SASL authenticated submission port.
* Dovecot for SASL and IMAP, TLS only.
* Maildir layout.
* No Procmail delivery - but may do it if people want it.