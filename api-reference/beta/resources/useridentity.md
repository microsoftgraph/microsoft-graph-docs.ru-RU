---
title: Тип удостоверению пользователя
description: 'Для Azure AD вызвать обзоры, этот тип представляет удостоверение пользователя Azure AD для рецензент проверки доступа.  '
ms.openlocfilehash: 6cbbe7aa017572bcd753a57edbf82751ac4986a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077814"
---
# <a name="useridentity-type"></a>Тип удостоверению пользователя

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Для Azure AD, [дается обзор доступа](accessreviews-root.md)этот тип представляет удостоверение пользователя Azure AD для рецензент проверки доступа.  
В контексте журнал аудита Azure AD представляет сведений о пользователе, который инициировал или затронутого пользователем действия аудита.

Этот тип наследуется от [удостоверения](identity.md) и одного дополнительного свойства имя участника-пользователя пользователя.

## <a name="methods"></a>Methods

Отсутствуют.  Объекты этого типа будет включать в теле запроса при [создании accessReview](../api/accessreview-create.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
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
|[Добавление accessReview редактор](../api/accessreview-addreviewer.md) |      Отсутствуют.   |   Добавьте проверяющий accessReview. |
|[Удаление accessReview редактор](../api/accessreview-removereviewer.md) | Отсутствуют.  |   Удаление рецензента из accessReview. |

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
