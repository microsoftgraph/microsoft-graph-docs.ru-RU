---
title: Тип ресурса Девицепротектионовервиев
description: Сведения об оборудовании для данного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e9bdadb7cef003a8d22653660d516afe8357d59
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784142"
---
# <a name="deviceprotectionoverview-resource-type"></a>Тип ресурса Девицепротектионовервиев

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения об оборудовании для данного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|тоталрепортеддевицекаунт|Int32|Общее количество устройств.|
|инактивесреатажентдевицекаунт|Int32|Устройство с неактивным числом агентов угроз|
|ункновнстатесреатажентдевицекаунт|Int32|Устройство с состоянием агента угроз "неизвестное количество".|
|пендингсигнатуреупдатедевицекаунт|Int32|Устройство со старым количеством подписей.|
|клеандевицекаунт|Int32|Очистка числа устройств.|
|пендингфуллскандевицекаунт|Int32|Количество устройств, ожидающих полного сканирования.|
|пендингрестартдевицекаунт|Int32|Количество устройств, ожидающих перезапуска.|
|пендингмануалстепсдевицекаунт|Int32|Количество устройств, ожидающих действий, выполняемых вручную.|
|пендингоффлинескандевицекаунт|Int32|Количество устройств, ожидающих автономной проверки.|
|критикалфаилуресдевицекаунт|Int32|Количество устройств критических сбоев.|

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
  "criticalFailuresDeviceCount": 1024
}
```



