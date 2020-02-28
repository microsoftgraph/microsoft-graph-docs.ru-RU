---
title: сложный тип Аппровалсеттингс
description: Используется для свойства Рекуестаппровалсеттингс политики назначения пакетов Access. Предоставляет дополнительные параметры для выбора лиц, которые должны утверждать каждый запрос.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e248e47cf94e2c26e80b505cbaead450e03561d4
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331442"
---
# <a name="approvalsettings-complex-type"></a>сложный тип Аппровалсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для `requestApprovalSettings` свойства [политики назначения пакетов Access](accesspackageassignmentpolicy.md). Предоставляет дополнительные параметры для выбора лиц, которые должны утверждать каждый запрос. 

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| исаппровалрекуиред | Логический | Если задано значение false, то для запросов в этой политике утверждение не требуется. |
| исаппровалрекуиредфорекстенсион | Логический| Если задано значение false, то утверждение не требуется для пользователя, который уже имеет назначение для расширения назначения. |
| исрекуесторжустификатионрекуиред | Логический | Указывает, требуется ли запрашивающему для предоставления обоснования в запросе. |
| аппровалмоде| String | Один из `NoApproval`, `SingleStage` или `Serial`. `NoApproval` Используется при `isApprovalRequired` значении false. |
| аппровалстажес | Коллекция [аппровалстаже](approvalstage.md)| Если необходимо утверждение, то один или два элемента этой коллекции определяют каждый из стадий утверждения. Пустой массив, если утверждение не нужно.  |

## <a name="json-representation"></a>Представление JSON

Ниже приведено представление свойства параметров утверждения запроса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings",
  "baseType": ""
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
