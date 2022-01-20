---
title: тип ресурсов governanceInsight
description: Представляет сведения, представленные рецензенту для accessReviewInstanceDecisionItem.
author: shubhamguptacal
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fdbe8aa65487e1d872e7f0943ae5582958fcaaec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137276"
---
# <a name="governanceinsight-resource-type"></a>тип ресурсов governanceInsight

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Представляет сведения, представленные рецензенту для [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md). Аналитика рекомендации рецензентам, которые помогут им завершить обзоры доступа.

Этот ресурс является абстрактным типом для [производных userSignInInsight.](usersignininsight.md)

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание |
| :---------------| :---------- | :---------- |
| id | Строка | Идентификатор проницательности. Только для чтения. |
| insightCreatedDateTime | DateTimeOffset | Указывает, когда была создана проницательность. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceInsight",
  "keyProperty": "id"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceinsight",
  "id": "String",
  "insightCreatedDateTime": "DateTimeOffset"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "governanceinsight resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
