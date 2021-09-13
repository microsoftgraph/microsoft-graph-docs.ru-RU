---
title: тип ресурса deviceProtectionOverview
description: Сведения о оборудовании данного устройства.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 310d7e8623dad1baac2d77b6b8e23e527e4e4709
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125864"
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



