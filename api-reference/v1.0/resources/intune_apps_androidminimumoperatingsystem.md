# <a name="androidminimumoperatingsystem-resource-type"></a>Тип ресурса androidMinimumOperatingSystem

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для минимальной версии операционной системы, необходимой для мобильного приложения Android.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|v4_0|Boolean|Версия 4.0 или выше.|
|v4_0_3|Boolean|Версия 4.0.3 или выше.|
|v4_1|Boolean|Версия 4.1 или выше.|
|v4_2|Boolean|Версия 4.2 или выше.|
|v4_3|Boolean|Версия 4.3 или выше.|
|v4_4|Boolean|Версия 4.4 или выше.|
|v5_0|Boolean|Версия 5.0 или выше.|
|v5_1|Boolean|Версия 5.1 или выше.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMinimumOperatingSystem",
  "v4_0": true,
  "v4_0_3": true,
  "v4_1": true,
  "v4_2": true,
  "v4_3": true,
  "v4_4": true,
  "v5_0": true,
  "v5_1": true
}
```



