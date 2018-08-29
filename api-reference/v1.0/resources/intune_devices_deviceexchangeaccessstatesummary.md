# <a name="deviceexchangeaccessstatesummary-resource-type"></a>Тип ресурса deviceExchangeAccessStateSummary

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сводка по состоянию доступа к Exchange для устройств
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowedDeviceCount|Int32|Общее количество устройств с состоянием доступа к Exchange "Разрешено".|
|blockedDeviceCount|Int32|Общее количество устройств с состоянием доступа к Exchange "Заблокировано".|
|quarantinedDeviceCount|Int32|Общее количество устройств с состоянием доступа к Exchange "Помещено в карантин".|
|unknownDeviceCount|Int32|Общее количество устройств с состоянием доступа к Exchange "Неизвестно".|
|unavailableDeviceCount|Int32|Общее количество устройств, для которых не найдены сведения о состоянии доступа к Exchange.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```



