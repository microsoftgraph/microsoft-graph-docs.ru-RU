# <a name="deviceconfigurationassignment-resource-type"></a>Тип ресурса deviceConfigurationAssignment

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceConfigurationAssignment](../api/intune_deviceconfig_deviceconfigurationassignment_list.md)|Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).|
|[Получение объекта deviceConfigurationAssignment](../api/intune_deviceconfig_deviceconfigurationassignment_get.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).|
|[Создание объекта deviceConfigurationAssignment](../api/intune_deviceconfig_deviceconfigurationassignment_create.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Создание объекта [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).|
|[Удаление объекта deviceConfigurationAssignment](../api/intune_deviceconfig_deviceconfigurationassignment_delete.md)|Нет|Удаляет объект [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).|
|[Обновление объекта deviceConfigurationAssignment](../api/intune_deviceconfig_deviceconfigurationassignment_update.md)|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ИД|string|Ключ назначения.|
|целевой|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Цель назначения для конфигурации устройств.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








