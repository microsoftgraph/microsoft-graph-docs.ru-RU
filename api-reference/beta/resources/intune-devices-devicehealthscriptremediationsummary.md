---
title: Тип ресурса Девицехеалсскриптремедиатионсуммари
description: Количество развернутых сценариев работоспособности устройств и количество устройств, которые были исправлены в сценариях.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7dd3a1b1ab22c2ac834150d1e1ad09938ed27550
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299431"
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




