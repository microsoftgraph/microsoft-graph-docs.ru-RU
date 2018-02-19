# <a name="androidforworkenrollmentprofile-resource-type"></a>Тип ресурса androidForWorkEnrollmentProfile

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Профиль регистрации, используемый для регистрации устройств COSU с помощью управления облачными клиентами от Google.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidForWorkEnrollmentProfiles](../api/intune_androidforwork_androidforworkenrollmentprofile_list.md)|Коллекция [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Список свойств и связей объектов [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Получение объекта androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_get.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Чтение свойств и связей объекта [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Создание объекта androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_create.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Создание объекта [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Удаление объекта androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_delete.md)|Нет|Удаление объекта [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[Обновление объекта androidForWorkEnrollmentProfile](../api/intune_androidforwork_androidforworkenrollmentprofile_update.md)|[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md)|Обновление свойств объекта [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).|
|[revokeToken action](../api/intune_androidforwork_androidforworkenrollmentprofile_revoketoken.md)|Нет|Н/Д|
|[Действие createToken](../api/intune_androidforwork_androidforworkenrollmentprofile_createtoken.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accountId|String|GUID клиента, которому принадлежит профиль регистрации.|
|id|String|Уникальный GUID профиля регистрации.|
|name|String|(Нерекомендуемое) Отображаемое имя профиля регистрации.|
|displayName|String|Отображаемое имя для профиля регистрации.|
|description|String|Описание профиля регистрации.|
|createdDateTime|DateTimeOffset|Дата и время создания профиля регистрации.|
|modifiedDateTime|DateTimeOffset|(Нерекомендуемое) Дата и время последнего изменения профиля регистрации.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения профиля регистрации.|
|tokenValue|String|Значение последнего созданного маркера для этого профиля регистрации.|
|tokenExpirationDateTime|DateTimeOffset|Дата и время, когда истекает срок действия последнего созданного маркера.|
|totalEnrollmentCount|Int32|(Нерекомендуемое) Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.|
|enrolledDeviceCount|Int32|Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.|
|qrCode|String|(Нерекомендуемое) Строка, используемая для создания QR-кода маркера.|
|qrCodeContent|String|Строка, используемая для создания QR-кода маркера.|
|qrCodeImage|[mimeContent](../resources/intune_androidforwork_mimecontent.md)|Строка, используемая для создания QR-кода маркера.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "name": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "totalEnrollmentCount": 1024,
  "enrolledDeviceCount": 1024,
  "qrCode": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```



