---
title: Тип ресурса unifiedApprovalStage
description: Определяет параметры этапов утверждения в объекте unifiedRoleManagementPolicyApprovalRule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b046071cb3468187d75ebd079b4329907e3550c5
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134477"
---
# <a name="unifiedapprovalstage-resource-type"></a>Тип ресурса unifiedApprovalStage

Пространство имен: microsoft.graph

Определяет параметры этапов утверждения в [объекте unifiedRoleManagementPolicyApprovalRule](unifiedrolemanagementpolicyapprovalrule.md) . Указывает основных утверждающих лиц и утверждающих эскалацию на каждом этапе, а также необходимость утверждения и эскалации.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|approvalStageTimeOutInDays|Int32| Количество дней, в течение которых запрос может быть ожидающим ответа, прежде чем он будет автоматически отклонен. |
|escalationApprovers|[Коллекция subjectSet](../resources/subjectset.md)| Утверждающие эскалацию на этом этапе, когда основные утверждающие не отвечают.|
|escalationTimeInMinutes|Int32|Время ожидания запроса от основного утверждающего, прежде чем его можно будет передать утверждающим эскалации.|
|isApproverJustificationRequired|Логическое| Указывает, должен ли утверждающий предоставлять обоснование для своего ответа.|
|isEscalationEnabled|Логическое| Указывает, включена ли эскалация.|
|primaryApprovers|[Коллекция subjectSet](../resources/subjectset.md)| Основные утверждающие на этом этапе.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unifiedApprovalStage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedApprovalStage",
  "approvalStageTimeOutInDays": "Integer",
  "isApproverJustificationRequired": "Boolean",
  "escalationTimeInMinutes": "Integer",
  "primaryApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "isEscalationEnabled": "Boolean",
  "escalationApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ]
}
```

