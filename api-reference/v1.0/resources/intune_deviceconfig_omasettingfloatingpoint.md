# <a name="omasettingfloatingpoint-resource-type"></a>Тип ресурса omaSettingFloatingPoint

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определение плавающей запятой параметра OMA.

Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String (строка)|Отображаемое имя. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|description|String (строка)|Описание. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|omaUri|String (строка)|OMA. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|value|Single|Значение.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1.5
}
```



