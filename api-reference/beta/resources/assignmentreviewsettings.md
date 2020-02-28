---
title: Тип ресурса Ассигнментревиевсеттингс
description: Тип Ассигнментревиевсеттингс, используемый для свойства Акцессревиевсеттингс политики назначения пакетов Access, предоставляет дополнительные параметры для выбора пользователей, которые должны проверить назначения пакетов доступа из этой политики и как часто они должны быть проверены.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c673d96ab5bb6dbb6f217d5b36f41520b421f5bf
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331425"
---
# <a name="assignmentreviewsettings-resource-type"></a>Тип ресурса Ассигнментревиевсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для свойства **акцессревиевсеттингс** [политики назначения пакетов Access](accesspackageassignmentpolicy.md). Предоставляет дополнительные параметры для выбора пользователей, которые должны просматривать назначения пакетов доступа из этой политики и как часто они должны проверяться.  

## <a name="properties"></a>Свойства

Этот тип имеет следующие свойства:

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| isEnabled| Boolean | Если этот параметр имеет значение true, для назначений из этой политики требуются обзоры доступа. |
| recurrenceType | String | Интервал повторения, например `monthly` или. `quarterly` |
| ревиевертипе | String | Кто должен иметь запрос на выполнение проверки, либо `Self` `Reviewers`. |
| startDateTime | DateTimeOffset | Когда должна начаться Первая проверка. |
| дуратиониндайс | Int32 | Количество дней, в течение которого допускается ввод данных от рецензентов.|
| обсужден | Коллекция [User](userset.md) Collection | Если задано `Reviewers`значение ревиевертипе, эта коллекция указывает пользователей, которые будут рецензентами, по идентификатору или членам группы, используя коллекцию [SingleUser.](singleuser.md) и [граупмемберс](groupmembers.md). |

## <a name="json-representation"></a>Представление JSON


Ниже представлено описание свойства "Просмотр параметров проверки доступа" для политики в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings",
  "baseType": ""
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
