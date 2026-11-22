# Image témoin du profil docker (build sur prd-build-runner-01) : page statique
# servie par busybox httpd, ~4 Mo. Non déployée (deploy/ utilise http-echo).
FROM busybox:1.37
COPY index.html /www/index.html
USER 65532:65532
EXPOSE 8080
CMD ["httpd", "-f", "-p", "8080", "-h", "/www"]
