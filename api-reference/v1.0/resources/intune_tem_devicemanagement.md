# <a name="devicemanagement-resource-type"></a>Тип ресурса deviceManagement

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceManagement](../api/intune_tem_devicemanagement_get.md)|[deviceManagement](../resources/intune_tem_devicemanagement.md)|Чтение свойств и связей объекта [deviceManagement](../resources/intune_tem_devicemanagement.md).|
|[Обновление объекта deviceManagement](../api/intune_tem_devicemanagement_update.md)|[deviceManagement](../resources/intune_tem_devicemanagement.md)|Обновление свойств объекта [deviceManagement](../resources/intune_tem_devicemanagement.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Н/Д|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|telecomExpenseManagementPartners|Коллекция [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|Партнеры по управлению затратами на телекоммуникации.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



