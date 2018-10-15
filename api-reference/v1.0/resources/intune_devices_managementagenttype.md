# <a name="managementagenttype-enum-type"></a>Тип перечисления managementAgentType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Тип агента управления.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|eas|1|Устройство управляется сервером Exchange.|
|mdm|2|Устройство управляется Intune MDM.|
|easMdm|3|Устройство управляется сервером Exchange и Intune MDM.|
|intuneClient|4|Управление клиентом Intune.|
|easIntuneClient|5|Устройство находится под двойным управлением EAS и клиента Intune.|
|configurationManagerClient|8|Устройство управляется диспетчером конфигураций.|
|configurationManagerClientMdm|10|Устройство управляется диспетчером конфигураций и MDM.|
|configurationManagerClientMdmEas|11|Устройство управляется диспетчером конфигураций, MDM и Eas.|
|unknown|16|Тип агента управления неизвестен.|
|jamf|32|Атрибуты устройства полученные от Jamf.|
|googleCloudDevicePolicyController|64|Устройство управляется Google CloudDPC.|








