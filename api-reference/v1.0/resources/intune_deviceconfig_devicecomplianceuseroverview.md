# <a name="devicecomplianceuseroverview-resource-type"></a>Тип ресурса deviceComplianceUserOverview

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceComplianceUserOverview](../api/intune_deviceconfig_devicecomplianceuseroverview_get.md)|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).|
|[Обновление объекта deviceComplianceUserOverview](../api/intune_deviceconfig_devicecomplianceuseroverview_update.md)|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Обновление свойств объекта [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|pendingCount|Int32|Количество ожидающих пользователей.|
|notApplicableCount|Int32|Количество неприменимых пользователей|
|successCount|Int32|Количество успешных пользователей.|
|errorCount|Int32|Количество пользователей с ошибками.|
|failedCount|Int32|Количество пользователей со сбоями.|
|lastUpdateDateTime|DateTimeOffset|Время последнего обновления.|
|configurationVersion|Int32|Версия политики для этого обзора|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



