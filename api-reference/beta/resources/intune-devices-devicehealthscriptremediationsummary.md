---
title: Тип ресурса Девицехеалсскриптремедиатионсуммари
description: Количество развернутых сценариев работоспособности устройств и количество устройств, которые были исправлены в сценариях.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e538ba04a9dc5007331b8dde3f4d6ec854938e91
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690625"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a>Тип ресурса Девицехеалсскриптремедиатионсуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Количество развернутых сценариев работоспособности устройств и количество устройств, которые были исправлены в сценариях.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|скрипткаунт|Int32|Количество развернутых сценариев работоспособности устройств.|
|remediatedDeviceCount|Int32|Количество устройств, исправленных сценариями работоспособности устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationSummary",
  "scriptCount": 1024,
  "remediatedDeviceCount": 1024
}
```





