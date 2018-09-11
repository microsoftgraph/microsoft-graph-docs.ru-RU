# <a name="devicecomplianceuserstatus-resource-type"></a>Тип ресурса deviceComplianceUserStatus

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceComplianceUserStatus](../api/intune_deviceconfig_devicecomplianceuserstatus_list.md)|Коллекция [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Список свойств и связей объектов [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).|
|[Получение объекта deviceComplianceUserStatus](../api/intune_deviceconfig_devicecomplianceuserstatus_get.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Чтение свойств и связей объекта [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).|
|[Создание объекта deviceComplianceUserStatus](../api/intune_deviceconfig_devicecomplianceuserstatus_create.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Создание объекта [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).|
|[Удаление объекта deviceComplianceUserStatus](../api/intune_deviceconfig_devicecomplianceuserstatus_delete.md)|Нет|Удаляет объект [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).|
|[Обновление объекта deviceComplianceUserStatus](../api/intune_deviceconfig_devicecomplianceuserstatus_update.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Обновление свойств объекта [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|userDisplayName|Строка|Имя пользователя в объекте DevicePolicyStatus.|
|devicesCount|Int32|Количество устройств для этого пользователя.|
|status|[complianceStatus](../resources/intune_shared_compliancestatus.md)|Состояние соответствия требованиям для отчета о политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего изменения отчета о политике.|
|userPrincipalName|Строка|Имя участника-пользователя.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```








