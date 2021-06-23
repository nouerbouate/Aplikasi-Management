#  APLIKASI INVOICE MANAGEMENT #

Aplikasi ini dipakai untuk mengelola invoice dan menyambungkan dengan berbagai metode pembayaran.
Diantara metode pembayaran yang akan disupport

* Virtual Account Bank
    
    * Bank BNI
    * Bank CIMB 
    * BANK BSI
    
* e-Wallet
    
    * OVO
    * Gopay
    
* QR Pyment
    
    * QRIS
    

# CARA SETUP DATABASE #

* Jalankan Postgres di docker

---
* Create Docker Container lewat terminal
  
    ``` 
    docker container create \
    --name invoice-db \
    -e POSTGRES_DB=invoicedb \
    -e POSTGRES_USER=invoice \
    -e POSTGRES_PASSWORD=oHJyiVYkOAXM5Q2YQPqp \
    -e PGDATA=/var/lib/postgresql/data/pgdata \
    -p 5432:5432 \
    postgres:13
    ```
  
* Run Container
  
  * Docker Container start (nama containernya)
  
---
* Langsung create container dan auto remove jika di stop

``` 
    docker run --rm \
    --name invoice-db \
    -e POSTGRES_DB=invoicedb \
    -e POSTGRES_USER=invoice \
    -e POSTGRES_PASSWORD=oHJyiVYkOAXM5Q2YQPqp \
    -e PGDATA=/var/lib/postgresql/data/pgdata \
    -p 5432:5432 \
    postgres:13
```
    





