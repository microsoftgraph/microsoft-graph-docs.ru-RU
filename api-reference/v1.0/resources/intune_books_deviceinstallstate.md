# <a name="deviceinstallstate-resource-type"></a>Тип ресурса deviceInstallState

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства состояния установки для устройства.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceInstallStates](../api/intune_books_deviceinstallstate_list.md)|Коллекция [deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Список свойств и связей объектов [deviceInstallState](../resources/intune_books_deviceinstallstate.md).|
|[Получение объекта deviceInstallState](../api/intune_books_deviceinstallstate_get.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Чтение свойств и связей объекта [deviceInstallState](../resources/intune_books_deviceinstallstate.md).|
|[Создание объекта deviceInstallState](../api/intune_books_deviceinstallstate_create.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Создание объекта [deviceInstallState](../resources/intune_books_deviceinstallstate.md).|
|[Удаление объекта deviceInstallState](../api/intune_books_deviceinstallstate_delete.md)|Нет|Удаляет объект [deviceInstallState](../resources/intune_books_deviceinstallstate.md).|
|[Обновление объекта deviceInstallState](../api/intune_books_deviceinstallstate_update.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Обновление свойств объекта [deviceInstallState](../resources/intune_books_deviceinstallstate.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ИД|Строка|Ключ объекта.|
|deviceName|Строка|Имя устройства.|
|deviceId|Строка|Идентификатор устройства.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации.|
|installState|[installState](../resources/intune_books_installstate.md)|Состояние установки электронной книги. Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.|
|errorCode|Строка|Код ошибки для сбоев при установке.|
|osVersion|Строка|Версия ОС.|
|osDescription|Строка|Описание ОС.|
|userName|Строка|Имя пользователя устройства.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```








