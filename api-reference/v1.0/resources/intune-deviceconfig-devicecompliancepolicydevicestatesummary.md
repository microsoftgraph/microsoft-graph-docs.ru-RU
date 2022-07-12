---
title: Тип ресурса deviceCompliancePolicyDeviceStateSummary
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f04912e9afa39eeeb7305153225c00ce6757643
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736463"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a>Тип ресурса deviceCompliancePolicyDeviceStateSummary

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceCompliancePolicyDeviceStateSummary](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).|
|[Обновление объекта deviceCompliancePolicyDeviceStateSummary](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|inGracePeriodCount|Int32|Количество устройств, для которых действует льготный период.|
|configManagerCount|Int32|Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.|
|id|String|Ключ объекта.|
|unknownDeviceCount|Int32|Количество неизвестных устройств.|
|notApplicableDeviceCount|Int32|Количество неприменимых устройств.|
|compliantDeviceCount|Int32|Количество устройств, соответствующих требованиям.|
|remediatedDeviceCount|Int32|Количество исправленных устройств.|
|nonCompliantDeviceCount|Int32|Количество устройств, не соответствующих требованиям.|
|errorDeviceCount|Int32|Количество устройств с ошибками.|
|conflictDeviceCount|Int32|Количество конфликтующих устройств|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





