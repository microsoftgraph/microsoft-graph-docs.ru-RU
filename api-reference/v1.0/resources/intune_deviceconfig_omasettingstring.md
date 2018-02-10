# <a name="omasettingstring-resource-type"></a>Тип ресурса omaSettingString

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определение строки параметра OMA.

Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя. Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|description|Строка|Описание. Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|omaUri|Строка|OMA. Наследуется от ресурса [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|value|Строка|Значение.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже этот ресурс представлен в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



