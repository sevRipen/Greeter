# Специально для канала Крипторелакс https://www.youtube.com/@Crypto-Relax 
# Наш телеграм : https://t.me/CRYPTORELAKS
* Официальные гайды от ZkSync era : https://era.zksync.io/docs/dev/building-on-zksync/hello-world.html и https://era.zksync.io/docs/api/hardhat/getting-started.html#learn-more
* Кран Goerli: https://goerlifaucet.com/ ;
* Натсройка тестовой сети ZkSync: https://era.zksync.io/docs/dev/troubleshooting/important-links.html ;
* Бридж для перевода в тестовую сеть zksync era : https://portal.zksync.io/bridge ;
* Эксплорер для проверки контракта и транзакций : https://goerli.explorer.zksync.io/ ;

# Действия :
1) Скачаиваем ( если нет ) Visual Studio Code : https://code.visualstudio.com/ 
2) Добваляем в VSC нужные расширения ( Solidity, npm Intellisense ), если по ходу работы в VSC выдает ошибки и всплывает окно в нижнем правом углу с предложением скачать пакеты - соглашаемся ( у всех может быть по-разному ), чего будет не хватать из пакетов ( yarn, node.js и тд ) устанавливаем вручную ( гайдов полно в интернете )
3) Добавляем ссылку с этого репозитория в VSC : https://github.com/sevRipen/Greeter
4) Подготавливаем метамаск : добавляем сеть ZkSync Era Testnet через https://chainlist.org/?testnets=true&search=zksync+era+testnet или вручную
5) Запрашиваем тестовые Goerli на https://goerlifaucet.com/
6) Отправляем Goerli ETH на ZkSync Era Testnet через мост https://portal.zksync.io/bridge (внизу справа проверяем чтобы стояла ZkSync Era Goerli
7) Переходим обратно в VSC и в терминале пишем команду :  ```yarn init -y``` или ```npm init -y``` 
8) Затем вводим : ```sudo npm i -D typescript ts-node ethers@^5.7.2 zksync-web3@^0.13.1 hardhat @matterlabs/hardhat-zksync-solc @matterlabs/hardhat-zksync-deploy```
9) Далее : ```yarn hardhat compile```        или     ```npx hardhat compile```
10) В ```deploy.ts``` вставляем свой приватный ключ от метамаска
11) И последняя команда : ```yarn hardhat deploy-zksync``` или ```npx hardhat deploy-zksync``` и ждем окончания деплоя контракта
12) Верефицируем контракт (см. видео )
13) Взаимодействуем со смартконтрактом (см. видео )
