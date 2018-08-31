# <a name="omasettingstringxml-resource-type"></a>Тип ресурса omaSettingStringXml

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определение строки параметра OMA в формате XML.

Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка​|Отображаемое имя. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|description|Строка​|Описание. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|omaUri|Строка​|OMA. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|fileName|Строка​|Имя файла, связанное со свойством Value (XML).|
|value|Двоичный|Значение (массив байтов в кодировке UTF8).|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```



