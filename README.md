const Web3 = require('web3');

// Подключение к локальному узлу Ethereum (например, Ganache)
const web3 = new Web3('http://localhost:8545');

// Пример вызова метода блокчейна (получение номера последнего блока)
web3.eth.getBlockNumber()
  .then(blockNumber => {
    console.log('Номер последнего блока:', blockNumber);
  })
  .catch(error => {
    console.error('Ошибка:', error);
  });
