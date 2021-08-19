---
title: тип ресурса deviceHealthScriptRemediationSummary
description: Количество развернутых скриптов для здоровья устройств и количество устройств, исправленных скриптами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3843bf13e7129f4025b1c520f49900aa5f5c8ffe379aca22f3d69eff17412403
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251276"
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




