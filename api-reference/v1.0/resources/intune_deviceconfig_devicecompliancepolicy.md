# <a name="devicecompliancepolicy-resource-type"></a>Тип ресурса deviceCompliancePolicy

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Это базовый класс для политик обеспечения соответствия требованиям. Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса. 
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление deviceCompliancePolicies](../api/intune_deviceconfig_devicecompliancepolicy_list.md)|Коллекция [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|Список свойств и связей объектов [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|[Получение deviceCompliancePolicy](../api/intune_deviceconfig_devicecompliancepolicy_get.md)|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|Считывание свойств и связей объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).|
|[Действие assign](../api/intune_deviceconfig_devicecompliancepolicy_assign.md)|Коллекция [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Пока не задокументировано|
|[Действие scheduleActionsForRules](../api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|описание|String (строка)|Указанное администратором описание конфигурации устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|displayName|String (строка)|Указанное администратором имя конфигурации устройства.|
|version|Int32|Версия конфигурации устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|scheduledActionsForRule|Коллекция [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|Список запланированных действий для этого правила.|
|deviceStatuses|Коллекция объектов [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|Список DeviceComplianceDeviceStatus.|
|userStatuses|Коллекция объектов [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Список DeviceComplianceUserStatus.|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|Обзор состояния соответствия требованиям устройств.|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Обзор состояния соответствия требованиям устройств для пользователей.|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Сводка по состоянию параметров обеспечения соответствия требованиям для устройств.|
|assignments|Коллекция [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|Коллекция назначений для этой политики обеспечения соответствия требованиям.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```








