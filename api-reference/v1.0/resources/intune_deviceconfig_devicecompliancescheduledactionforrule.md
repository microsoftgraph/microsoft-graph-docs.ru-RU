# <a name="devicecompliancescheduledactionforrule-resource-type"></a>Тип ресурса deviceComplianceScheduledActionForRule

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Запланированное действие для правила
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceComplianceScheduledActionForRule](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_list.md)|Коллекция [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Список свойств и связей объектов [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).|
|[Получение объекта deviceComplianceScheduledActionForRule](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_get.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Чтение свойств и связей объекта [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).|
|[Создание объекта deviceComplianceScheduledActionForRule](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_create.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).|
|[Удаление объекта deviceComplianceScheduledActionForRule](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_delete.md)|Нет|Удаляет объект [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).|
|[Обновление объекта deviceComplianceScheduledActionForRule](../api/intune_deviceconfig_devicecompliancescheduledactionforrule_update.md)|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Обновление свойств объекта [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|ruleName|Cтрока|Имя правила, к которому применяется это запланированное действие.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|scheduledActionConfigurations|Коллекция [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|Список конфигураций запланированных действий для этой политики соответствия требованиям.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScheduledActionForRule"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```








