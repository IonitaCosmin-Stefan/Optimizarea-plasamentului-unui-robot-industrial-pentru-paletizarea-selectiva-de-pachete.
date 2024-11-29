# Optimizarea-plasamentului-unui-robot-industrial-pentru-paletizarea-selectiva-de-pachete.
# ONGOING PROJECT
Se cere realizarea unui sistem compus dintr-o banda transportoare pe care vin pachete primite de curier
pentru a fi livrate. Aceste pachete au o anumita adresa (citita de un sistem de vedere artificiala si
trimisa controllerului robot pe interfața de rețea). In funcție de adresa specificata exista 10 posibile
destinații. Fiecărei destinații îi este asociata o lisa cu un container care este umplut pana la refuz cu
pachete către acea destinație. Sistemul robot-VA-banda transportoare-containere funcționează
continuu. Pachetele care vin pe banda sunt paletizate selectiv către containerul destinație și când un
container se umple el va fi scos din producție pentru o perioada de timp (20 secunde) pentru a fi
încărcat în mașina. Fiecare container permite stocarea unui număr maxim de cutii. După ce se umple
este scos din producție si cutiile sunt eliminate, returnând containerul gol.
Se cere crearea unui model digital al sistemului de mai sus care generează pachete de 10 tipuri diferite
prin citirea unui mesaj pe interfața de rețea. În funcție de tipul pachetului robotul executa traiectoria de
manipulare către containerul aferent. Containerul are dimensiunea externa 400(mm) lățime, 300mm
(lungime), 270mm (adâncime). Pachetele sunt cuburi de dimensiune 40X40X40mm. Se va calcula
capacitatea maxima a containerului și dispoziția cutiilor in container. Cuplarea modelului digital al
postului de lucru la o aplicație de comanda a creării cutiilor si specificare a tipului lor. Se va implementa
o comunicație pe socket, in care controllerul robot este server si clientul ii transmite o comanda de
creare cutie si tip cutie.
Proiectul este compus doar din programul RobotStudio&Rapid, cu cod comentat astfel încât să se
înțeleagă modalitatea de operare a protocolului de interacțiune (controller Robot-Hercules/Putty/client
TCP).
