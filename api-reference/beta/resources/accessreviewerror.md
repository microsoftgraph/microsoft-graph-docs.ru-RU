---
title: Тип ресурса accessReviewError
description: Представляет ошибку, которая произошла в жизненном цикле экземпляра проверки доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7e0b773bd8b1393b160cb666db4d5f19d9501a54
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697934"
---
# <a name="accessreviewerror-resource-type"></a>Тип ресурса accessReviewError

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет ошибку, которая произошла в жизненном цикле экземпляра проверки доступа. Этот ресурс доступен только для чтения.

Наследуется от [genericError](../resources/genericerror.md).

## <a name="properties"></a>Свойства
| Свойство                     | Тип     | Описание                          |
| :--------------------------- | :------  | :----------                          |
| code  |String  | Представляет тип ошибки. Наследуется от genericError. Только для чтения. |
| message |String | Представляет сведения об ошибке. Наследуется от genericError. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление JSON
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
