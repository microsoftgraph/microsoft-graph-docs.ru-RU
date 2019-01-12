---
title: Тип удостоверению пользователя
description: 'Для Azure AD вызвать обзоры, этот тип представляет удостоверение пользователя Azure AD для рецензент проверки доступа.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 80e8cc68d4fc2f642be6c748b762fe47c7489d59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932282"
---
# <a name="useridentity-type"></a>Тип удостоверению пользователя

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Для Azure AD, [дается обзор доступа](accessreviews-root.md)этот тип представляет удостоверение пользователя Azure AD для рецензент проверки доступа.  
В контексте журнал аудита Azure AD представляет сведений о пользователе, который инициировал или затронутого пользователем действия аудита.

Этот тип наследуется от [удостоверения](identity.md) и одного дополнительного свойства имя участника-пользователя пользователя.

## <a name="methods"></a>Methods

Нет.  Объекты этого типа будет включать в теле запроса при [создании accessReview](../api/accessreview-create.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `displayName` | `String` | Отображаемое имя удостоверения. Обратите внимание, что не всегда возможно, доступен или актуальными.    |
| `id`          | `String` | Уникальный идентификатор удостоверения.  |
| `ipAddress`| `String`| Указывает IP-адрес клиента, используемых пользователь, выполняющий действие (только для журнала аудита).|
| `userPrincipalName`|`String` | Атрибут userPrincipalName пользователя. |

## <a name="remarks"></a>Заметки

В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

## <a name="relationships"></a>Связи

Нет.

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение accessReview рецензентов](../api/accessreview-listreviewers.md) |       Коллекция [удостоверению пользователя](useridentity.md)| Получите рецензентов accessReview. |
|[Добавление accessReview редактор](../api/accessreview-addreviewer.md) |      Нет.   |   Добавьте проверяющий accessReview. |
|[Удаление accessReview редактор](../api/accessreview-removereviewer.md) | Нет.  |   Удаление рецензента из accessReview. |

## <a name="json-representation"></a>Представление JSON

Ниже представлена JSON типа.

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
 "userPrincipalName": "String"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
