# <a name="devicecomplianceactionitem-resource-type"></a>Тип ресурса deviceComplianceActionItem

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Конфигурация запланированного действия
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_list.md)|Коллекция [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Список свойств и связей объектов [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|
|[Получение объекта deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_get.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Чтение свойств и связей объекта [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|
|[Создание объекта deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_create.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Создание объекта [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|
|[Удаление объекта deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_delete.md)|Нет|Удаляет объект [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|
|[Обновление объекта deviceComplianceActionItem](../api/intune_deviceconfig_devicecomplianceactionitem_update.md)|[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Обновление свойств объекта [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|gracePeriodHours|Int32|Время ожидания (в часах) до применения действия. Допустимые значения: от 0 до 8760.|
|actionType|[deviceComplianceActionType](../resources/intune_deviceconfig_devicecomplianceactiontype.md)|Какое действие необходимо выполнить. Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.|
|notificationTemplateId|String|Используемый шаблон сообщения уведомления|
|notificationMessageCCList|Коллекция String|Список идентификаторов групп, которым будет отправлена копия этого сообщения уведомления.|

## <a name="relationships"></a>Связи
None
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```



