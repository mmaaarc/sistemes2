## AUTOMATITZACIÓ FUNCIONAL
En primer lloc el que demana la pràctica és unir el client Ubbuntu Desktop al domini que ja tinc al Windows Server.
Per tant primer comprvo la communicació entre les dues màquines.
De client a Servidor.
<img width="596" height="188" alt="image" src="https://github.com/user-attachments/assets/c6289b4b-1c9a-4114-bddf-15ab3a355424" />

De servidor a client.
<img width="515" height="237" alt="image" src="https://github.com/user-attachments/assets/f0cd35fb-9cd9-4c2c-9a48-bb37454ab715" />

Per tant ara cercare desde el client UBuntu amb la comanda realm discover el domini del servidor Windows.

<img width="451" height="261" alt="image" src="https://github.com/user-attachments/assets/3a4291aa-2827-4ab8-9cbc-aaf5d6213af9" />

Per tant el troba i ara m'unire amb la comanda realm joun el domini i l'usuari al qual em connecto Administrador.

<img width="606" height="88" alt="image" src="https://github.com/user-attachments/assets/5420e617-1041-479d-a99c-851e7626599c" />

I puc comprovar que m'he unit al domini amb la comanda realm list.

<img width="383" height="299" alt="image" src="https://github.com/user-attachments/assets/66c2d775-f99d-490f-8e3b-69e05d45b48e" />

## INSTAL·LACIÓ IIS WINDOWS SERVER

Per instal·lar el servidor web IIS em dirigeixo a Administració del servidor i afegir rols i procedire a afegir el rol de Servidor Web IIS.

<img width="786" height="557" alt="image" src="https://github.com/user-attachments/assets/ec360950-705b-42cf-a654-9d50c6b539c6" />

I el comença a instal·lar.

<img width="781" height="555" alt="image" src="https://github.com/user-attachments/assets/7411dfa0-3d7e-4a78-bc0c-5986021ed1a4" />

Un cop instal·lat posare al navegador http://localhost per comprovar el correcte funcionament del servidor web.

<img width="762" height="509" alt="image" src="https://github.com/user-attachments/assets/238bea12-bb61-47f5-80ed-f9cd32226423" />

També he fet la comprovació desde el client Ubuntu Desktop connectat al domini.

<img width="1025" height="551" alt="image" src="https://github.com/user-attachments/assets/ded8a3b2-f3d6-4a7b-8a24-6158e931948b" />

Ara he creat un index.html de prova dins de la ruta /inetpub/wwwroot on es guarden els arxius del IIS.

<img width="320" height="224" alt="image" src="https://github.com/user-attachments/assets/ed2d48b5-e795-4e90-a86c-05345f546be1" />

<img width="439" height="156" alt="image" src="https://github.com/user-attachments/assets/78f8b1b3-6bf7-4073-9376-f9c48e8d70fb" />

## CERTIFICATS I WEB AMB HTTPS


<img width="560" height="149" alt="image" src="https://github.com/user-attachments/assets/58fd7b6a-74b7-41b9-a936-940223e50e05" />

<img width="403" height="559" alt="image" src="https://github.com/user-attachments/assets/d86ed353-2e5e-4329-9691-467be703e896" />

<img width="403" height="563" alt="image" src="https://github.com/user-attachments/assets/1c58f678-fc0f-4f48-8445-4f0ea4e4a0a4" />

<img width="401" height="560" alt="image" src="https://github.com/user-attachments/assets/977f47ca-4340-4d93-b8e4-67f9918e6782" />

<img width="552" height="406" alt="image" src="https://github.com/user-attachments/assets/f9ee8b63-93c6-45cc-b31a-79c9f6a0b255" />

<img width="419" height="145" alt="image" src="https://github.com/user-attachments/assets/a7ce2885-9add-4f14-b0d9-00518d851b8d" />

<img width="375" height="86" alt="image" src="https://github.com/user-attachments/assets/4b4ee1de-3f34-463c-8fe4-676aa23901d7" />


<img width="395" height="251" alt="image" src="https://github.com/user-attachments/assets/e93ba278-4628-4335-b19b-b752073b5c92" />

<img width="561" height="72" alt="image" src="https://github.com/user-attachments/assets/c94b1f10-a326-4220-8d40-e433473f76cb" />


Per poder passar la web a https, és necessari un certificat web, en el meu cas he creat jo mateix el certificat.

Per tant m'he dirigit a la'apartat Administrador de IIS dins del servidor, he seleccionat la màquina i he fet clic a certificados de servidor.

<img width="910" height="559" alt="image" src="https://github.com/user-attachments/assets/a2fc73d1-d808-4580-a562-fa3dfbac4816" />

Hi he creat una solicitud de certificat nou.

<img width="221" height="259" alt="image" src="https://github.com/user-attachments/assets/e098ad67-6072-4909-b33e-6215bfdeb813" />

<img width="670" height="512" alt="image" src="https://github.com/user-attachments/assets/e6a85c28-13bf-42ec-8255-4c36a7ab5b62" />


Aquest és el certificat.

<img width="600" height="181" alt="image" src="https://github.com/user-attachments/assets/96ae325d-b76d-4186-ad0b-1a3efe4bac80" />



Ara importare el certificat.

<img width="233" height="287" alt="image" src="https://github.com/user-attachments/assets/88c7730a-8742-408d-b802-1171077f811a" />

Importare el certificat creat.

<img width="525" height="414" alt="image" src="https://github.com/user-attachments/assets/a8af8590-d214-4591-bf41-1bd3c33f7198" />


Ara em dirigire a sitios i enlaces.

<img width="1002" height="186" alt="image" src="https://github.com/user-attachments/assets/d043019a-0e97-4051-ba55-e3796185988a" />

Creare un nou enllaç.

<img width="533" height="418" alt="image" src="https://github.com/user-attachments/assets/8e284c6d-014e-414c-b6dc-fa77a66b8c57" />

<img width="646" height="371" alt="image" src="https://github.com/user-attachments/assets/4c974222-b7ab-46b1-99e0-b7975d059c6a" />

I ara ja podre accedir per https al meu index.html del servidor.

<img width="600" height="181" alt="image" src="https://github.com/user-attachments/assets/a9d85a6b-57ec-42f2-ae76-7d9698f04be4" />

I efectivament ja tinc el meu inde.html funcional amb https i http.

<img width="694" height="186" alt="image" src="https://github.com/user-attachments/assets/01904ab1-2ea3-4198-9a64-17a424907db6" />








