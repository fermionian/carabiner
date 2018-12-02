### How to start a jupyter notebook from a remote server  ###


From: [Remote Access to IPython Notebooks via SSH](https://coderwall.com/p/ohk6cg/remote-access-to-ipython-notebooks-via-ssh)

1) Start jupyter on the remote machine 

        remote_user@remote_host$ jupyter notebook --no-browser --port=8889

2) Start an SSH tunnel on local machine, and forwarding remote port 8889 to local port 8888

        local_user@local_host$ ssh -N -f -L localhost:8888:localhost:8889 remote_user@remote_host

3) * If you have set up password config, just type the following in your browser on your local machine

            localhost:8888

   * If not, you need to type in the url with token info, copy the link from 1) but change the port to 8888

