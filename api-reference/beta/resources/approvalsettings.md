---
title: Сложный тип approvalSettings
description: Используется для свойства requestApprovalSettings политики назначения пакета доступа. Предоставляет дополнительные параметры для выбора, кто должен утвердить каждый запрос.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 85d47e09de1b4d8f687a8dff2abf6aff1af0f21f
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777731"
---
# <a name="approvalsettings-complex-type"></a>Сложный тип approvalSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для `requestApprovalSettings` свойства политики назначения пакета [доступа.](accesspackageassignmentpolicy.md) Предоставляет дополнительные параметры для выбора, кто должен утвердить каждый запрос. 

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| isApprovalRequired | Boolean | Если задается false, утверждение для запросов в этой политике не требуется. |
| isApprovalRequiredForExtension | Boolean| Если задается false, то для пользователя, у которого уже есть назначение для расширения назначения, утверждение не требуется. |
| isRequestorJustificationRequired | Boolean | Указывает, требуется ли запрашивать обоснование в своем запросе. |
| approvalMode| String | Один из `NoApproval` , `SingleStage` или `Serial` . Используется, `NoApproval` если `isApprovalRequired` заведомо неверно. |
| approvalStages | [Коллекция approvalStage](approvalstage.md)| Если требуется утверждение, один или два элемента этой коллекции определяют каждый из этапов утверждения. Пустой массив, если утверждение не требуется.  |

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление свойства параметров утверждения запроса в JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings"
}-->

```json
{
    "isApprovalRequired": true,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": true,
    "approvalMode": "Serial",
    "approvalStages": [{"@odata.type": "microsoft.graph.approvalStage"}]
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


