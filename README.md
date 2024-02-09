version: '3'
services:
  guacamole:
    image: jwetzell/guacamole
    container_name: guacamole
    volumes:
      - ./postgres:/config
    ports:
      - "8290:8080"
volumes:
  postgres:
    driver: local
