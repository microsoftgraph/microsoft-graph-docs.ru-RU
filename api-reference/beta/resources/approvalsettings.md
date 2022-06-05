---
title: Сложный тип approvalSettings
description: Параметры для утверждения, определенные в правиле политики управления ролем.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0fd8af9a314052dab87908fde5987850899e8f90
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900221"
---
# <a name="approvalsettings-complex-type"></a>Сложный тип approvalSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры для утверждения, определенные в правиле политики управления ролем.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|approvalMode|Строка|Один из `SingleStage`, `Serial`, `Parallel`( `NoApproval` по умолчанию). `NoApproval` используется в том случае `isApprovalRequired` , если это `false`.|
|approvalStages|[Коллекция approvalStage](../resources/approvalstage.md)|Если требуется утверждение, один или два элемента этой коллекции определяют каждый из этапов утверждения. Пустой массив, если утверждение не требуется.|
|isApprovalRequired|Boolean|Указывает, требуется ли утверждение для запросов в этой политике.|
|isApprovalRequiredForExtension|Boolean|Указывает, требуется ли утверждение для продления назначения пользователем.|
|isRequestorJustificationRequired|Boolean|Указывает, требуется ли инициатору запроса предоставить обоснование в своем запросе.|

## <a name="relationships"></a>Отношения
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
      "@odata.type": "microsoft.graph.approvalStage"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "approvalSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


