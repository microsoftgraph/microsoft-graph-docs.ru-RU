---
title: Тип ресурса Девицепротектионовервиев
description: Сведения об оборудовании для данного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fcdcbe69c1c5d94a00ec50e7e7b29b11a471441f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528596"
---
# <a name="deviceprotectionoverview-resource-type"></a>Тип ресурса Девицепротектионовервиев

Пространство имен: Microsoft. Graph

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



