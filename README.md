# crontab_script_journalisation
Ecrire un script, le lancer dans un crontab et le journaliser

# creation du script et fichier log dans un repertoire lab
touch /home/kali/lab/script1.sh
touch /home/kali/lab/scriptLog.log

# accéder à l'intérieur via vim
vim /home/kali/lab/script.sh

# insertion du shebang et afficher un "hello wordl"
#!/bin/bash/
echo "Hello World"

# pour lancer l'execution et la journalisation via le crontab
crontab -e
*/1 * * * * /home/kali/lab/script1.sh >> /home/kali/lab/scriptLog.log


