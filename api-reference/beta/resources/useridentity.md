---
title: тип userIdentity
description: Представляет идентификатор пользователя Azure AD для рецензента обзора доступа.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 9379955a4356ff9c969e4813fbf9b812316aa821
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719859"
---
# <a name="useridentity-type"></a>тип userIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для обзоров доступа к Azure [AD](accessreviews-root.md)этот тип представляет идентификатор пользователя Azure AD для создателя или рецензента обзора доступа.
В контексте журнала аудита Azure AD это представляет сведения пользователей, которые инициировали или пострадали от действий аудита.

Этот тип наследуется от [удостоверения](identity.md) и имеет одно дополнительное свойство, основное имя пользователя.

## <a name="methods"></a>Methods

Нет  При создании [accessReview](../api/accessreview-create.md)в тело запроса будут включены объекты этого типа.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание|
|:---------------|:--------|:----------|
| `displayName` | `String` | Отображаемое имя удостоверения. Обратите внимание, что это может быть не всегда доступно или в курсе.    |
| `id`          | `String` | Уникальный идентификатор удостоверения.  |
| `ipAddress`| `String`| Указывает IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).|
| `userPrincipalName`|`String` | Атрибут userPrincipalName пользователя. |

## <a name="remarks"></a>Заметки

В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="see-also"></a>См. также

| Метод                                                                | Возвращаемый тип                                | Описание                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [Получите рецензенты accessReview](../api/accessreview-listreviewers.md)    | [коллекция userIdentity](useridentity.md) | Получите рецензентов accessReview.   |
| [Добавление рецензента accessReview](../api/accessreview-addreviewer.md)       | Нет                                      | Добавление рецензента в accessReview.      |
| [Удаление рецензента accessReview](../api/accessreview-removereviewer.md) | Нет                                      | Удаление рецензента из accessReview. |

## <a name="json-representation"></a>Представление JSON

Вот представление JSON этого типа.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
  "userPrincipalName": "String",
  "ipAddress": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


