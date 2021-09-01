---
title: тип ресурса deviceHealthScriptRemediationSummary
description: Количество развернутых скриптов для здоровья устройств и количество устройств, исправленных скриптами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac9e06cdbc8aa5ba754528459e52142b7e4f3679
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820690"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a>тип ресурса deviceHealthScriptRemediationSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Количество развернутых скриптов для здоровья устройств и количество устройств, исправленных скриптами.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|scriptCount|Int32|Количество развернутых скриптов для здоровья устройств.|
|remediatedDeviceCount|Int32|Количество устройств, исправленных скриптами для здоровья устройств.|

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



