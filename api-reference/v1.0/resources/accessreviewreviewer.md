---
title: тип ресурса accessReviewReviewer
description: Представляет рецензента, с которым связались для проверки доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a2a51908f73278e592ec02852c96f75570b7646
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162147"
---
# <a name="accessreviewreviewer-resource-type"></a>тип ресурса accessReviewReviewer

Пространство имен: microsoft.graph

Представляет удостоверения проверяющих, с которыми связывались для завершения проверки.

Наследует от [объекта](entity.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| createdDateTime | DateTimeOffset | Дата, когда рецензент был добавлен для проверки доступа. |
| displayName | Строка | Имя рецензента. |
| id | Строка | Идентификатор рецензента. Наследуется от [сущности](entity.md). |
| userPrincipalName | String | Имя основного пользователя рецензента. |


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
