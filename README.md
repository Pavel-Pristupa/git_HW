# Linux terminal (GitBash) commands
____
__1) Посмотреть где я.__   
	`pwd`  
__2) Создать папку.__   
	`mkdir git_bash_HW`  
__3) Зайти в папку.__   
	`cd git_bash_HW`  
__4) Создать 3 папки.__   
	`mkdir folder_1 folder_2 folder_3`  
__5) Зайти в любоую папку.__   
	`cd folder_1`  
__6) Создать 5 файлов (3 txt, 2 json).__   
	`touch file_1.txt file_2.txt file_3.txt json_1.json json_2.json`  
__7) Создать 3 папки.__   
	`mkdir p_1 p_2 p_3`  
__8) Вывести список содержимого папки.__   
	`ls -la`  
__9) + Открыть любой txt файл.__     
	`vim file_1.txt`  
__10) + написать туда что-нибудь, любой текст.__   
	➡️ __i__   
	*insert some text*  
__11) + сохранить и выйти.__   
	➡️ __Esc__  
	➡️ `:wq`  
__12) Выйти из папки на уровень выше.__   
	`cd ..`  
__13) переместить любые 2 файла, которые вы создали, в любую другую папку.__   
	`mv -i ./folder_1/{file_1.txt,file_2.txt} ./folder_2/`  
__14) скопировать любые 2 файла, которые вы создали, в любую другую папку.__   
	`cp ./folder_1/{file_3.txt,json_1.json} ./folder_3/`  
__15) Найти файл по имени.__   
	`find -iname "file_1.txt"`  
__16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.__   
	`tail -f file_1.txt`  
__17) вывести несколько первых строк из текстового файла.__   
	`head -n3 file_1.txt`  
__18) вывести несколько последних строк из текстового файла.__   
	`tail -n4 file_1.txt`  
__19) просмотреть содержимое длинного файла (команда less) изучите как она работает.__   
	`less file_1.txt`  
__20) вывести дату и время.__   
	`date`  
____

## Задание *  
__1) Отправить http запрос на сервер.__   
http://162.55.220.72:5005/terminal-hw-request  
	`curl 'http://162.55.220.72:5005/terminal-hw-request'`  
	`curl 'http://162.55.220.72:5005/get_method?name=(Pavel_Pristupa)&age=(32)'`  
__2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13.__   
*Я добавил в скрипт пункт 2 + небольшое описание происходящего.*  
`touch script_1.sh`  
`chmod +x script_1.sh`  
`vim script_1.sh`  
➡️ __i__ 
```bash
echo ""  
echo "===================================================="  
echo "I will create a general folder with 3 folders inside"  
echo "3 .txt and 2 .json files in the first folder"  
echo "Then I will create 3 folders inside the first one"  
echo "and move 2 .txt files into the first of them"  
echo "===================================================="  
echo ""  
mkdir git_bash_gr27  
cd git_bash_gr27  
mkdir folder_1 folder_2 folder_3  
cd folder_1  
touch file_1.txt file_2.txt file_3.txt json_1.json json_2.json  
mkdir ff_1 ff_2 ff_3  
ls -la  
mv -i ./{file_1.txt,file_2.txt} ./ff_1/  
```  
➡️ __Esc__  
➡️ `:wq`  
__Для запуска скрипта использовать команду:__  
`./script_1.sh`  
