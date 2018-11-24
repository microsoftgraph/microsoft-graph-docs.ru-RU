# <a name="omasettingboolean-resource-type"></a>Тип ресурса omaSettingBoolean

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Логическое определение параметров OMA.

Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|description|String|Описание. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|omaUri|String|OMA. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|value|Boolean|Значение|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



