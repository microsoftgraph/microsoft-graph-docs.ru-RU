# <a name="iosminimumoperatingsystem-resource-type"></a>Тип ресурса iosMinimumOperatingSystem

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения iOS.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v8_0|Boolean|Версия 8.0 или выше.|
|v9_0|Boolean|Версия 9.0 или выше.|
|v10_0|Boolean|Версия 10.0 или выше.|
|v11_0|Boolean|Версия 11.0 или выше.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true
}
```



