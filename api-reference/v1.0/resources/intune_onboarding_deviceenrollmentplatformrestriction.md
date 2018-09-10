# <a name="deviceenrollmentplatformrestriction-resource-type"></a>Тип ресурса deviceEnrollmentPlatformRestriction

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ограничения на регистрацию для определенных платформ
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|platformBlocked|Boolean|Указывает, блокируется ли регистрация платформы|
|personalDeviceEnrollmentBlocked|Boolean|Указывает, блокируется ли регистрация личных устройств|
|osMinimumVersion|String|Минимальная поддерживаемая версия ОС|
|osMaximumVersion|String|Максимальная поддерживаемая версия ОС|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```








