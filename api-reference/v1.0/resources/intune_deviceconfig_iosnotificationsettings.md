# <a name="iosnotificationsettings-resource-type"></a>Тип ресурса iosNotificationSettings

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Элемент, описывающий параметры уведомлений.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bundleID|Строка|Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.|
|appName|Строка|Имя приложения, которое нужно связать со свойством bundleID.|
|publisher|Строка|Издатель, которого нужно связать со свойством bundleID.|
|enabled|Логический|Указывает, разрешены ли уведомления для этого приложения.|
|showInNotificationCenter|Логический|Указывает, можно ли отображать уведомления в центре уведомлений.|
|showOnLockScreen|Логический|Указывает, можно ли отображать уведомления на экране блокировки.|
|alertType|[iosNotificationAlertType](../resources/intune_deviceconfig_iosnotificationalerttype.md)|Определяет тип оповещения для уведомлений, связанных с этим приложением. Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.|
|badgesEnabled|Логический|Указывает, разрешены ли эмблемы для этого приложения.|
|soundsEnabled|Логический|Указывает, разрешены ли звуковые сигналы для этого приложения.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```



