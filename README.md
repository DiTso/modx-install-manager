Модуль для установки елементов в MODX EVO

1. Создаем новый модуль Install с кодом: 
$modulePath = $modx->config['base_path'].'assets/modules/install-manager/';
include_once($modulePath . "index.php");

2. записываем папку install-manager в assets/module


из багов: 
- ошибка underfined иногда появляется пока не решил багу + не работает установка демо контента по той же причине
- нужно пойтись в файлике instprocessor.php  выпилить все что касается sqlParser оно там не надо у нас подключение к базе и так есть 

доработки: 
- добавить проверку что б не перезаписывало файлы а как минимум делало бекап старыхъ


