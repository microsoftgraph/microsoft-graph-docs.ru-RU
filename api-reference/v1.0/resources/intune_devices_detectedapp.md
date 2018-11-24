# <a name="detectedapp-resource-type"></a>Тип ресурса detectedApp

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список detectedApps](../api/intune_devices_detectedapp_list.md)|Коллекция [detectedApp](../resources/intune_devices_detectedapp.md)|Список свойств и связей объектов [detectedApp](../resources/intune_devices_detectedapp.md).|
|[Получение detectedApp](../api/intune_devices_detectedapp_get.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|Получение свойств и связей объекта [detectedApp](../resources/intune_devices_detectedapp.md).|
|[Создание объекта detectedApp](../api/intune_devices_detectedapp_create.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|Создание объекта [detectedApp](../resources/intune_devices_detectedapp.md).|
|[Удаление объекта detectedApp](../api/intune_devices_detectedapp_delete.md)|Нет|Удаление объекта [detectedApp](../resources/intune_devices_detectedapp.md).|
|[Обновление detectedApp](../api/intune_devices_detectedapp_update.md)|[detectedApp](../resources/intune_devices_detectedapp.md)|Обновление свойств объекта [detectedApp](../resources/intune_devices_detectedapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для обнаруженного приложения. Он создается Intune автоматически при создании приложения. Только для чтения.|
|displayName|String|Имя обнаруженного приложения. Только для чтения|
|version|String|Версия обнаруженного приложения. Только для чтения|
|sizeInByte|Int64|Размер обнаруженного приложения в байтах. Только для чтения|
|deviceCount|Int32|Количество устройств, на которых было успешно установлено это приложение.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevices|Коллекция [managedDevice](../resources/intune_devices_manageddevice.md)|Устройства, на которых установлено обнаруженное приложение|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```



