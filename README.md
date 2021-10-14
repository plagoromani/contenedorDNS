
version: '2'  //tipo de versión

services:       //declaramos los servicios
  bind9:        //nombre del docker
    image: internetsystemsconsortium/bind9:9.16     //imagen que empleamos
    ports:      //puertos que empleamos
    - 53:53
    volumes:    //creación de volumenes
      - configpablo1:/etc/bind          //carpeta del volumen
      - configpablo2:/var/cache/bind
      - configpablo3:/var/lib/bind
      - configpablo4:/var/log
volumes:        //Declaramos volumen
  configpablo1:         //nombre del volumen
  configpablo2:
  configpablo3:
  configpablo4: