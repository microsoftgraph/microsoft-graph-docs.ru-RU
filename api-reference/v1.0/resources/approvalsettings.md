---
title: Тип ресурса approvalSettings
description: Параметры для утверждения, определенные в правиле политики управления ролем.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2dc0240fd272e4d79209ee37bf79f293052eb400
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134448"
---
# <a name="approvalsettings-resource-type"></a>Тип ресурса approvalSettings

Пространство имен: microsoft.graph

Параметры для утверждения, определенные в правиле политики управления ролем.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|approvalMode|String|Один из `SingleStage`, `Serial`, `Parallel`( `NoApproval` по умолчанию). `NoApproval` используется в том случае `isApprovalRequired` , если это `false`.|
|approvalStages|[Коллекция unifiedApprovalStage](../resources/unifiedapprovalstage.md)|Если требуется утверждение, один или два элемента этой коллекции определяют каждый из этапов утверждения. Пустой массив, если утверждение не требуется.|
|isApprovalRequired|Boolean|Указывает, требуется ли утверждение для запросов в этой политике.|
|isApprovalRequiredForExtension|Логическое|Указывает, требуется ли утверждение для продления назначения пользователем.|
|isRequestorJustificationRequired|Логическое|Указывает, требуется ли инициатору запроса предоставить обоснование в своем запросе.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.approvalSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approvalSettings",
  "isApprovalRequired": "Boolean",
  "isApprovalRequiredForExtension": "Boolean",
  "isRequestorJustificationRequired": "Boolean",
  "approvalMode": "String",
  "approvalStages": [
    {
      "@odata.type": "microsoft.graph.unifiedApprovalStage"
    }
  ]
}
```

