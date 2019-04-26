---
title: Тип userIdentity
description: 'Для проверок доступа Azure AD этот тип представляет удостоверение пользователя Azure AD для проверяющего, проверяющего доступ.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 554aa9d38b4635ab3410fd95441b5c5045a1f1f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345051"
---
# <a name="useridentity-type"></a>Тип userIdentity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для [просмотров Access](accessreviews-root.md)Azure AD этот тип представляет собой удостоверение пользователя Azure AD для создателя или рецензента проверки доступа.  
В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.

Этот тип наследуется от [Identity](identity.md) и имеет одно дополнительное свойство, имя участника пользователя.

## <a name="methods"></a>Методы

Отсутствуют.  При [создании Акцессревиев](../api/accessreview-create.md)необходимо включить в текст запроса объекты этого типа.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| `displayName` | `String` | Отображаемое имя удостоверения. Обратите внимание, что эта возможность не всегда доступна или не актуальна.    |
| `id`          | `String` | Уникальный идентификатор удостоверения.  |
| `ipAddress`| `String`| IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).|
| `userPrincipalName`|`String` | Атрибут userPrincipalName пользователя. |

## <a name="remarks"></a>Заметки

В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="see-also"></a>См. также

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение рецензентов Акцессревиев](../api/accessreview-listreviewers.md) |       Коллекция [userIdentity](useridentity.md)| Получение рецензентов объекта Акцессревиев. |
|[Добавление рецензента Акцессревиев](../api/accessreview-addreviewer.md) |      Отсутствуют.   |   Добавьте проверяющего в объект Акцессревиев. |
|[Удаление рецензента Акцессревиев](../api/accessreview-removereviewer.md) | Отсутствуют.  |   Удаление проверяющего из Акцессревиев. |

## <a name="json-representation"></a>Представление JSON

Ниже показано представление типа в формате JSON.

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
