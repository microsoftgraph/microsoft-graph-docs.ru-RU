---
title: тип ресурса deviceHealthScriptRemediationSummary
description: Количество развернутых скриптов для здоровья устройств и количество устройств, исправленных скриптами.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2eb1177b80f95572599e6205cfdd00499e65b0f3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59144316"
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



