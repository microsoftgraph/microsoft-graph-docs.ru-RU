---
title: тип ресурсов accessReviewError
description: Представляет ошибку, которая произошла в жизненном цикле экземпляра проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dc0fe94daaba28bf92b20cb986760b0d3eb0901b
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534388"
---
# <a name="accessreviewerror-resource-type"></a>тип ресурсов accessReviewError

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет ошибку, которая произошла в жизненном цикле экземпляра проверки доступа. Этот ресурс только для чтения.

Наследует от [genericError](../resources/genericerror.md).

## <a name="properties"></a>Свойства
| Свойство                     | Тип     | Описание                          |
| :--------------------------- | :------  | :----------                          |
| code  |Строка  | Представляет тип ошибки. Наследуется от genericError. Только для чтения. |
| message |String | Представляет сведения об ошибках. Наследуется от genericError. Только для чтения.|

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewError"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
