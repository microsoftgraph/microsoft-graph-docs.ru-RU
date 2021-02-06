---
title: Сложный тип approvalSettings
description: Используется для свойства requestApprovalSettings политики назначения пакета доступа. Предоставляет дополнительные параметры, чтобы выбрать, кто должен утвердить каждый запрос.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 99892e0943b993fe43edb4bd104fd2a3a8736a51
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135263"
---
# <a name="approvalsettings-complex-type"></a>Сложный тип approvalSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для `requestApprovalSettings` свойства политики назначения пакета [доступа.](accesspackageassignmentpolicy.md) Предоставляет дополнительные параметры, чтобы выбрать, кто должен утвердить каждый запрос. 

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| isApprovalRequired | Boolean | Если задается false, утверждение для запросов в этой политике не требуется. |
| isApprovalRequiredForExtension | Boolean| Если задается false, то для пользователя, у которого уже есть назначение для расширения назначения, утверждение не требуется. |
| isRequestorJustificationRequired | Boolean | Указывает, требуется ли запрашивать обоснование в своем запросе. |
| approvalMode| Строка | Один из `NoApproval` , `SingleStage` или `Serial` . Используется, `NoApproval` если `isApprovalRequired` заведомо false. |
| approvalStages | [Коллекция approvalStage](approvalstage.md)| Если требуется утверждение, один или два элемента этой коллекции определяют каждый из этапов утверждения. Пустой массив, если утверждение не требуется.  |

## <a name="json-representation"></a>Представление в формате JSON

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


