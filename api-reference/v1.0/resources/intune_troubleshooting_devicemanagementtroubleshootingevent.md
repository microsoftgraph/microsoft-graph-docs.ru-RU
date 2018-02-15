# <a name="devicemanagementtroubleshootingevent-resource-type"></a>Тип ресурса deviceManagementTroubleshootingEvent

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Событие, представляющее общий сбой.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceManagementTroubleshootingEvent](../api/intune_troubleshooting_devicemanagementtroubleshootingevent_list.md)|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|Список свойств и связей объектов [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).|
|[Получение объекта deviceManagementTroubleshootingEvent](../api/intune_troubleshooting_devicemanagementtroubleshootingevent_get.md)|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|Чтение свойств и связей объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).|
|[Создание объекта deviceManagementTroubleshootingEvent](../api/intune_troubleshooting_devicemanagementtroubleshootingevent_create.md)|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|Создание объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).|
|[Удаление объекта deviceManagementTroubleshootingEvent](../api/intune_troubleshooting_devicemanagementtroubleshootingevent_delete.md)|Нет|Удаляет объект [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).|
|[Обновление объекта deviceManagementTroubleshootingEvent](../api/intune_troubleshooting_devicemanagementtroubleshootingevent_update.md)|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|Обновление свойств объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|eventDateTime|DateTimeOffset|Время возникновения события.|
|correlationId|String|ИД, используемый для трассировки сбоя в службе.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String"
}
```



