# Spring Boot demo

Requires to have a `java.security` with the following properties:

``` 
# register our Spiffe Provider
security.provider.14=io.spiffe.provider.SpiffeProvider

#
# Determines the default key and trust manager factory algorithms for
# the javax.net.ssl package.
#
ssl.KeyManagerFactory.algorithm=Spiffe
ssl.TrustManagerFactory.algorithm=Spiffe

# list of accepted SPIFFE IDs
ssl.spiffe.accept=spiffe://example.org/myservice
```