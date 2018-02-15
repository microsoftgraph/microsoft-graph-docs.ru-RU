# <a name="localizednotificationmessage-resource-type"></a>Тип ресурса localizedNotificationMessage

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Текстовое содержимое шаблона сообщения уведомления для указанного языкового стандарта.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_list.md)|Коллекция [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|Список свойств и связей объектов [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).|
|[Получение объекта localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_get.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|Чтение свойств и связей объекта [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).|
|[Создание объекта localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_create.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|Создание объекта [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).|
|[Удаление объекта localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_delete.md)|Нет|Удаляет объект [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).|
|[Обновление объекта localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_update.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|Обновление свойств объекта [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|locale|String|Языковой стандарт, для которого предназначено сообщение.|
|subject|String|Тема шаблона сообщения.|
|messageTemplate|String|Содержимое шаблона сообщения.|
|isDefault|Boolean|Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка. Этот флаг можно только устанавливать. Чтобы снять его, задайте значение true для аналогичного свойства другого локализованного сообщения уведомления.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```



