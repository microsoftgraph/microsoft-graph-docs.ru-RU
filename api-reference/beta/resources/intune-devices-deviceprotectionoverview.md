---
title: тип ресурса deviceProtectionOverview
description: Сведения о оборудовании данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 867dba54fd94c86dee017f4c9716eacabd3bee98a0ea2de2fbc6f3c513fc434e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248413"
---
# <a name="deviceprotectionoverview-resource-type"></a>тип ресурса deviceProtectionOverview

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения о оборудовании данного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|Общее число устройств.|
|inactiveThreatAgentDeviceCount|Int32|Устройство с неактивным количеством агентов угроз|
|unknownStateThreatAgentDeviceCount|Int32|Устройство с состоянием агента угрозы как неизвестное количество.|
|pendingSignatureUpdateDeviceCount|Int32|Устройство со старым количеством подписей.|
|cleanDeviceCount|Int32|Чистое количество устройств.|
|pendingFullScanDeviceCount|Int32|Ожидание полного подсчета устройств сканирования.|
|pendingRestartDeviceCount|Int32|Ожидающее перезапуска количество устройств.|
|pendingManualStepsDeviceCount|Int32|В ожидании подсчета ручных действий устройства.|
|pendingOfflineScanDeviceCount|Int32|Ожидание автономного подсчета устройств сканирования.|
|criticalFailuresDeviceCount|Int32|Количество устройств с критическими сбоями.|
|pendingQuickScanDeviceCount|Int32|Ожидание быстрого подсчета устройств сканирования. Допустимые значения 2147483648 2147483647|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024,
  "pendingQuickScanDeviceCount": 1024
}
```




