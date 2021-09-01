---
title: тип ресурса deviceHealthScriptRemediationHistoryData
description: Количество устройств, исправленных скриптом состояния устройства в заданную дату.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6c456b3edc591c0394446bbb23b6975781da4d4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793812"
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



