Lab Assignment 3.0
Matthew McCarthy
CS 166 / Fall 2022



The changes that I made to the CatCoin_Stock.html file include Subresource Integrity. Subresource Integrity uses CDNs to host to improve site
performance and conserve bandwidth. It allows you to mitigate some risks of attacks.

To mitigate the XSS attack I changed the CatCoin_Stock.html file. To start I had to take the link "https://jreddy1.w3.uvm.edu/getStock.js" and
paste it into a SRI Hash Generator using srihash.org. The SRI Hash Generator gave me these lines to include in my <script>

integrity="sha384-eLjZLjnEqrqfoIzgU/ObMimoH+M3VIrXBaNuJyCDBRARMwzvENHbNIOs8PgnaJUT"
crossorigin="anonymous"

When adding these lines to the code, the XSS attack is mitigated and does not pop up when you refresh the website anymore.