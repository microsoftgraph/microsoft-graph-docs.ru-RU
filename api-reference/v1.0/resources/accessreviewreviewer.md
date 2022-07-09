---
title: Тип ресурса accessReviewReviewer
description: Представляет рецензента, к которому обращались для проверки доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ab365ee1d3b3fd53696e8fa92a2aa25dfdfd0a97
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698417"
---
# <a name="accessreviewreviewer-resource-type"></a>Тип ресурса accessReviewReviewer

Пространство имен: microsoft.graph

Представляет удостоверения рецензентов, с которыми связывались для завершения проверки.

Наследует [от сущности](entity.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| createdDateTime | DateTimeOffset | Дата добавления рецензента для проверки доступа. |
| displayName | Строка | Имя рецензента. |
| id | String | Идентификатор рецензента. Наследуется от [сущности](entity.md). |
| userPrincipalName | String | Имя участника-пользователя рецензента. |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewer",
  "id": "String",
  "displayName": "String",
  "userPrincipalName": "String",
  "createdDateTime": "String (timestamp)",
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
