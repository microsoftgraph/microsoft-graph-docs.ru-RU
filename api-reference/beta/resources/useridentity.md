---
title: Тип userIdentity
description: Представляет удостоверение пользователя Azure AD для рецензента проверки доступа.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 5451216ea41e6de286b5ecc0de2bed1b7ce7c8cf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132974"
---
# <a name="useridentity-type"></a>Тип userIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для проверок доступа Azure [AD](accessreviews-root.md)этот тип представляет удостоверение пользователя Azure AD для создателя или рецензента проверки доступа.
В контексте журнала аудита Azure AD это сведения о пользователях, которые инициировали или были затронуты действиями аудита.

Этот тип наследуется от [удостоверения](identity.md) и имеет одно дополнительное свойство, имя пользователя-пользователя.

## <a name="methods"></a>Методы

Нет.  При создании accessReview объекты этого типа будут включены в тело [запроса.](../api/accessreview-create.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание|
|:---------------|:--------|:----------|
| `displayName` | `String` | Отображаемое имя удостоверения. Обратите внимание, что это может быть не всегда доступно или не всегда в курсе.    |
| `id`          | `String` | Уникальный идентификатор удостоверения.  |
| `ipAddress`| `String`| Указывает IP-адрес клиента, используемый пользователем, выполнив действие (только в журнале аудита).|
| `userPrincipalName`|`String` | Атрибут userPrincipalName пользователя. |

## <a name="remarks"></a>Заметки

В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="see-also"></a>См. также

| Метод                                                                | Возвращаемый тип                                | Описание                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [Просмотр рецензентов accessReview](../api/accessreview-listreviewers.md)    | [Коллекция userIdentity](useridentity.md) | Получите проверяющих accessReview.   |
| [Добавление рецензента accessReview](../api/accessreview-addreviewer.md)       | Нет.                                      | Добавление рецензента в accessReview.      |
| [Удаление рецензента accessReview](../api/accessreview-removereviewer.md) | Нет.                                      | Удаление рецензента из accessReview. |

## <a name="json-representation"></a>Представление в формате JSON

Вот представление типа в JSON.

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


