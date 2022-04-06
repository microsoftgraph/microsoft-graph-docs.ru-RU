---
title: тип ресурса accessPackageApprovalStage
description: Используется для свойства этапов параметров утверждения. Указывает основные, откаты и утверждения эскалации на каждом этапе.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cffd48048af6d9b44ef475cdc3adcc6d9f0da05f
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608393"
---
# <a name="accesspackageapprovalstage-complex-type"></a>accessPackageApprovalStage сложный тип

Пространство имен: microsoft.graph

Используется для **свойства этапов** параметров [утверждения](accesspackageassignmentapprovalsettings.md) в политике [назначения пакета доступа](accesspackageassignmentpolicy.md). Указывает основные, откаты и утверждения эскалации на каждом этапе.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|durationBeforeAutomaticDenial|Длительность|Количество дней, в которые запрос может быть отложен до автоматического отключаемого ответа.|
|durationBeforeEscalation|Длительность|Если требуется эскалация, время ожидания запроса от основного утвержденного.|
|escalationApprovers|[коллекция subjectSet](../resources/subjectset.md)|Если эскалация включена, а основные одобрители не реагируют до времени эскалации, пользователи, которым будет предложено утвердить запросы, будут запрашивать. |
|fallbackEscalationApprovers|[коллекция subjectSet](../resources/subjectset.md)|Субъекты, как правило, пользователи, которые являются утверждениями эскалации отката.|
|fallbackPrimaryApprovers|[коллекция subjectSet](../resources/subjectset.md)|Субъекты, как правило, пользователи, которые являются основными утверждениями отката.|
|isApproverJustificationRequired|Boolean|Указывает, требуется ли одобрение для обоснования утверждения запроса.|
|isEscalationEnabled|Boolean|Если `true`на этом этапе утверждения настроен один или несколько **escalationApprovers** .|
|primaryApprovers|[коллекция subjectSet](../resources/subjectset.md)|Субъекты, как правило, пользователи, которым будет предложено утвердить запросы. Коллекция [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) или [externalSponsors](externalsponsors.md).|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageApprovalStage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageApprovalStage",
  "durationBeforeAutomaticDenial": "String (duration)",
  "isApproverJustificationRequired": "Boolean",
  "isEscalationEnabled": "Boolean",
  "durationBeforeEscalation": "String (duration)",
  "primaryApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "fallbackPrimaryApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "escalationApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "fallbackEscalationApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ]
}
```


