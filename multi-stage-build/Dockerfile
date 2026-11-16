# stage 1: builder

from ubuntu:24.04 as builder

workdir /app

copy index.html .

#stage-2:final image

from nginx:alpine

copy --from=builder /app/index.html /usr/share/nginx/html/index.html

expose 80

cmd [ "nginx", "-g", "daemon off;" ]

