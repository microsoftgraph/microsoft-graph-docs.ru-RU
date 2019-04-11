---
title: Тип ресурса Девицепротектионовервиев
description: Сведения об оборудовании для данного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f76918b5a959a6621fb7f5c6480a7a2513afead
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804314"
---
# <a name="deviceprotectionoverview-resource-type"></a>Тип ресурса Девицепротектионовервиев

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения об оборудовании для данного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Тоталрепортеддевицекаунт|Int32|Общее количество устройств.|
|Инактивесреатажентдевицекаунт|Int32|Устройство с неактивным числом агентов угроз|
|Ункновнстатесреатажентдевицекаунт|Int32|Устройство с состоянием агента угроз "неизвестное количество".|
|Пендингсигнатуреупдатедевицекаунт|Int32|Устройство со старым количеством подписей.|
|Клеандевицекаунт|Int32|Очистка числа устройств.|
|Пендингфуллскандевицекаунт|Int32|Количество устройств, ожидающих полного сканирования.|
|Пендингрестартдевицекаунт|Int32|Количество устройств, ожидающих перезапуска.|
|Пендингмануалстепсдевицекаунт|Int32|Количество устройств, ожидающих действий, выполняемых вручную.|
|Пендингоффлинескандевицекаунт|Int32|Количество устройств, ожидающих автономной проверки.|
|Критикалфаилуресдевицекаунт|Int32|Количество устройств критических сбоев.|

## <a name="relationships"></a>Отношения
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





