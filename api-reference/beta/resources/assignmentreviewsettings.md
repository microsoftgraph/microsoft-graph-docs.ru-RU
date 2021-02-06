---
title: Тип ресурса assignmentReviewSettings
description: Тип assignmentReviewSettings, используемый для свойства accessReviewSettings политики назначения пакета доступа, предоставляет дополнительные параметры, чтобы выбрать, кто должен просмотреть назначения пакетов доступа из этой политики и как часто их необходимо просмотреть.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bde8c6d330eda7e100071edbf2190e170ca913ea
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131343"
---
# <a name="assignmentreviewsettings-resource-type"></a>Тип ресурса assignmentReviewSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для свойства **accessReviewSettings** политики [назначения пакета доступа.](accesspackageassignmentpolicy.md) Предоставляет дополнительные параметры, чтобы выбрать, кто должен просмотреть назначения пакетов доступа из этой политики и как часто их необходимо просмотреть.  

## <a name="properties"></a>Свойства

Этот тип имеет следующие свойства:

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| isEnabled| Boolean | Если имеется true, для назначений из этой политики требуются проверки доступа. |
| recurrenceType | Строка | Интервал повторения, например `monthly` или `quarterly` . |
| reviewerType | Строка | Кто должен быть предложено сделать отзыв, либо `Self` `Reviewers` . |
| startDateTime | DateTimeOffset | Когда должен начаться первый обзор. |
| durationInDays | Int32 | Количество дней, в течение которые можно разрешить ввод данных от проверяющих.|
| рецензенты | [Коллекция userSet](userset.md) | Если это reviewerType, эта коллекция указывает пользователей, которые будут рецензентами по ИД или в качестве членов группы, используя коллекцию `Reviewers` [singleUser](singleuser.md) и [groupMembers.](groupmembers.md) |

## <a name="json-representation"></a>Представление в формате JSON


Ниже приводится представление свойства параметров проверки доступа политики в JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings"
}-->

```json
{
  "isEnabled": true,
  "recurrenceType": "quarterly",
  "reviewerType": "Self",
  "startDateTime": "2020-01-23T07:59:59.998Z",
  "durationInDays": 25,
  "reviewers": []
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignmentReviewSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


