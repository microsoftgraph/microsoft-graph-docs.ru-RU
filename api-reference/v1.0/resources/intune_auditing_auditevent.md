# <a name="auditevent-resource-type"></a>Тип ресурса auditEvent

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Класс, содержащий свойства события аудита.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов auditEvent](../api/intune_auditing_auditevent_list.md)|Коллекция [auditEvent](../resources/intune_auditing_auditevent.md)|Список свойств и связей объектов [auditEvent](../resources/intune_auditing_auditevent.md).|
|[Получение объекта auditEvent](../api/intune_auditing_auditevent_get.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|Чтение свойств и связей объекта [auditEvent](../resources/intune_auditing_auditevent.md).|
|[Создание объекта auditEvent](../api/intune_auditing_auditevent_create.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|Создание объекта [auditEvent](../resources/intune_auditing_auditevent.md).|
|[Удаление объекта auditEvent](../api/intune_auditing_auditevent_delete.md)|Нет|Удаляет объект [auditEvent](../resources/intune_auditing_auditevent.md).|
|[Обновление объекта auditEvent](../api/intune_auditing_auditevent_update.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|Обновление свойств объекта [auditEvent](../resources/intune_auditing_auditevent.md).|
|[Функция getAuditCategories](../api/intune_auditing_auditevent_getauditcategories.md)|Коллекция строк|Н/Д|
|[Функция getAuditActivityTypes](../api/intune_auditing_auditevent_getauditactivitytypes.md)|Коллекция строк|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String (строка)|Ключ объекта.|
|displayName|String (строка)|Отображаемое имя события.|
|componentName|String (строка)|Имя компонента.|
|actor|[auditActor](../resources/intune_auditing_auditactor.md)|Пользователь AAD и приложение, связанные с событием аудита.|
|activity|String (строка)|Понятное имя действия.|
|activityDateTime|DateTimeOffset|Дата и время выполнения действия (в формате UTC).|
|activityType|String (строка)|Тип выполненного действия.|
|activityOperationType|String (строка)|Тип операции HTTP для действия.|
|activityResult|String (строка)|Результат действия.|
|correlationId|Guid|Идентификатор клиентского запроса, используемый для согласования действий в системе.|
|resources|Коллекция [auditResource](../resources/intune_auditing_auditresource.md)|Изменяемые ресурсы.|
|category|String (строка)|Категория аудита.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "79199ed9-e50b-4257-8de4-70b9c8685061",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```



