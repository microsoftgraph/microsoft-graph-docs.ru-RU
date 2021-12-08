---
title: Тип ресурса deviceCompliancePolicy
description: 'Это базовый класс для политик обеспечения соответствия требованиям. Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса. '
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 507b2a6f6d1ffc3c560979709932acf61b251d5a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61344836"
---
# <a name="devicecompliancepolicy-resource-type"></a>Тип ресурса deviceCompliancePolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Это базовый класс для политик обеспечения соответствия требованиям. Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса. 

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление deviceCompliancePolicies](../api/intune-shared-devicecompliancepolicy-list.md)|Коллекция [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|Список свойств и связей объектов [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|[Получение deviceCompliancePolicy](../api/intune-shared-devicecompliancepolicy-get.md)|[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|Считывание свойств и связей объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|**Конфигурация устройств**|
|[Действие assign](../api/intune-shared-devicecompliancepolicy-assign.md)|Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Пока не задокументировано|
|[Действие scheduleActionsForRules](../api/intune-shared-devicecompliancepolicy-scheduleactionsforrules.md)|None|Н/Д|
|[Действие refreshDeviceComplianceReportSummarization](../api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)|Нет|Н/Д|
|**Набор политик**|
|[действие hasPayloadLinks](../api/intune-shared-devicecompliancepolicy-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|description|Строка|Указанное администратором описание конфигурации устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|displayName|String|Указанное администратором имя конфигурации устройства.|
|version|Int32|Версия конфигурации устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Конфигурация устройств**|
|scheduledActionsForRule|Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Список запланированных действий для этого правила.|
|deviceStatuses|Коллекция [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Список DeviceComplianceDeviceStatus.|
|userStatuses|Коллекция [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Список DeviceComplianceUserStatus.|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Обзор состояния соответствия требованиям устройств.|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|Обзор состояния соответствия требованиям устройств для пользователей.|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка по состоянию параметров обеспечения соответствия требованиям для устройств.|
|assignments|Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Коллекция назначений для этой политики обеспечения соответствия требованиям.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



