---
title: тип ресурса accessReviewReviewer
description: Представляет рецензента, с которым связались для проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f5fbeda2ca839fe07009a46ab2bccd1deb502f17
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259348"
---
# <a name="accessreviewreviewer-resource-type"></a>тип ресурса accessReviewReviewer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Объект, представляющий удостоверения проверяющих, с которыми связывались для завершения проверки.

Наследует от [объекта](entity.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| createdDateTime | DateTimeOffset | Дата, когда рецензент был добавлен для проверки доступа. |
| displayName | Строка | Имя рецензента. |
| id | String | Идентификатор рецензента. Наследуется от [сущности](entity.md). |
| userPrincipalName | String | Основное имя пользователя. |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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
