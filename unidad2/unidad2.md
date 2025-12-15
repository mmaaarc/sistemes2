## Pràctica Windows 
## Pràctica Windows 
En primer lloc aquest és l'esquema de les IPs i la configuració dels equips entre client, servidor, on el client rebra una IP en VPN desde el servidor Windows Active Directory.

<img width="439" height="289" alt="image" src="https://github.com/user-attachments/assets/d28d97ec-25b5-40a8-a345-1e7c2bc390a7" />

Per tant el primer que fare és configurar els moduls al servidor active directory necessaris.

<img width="501" height="461" alt="image" src="https://github.com/user-attachments/assets/e43631b9-0801-46b9-a505-cc4e96faf113" />

<img width="501" height="461" alt="image" src="https://github.com/user-attachments/assets/24bccc1e-bd17-4584-8f92-6a4e2924128f" />

<img width="612" height="345" alt="image" src="https://github.com/user-attachments/assets/ee919563-687e-441c-9ded-1bbfb2f63493" />

I aquesta és la configuració a la primera interfícies de xarxa interna del servidor.

<img width="392" height="420" alt="image" src="https://github.com/user-attachments/assets/b88239e1-4444-4876-a047-f2595c3f0684" />

I aquesta és la segona interfície del servidor de xarxa interna.

<img width="455" height="542" alt="image" src="https://github.com/user-attachments/assets/1e854c9c-a76e-4d80-adbd-4539c4b23f6a" />

Seguidament passare a configurar la VPN al servidor per tant em direccionare a Enrutamineto y acceso remoto i l'activare.

<img width="605" height="395" alt="image" src="https://github.com/user-attachments/assets/b310946d-cb4e-4e93-aa7f-93b36ae105bd" />

Permeto l'accés remot a dispositius de la xerxa privada.

<img width="510" height="479" alt="image" src="https://github.com/user-attachments/assets/8236a6ae-b949-4257-ae3f-f64d067e05ee" />

Configuro per accés VPN.

<img width="510" height="479" alt="image" src="https://github.com/user-attachments/assets/3304ff4c-9eea-42cf-bc97-e00b39be4959" />

Selecciono la interfaç 10.10.1.2 que es a la que es connectara el client.

<img width="507" height="480" alt="image" src="https://github.com/user-attachments/assets/67edd805-8325-4cce-af59-d69a5e390cd2" />

I configuro en un rang de IPs.

<img width="523" height="486" alt="image" src="https://github.com/user-attachments/assets/167ef2d6-cad3-47fa-bc0d-06abe8f3fd87" />

Com diu la imatge de la 172.16.0.0 a la 172.16.0.10.

<img width="515" height="480" alt="image" src="https://github.com/user-attachments/assets/5be7c2c4-ece5-49e7-9c18-5938c2b33d8d" />

<img width="516" height="477" alt="image" src="https://github.com/user-attachments/assets/3902dc2f-b4a9-4d77-8b3a-344e1b834d21" />

<img width="469" height="92" alt="image" src="https://github.com/user-attachments/assets/9cacadc4-e54e-4941-833b-218a0aace41e" />

Ara el servidor ja consta de accés remot per als possibles clients.

<img width="580" height="333" alt="image" src="https://github.com/user-attachments/assets/a0e861a4-9680-4c24-90ad-1572404532d0" />

## USUARI 
Seguidament creo un usuari per fer les proves de connexió al servidor desde un altre dispositiu client.

<img width="557" height="517" alt="image" src="https://github.com/user-attachments/assets/60dcf9fc-f427-45a2-b3e7-98a2e0899d2f" />

Es important permetre l'accés a altres reds dins de la configuració del usuari.

<img width="449" height="200" alt="image" src="https://github.com/user-attachments/assets/2faa6997-6e4a-4dbc-b5b8-b3d7617018da" />

## CONNEXIÓ CLIENT

A continuació comprovo que tinc connexió entre màquina client i servidor.

<img width="344" height="484" alt="image" src="https://github.com/user-attachments/assets/d81f007c-f0d0-4358-bca8-eaa719111f31" />

Aquesta és la ip del client.

<img width="602" height="229" alt="image" src="https://github.com/user-attachments/assets/fc508ab7-393b-4a29-9089-917fdc8dd909" />

I li intento fer un ping al servidor que efectivament el resol.

<img width="603" height="295" alt="image" src="https://github.com/user-attachments/assets/fff4251b-5378-4e49-a325-647abc91ae5d" />

El mateix de servidor a client.

<img width="602" height="465" alt="image" src="https://github.com/user-attachments/assets/6cf7b773-c814-4225-b855-dfd397158acf" />

## CONNEXIÓ PER VPN AL CLIENT

Per connectarme per VPN al servidor entrare a reds i internet.

<img width="345" height="129" alt="image" src="https://github.com/user-attachments/assets/73f8aca1-c2fa-4f98-ace4-9a407b4f4848" />

Al centre de reds i recursos compartits.

<img width="592" height="92" alt="image" src="https://github.com/user-attachments/assets/8a7c8010-cd18-4027-8e0a-63f7f6b7d663" />

Configurare una nova connesxió.

<img width="503" height="261" alt="image" src="https://github.com/user-attachments/assets/b24f0b86-f4ec-446b-acad-2342ca517627" />

Selecciona la opció de connectarse a un lloc de treball. 

<img width="592" height="320" alt="image" src="https://github.com/user-attachments/assets/13afe9ce-5f9f-4425-92a3-f320f1a6a20e" />

I selecciono la opció de connectarme mitjançant una xarxa virtual privada (VPN).

<img width="613" height="435" alt="image" src="https://github.com/user-attachments/assets/4b16eacd-df5d-418f-ac87-a67b8510ae18" />

I poso la IP del servidor i qualsevol nom.

<img width="507" height="388" alt="image" src="https://github.com/user-attachments/assets/bb98a91d-58e3-4808-8e4c-78151330d797" />

Un cop fet això ja tindre feta la connexió per VPN de client a servidor.

<img width="494" height="318" alt="image" src="https://github.com/user-attachments/assets/0b0ec772-c2a9-445f-aeca-f9a4c11a8e6e" />

<img width="364" height="218" alt="image" src="https://github.com/user-attachments/assets/7e53111a-c286-48ed-b959-5b9ec335a631" />

<img width="599" height="327" alt="image" src="https://github.com/user-attachments/assets/3a33c070-0f82-4009-9847-15d5fd185503" />

