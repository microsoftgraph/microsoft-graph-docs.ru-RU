# <a name="auditactor-resource-type"></a>Тип ресурса auditActor

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Класс, содержащий свойства субъекта аудита.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|type|Строка|Тип субъекта.|
|userPermissions|Коллекция строк|Список разрешений пользователей во время аудита.|
|applicationId|Строка|ИД приложения AAD.|
|applicationDisplayName|Строка|Имя приложения.|
|userPrincipalName|Строка|Имя участника-пользователя (UPN).|
|servicePrincipalName|Строка|Имя субъекта-службы (SPN).|
|ipAddress|Строка|IP-адрес.|
|userId|Строка|ИД пользователя.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
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
}
```



