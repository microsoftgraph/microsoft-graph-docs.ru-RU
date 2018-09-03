# <a name="applepushnotificationcertificate-resource-type"></a>Тип ресурса applePushNotificationCertificate

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сертификат push-уведомлений Apple
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта applePushNotificationCertificate](../api/intune_devices_applepushnotificationcertificate_get.md)|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).|
|[Обновление объекта applePushNotificationCertificate](../api/intune_devices_applepushnotificationcertificate_update.md)|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Обновление свойств объекта [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).|
|[Функция downloadApplePushNotificationCertificateSigningRequest](../api/intune_devices_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest.md)|String (строка)|Скачивание запроса на подпись сертификата для push-уведомлений Apple|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String (строка)|Уникальный идентификатор сертификата|
|appleIdentifier|String (строка)|Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.|
|topicIdentifier|String (строка)|Идентификатор темы.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сертификата push-уведомлений Apple.|
|expirationDateTime|DateTimeOffset|Дата и время окончания срока действия для сертификата push-уведомлений Apple.|
|certificate|String (строка)|Н/Д|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



