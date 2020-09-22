---
title: Тип ресурса Девицехеалсскриптремедиатионхистори
description: Количество устройств, исправленных сценарием работоспособности устройства на указанную дату в последний момент времени изменения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51f85549ecceb1a867bd08f5ef21b223a22c3f67
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060309"
---
# <a name="devicehealthscriptremediationhistory-resource-type"></a>Тип ресурса Девицехеалсскриптремедиатионхистори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Количество устройств, исправленных сценарием работоспособности устройства на указанную дату в последний момент времени изменения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата, на которую рассчитывается журнал результатов для хеалсскрипт.|
|хисторидата|Коллекция [девицехеалсскриптремедиатионхисторидата](../resources/intune-devices-devicehealthscriptremediationhistorydata.md)|Количество устройств, исправленных сценарием работоспособности устройства на указанную дату.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistory",
  "lastModifiedDateTime": "String (timestamp)",
  "historyData": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
      "date": "String (Date)",
      "remediatedDeviceCount": 1024,
      "noIssueDeviceCount": 1024
    }
  ]
}
```






