# <a name="devicecategory-resource-type"></a>Тип ресурса deviceCategory

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceCategory](../api/intune_devices_devicecategory_get.md)|[deviceCategory](../resources/intune_devices_devicecategory.md)|Чтение свойств и связей объекта [deviceCategory](../resources/intune_devices_devicecategory.md).|
|[Обновление объекта deviceCategory](../api/intune_devices_devicecategory_update.md)|[deviceCategory](../resources/intune_devices_devicecategory.md)|Обновление свойств объекта [deviceCategory](../resources/intune_devices_devicecategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор категории устройства. Только для чтения.|

## <a name="relationships"></a>Отношения
Нет
## <a name="json-representation"></a>Представление JSON
Ниже этот ресурс представлен в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)"
}
```



