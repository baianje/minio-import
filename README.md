

## Download from NPM

```sh
npm install --save minio-import
```



## Using with TypeScript

```sh
npm install --save-dev @types/minio
```

## Initialize MinIO Client

You need five items in order to connect to MinIO object storage server.


| Params     | Description |
| :------- | :------------ |
| endPoint	 | URL to object storage service. |
|port| TCP/IP port number. This input is optional. Default value set to ``80`` for HTTP and ``443`` for HTTPs.|
| accessKey | Access key is like user ID that uniquely identifies your account.   |
| secretKey	| Secret key is the password to your account.    |
|useSSL |Set this value to 'true' to enable secure (HTTPS) access |


```js
import Minio from 'minio-import'

var minioClient = new Minio.Client({
    endPoint: 'play.min.io',
    port: 9000,
    useSSL: true,
    accessKey: 'Q3AM3UQ867SPQQA43P2F',
    secretKey: 'zuf+tfteSlswRu7BJ86wekitnifILbZam1KYY3TG'
});
```

