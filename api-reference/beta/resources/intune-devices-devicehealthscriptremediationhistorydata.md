---
title: тип ресурса deviceHealthScriptRemediationHistoryData
description: Количество устройств, исправленных скриптом состояния устройства в заданную дату.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a7578a8455b3c74f843c090522ad5d3e491cd1b1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59144331"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a>тип ресурса deviceHealthScriptRemediationHistoryData

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Количество устройств, исправленных скриптом состояния устройства в заданную дату.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|date|Date|Дата, в которую устройства были исправлены с помощью скрипта состояния устройства.|
|remediatedDeviceCount|Int32|Количество устройств, исправленных скриптом для здоровья устройств.|
|noIssueDeviceCount|Int32|Количество устройств, которые не имеют проблем со сценарием здоровья устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistoryData",
  "date": "String (Date)",
  "remediatedDeviceCount": 1024,
  "noIssueDeviceCount": 1024
}
```



