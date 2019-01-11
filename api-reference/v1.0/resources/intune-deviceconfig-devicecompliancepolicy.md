---
title: Тип ресурса deviceCompliancePolicy
description: 'Это базовый класс для политик обеспечения соответствия требованиям. Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса. '
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2ab919a24c7c2819963ce047612f5a829913060
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834414"
---
# <a name="devicecompliancepolicy-resource-type"></a>Тип ресурса deviceCompliancePolicy

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Это базовый класс для политик обеспечения соответствия требованиям. Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса. 
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление deviceCompliancePolicies](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|Коллекция [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|Список свойств и связей объектов [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|[Получение deviceCompliancePolicy](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|Считывание свойств и связей объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|[Действие assign](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Пока не задокументировано|
|[Действие scheduleActionsForRules](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|None|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|описание|Строка|Указанное администратором описание конфигурации устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|displayName|Строка|Указанное администратором имя конфигурации устройства.|
|version|Int32|Версия конфигурации устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|scheduledActionsForRule|Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|Список запланированных действий для этого правила.|
|deviceStatuses|Коллекция объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Список DeviceComplianceDeviceStatus.|
|userStatuses|Коллекция объектов [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Список DeviceComplianceUserStatus.|
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
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



