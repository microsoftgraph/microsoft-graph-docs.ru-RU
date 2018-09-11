# <a name="notificationmessagetemplate-resource-type"></a>Тип ресурса notificationMessageTemplate

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сообщения уведомлений отправляются пользователям, которые не отвечают политикам соответствия требованиям, определяемым администратором. Администраторы выбирают уведомления и настраивают их в консоли администрирования Intune, используя страницу создания политики соответствия требованиям в разделе "Действия для несоответствия". Используйте объект notificationMessageTemplate, чтобы создать собственные настраиваемые уведомления, которые могут выбрать администраторы во время настройки действий в случае несоответствия требованиям.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_list.md)|Коллекция объектов [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Список свойств и связей объектов [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Получение объекта notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_get.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Чтение свойств и связей объекта [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Создание объекта notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_create.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Создание объекта [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Удаление объекта notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_delete.md)|Нет|Удаление объекта [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Обновление объекта notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_update.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Обновление свойств объекта [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Действие sendTestMessage](../api/intune_notification_notificationmessagetemplate_sendtestmessage.md)|Нет|Отправляет проверочное сообщение, используя объект notificationMessageTemplate, указанный в языковом стандарте по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|displayName|String (строка)|Отображаемое имя для шаблона сообщения уведомления.|
|defaultLocale|String (строка)|Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.|
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune_notification_notificationtemplatebrandingoptions.md)|Параметры фирменной символики шаблона сообщения. Фирменная символика определяется в консоли администрирования Intune. Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|localizedNotificationMessages|Коллекция объектов [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|Список локализованных сообщений для шаблона сообщения уведомления.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String"
}
```








