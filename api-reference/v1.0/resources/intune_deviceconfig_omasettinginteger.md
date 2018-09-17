# <a name="omasettinginteger-resource-type"></a>Тип ресурса omaSettingInteger

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определение целого числа параметра OMA.

Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Cтрока|Отображаемое имя. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|описание|Cтрока|Описание. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|omaUri|Cтрока|OMA. Наследуется от [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|значение|Int32|Значение.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```








