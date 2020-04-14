---
title: Тип userIdentity
description: Представляет удостоверение пользователя Azure AD для проверяющего, проверяющего доступ.
localization_priority: Normal
author: krbain
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0cb40f4d9815ed0c95f319fd5f112dfd5802f10a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384972"
---
# <a name="useridentity-type"></a>Тип userIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для [просмотров Access](accessreviews-root.md)Azure AD этот тип представляет собой удостоверение пользователя Azure AD для создателя или рецензента проверки доступа.  
В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.

Этот тип наследуется от [Identity](identity.md) и имеет одно дополнительное свойство, имя участника пользователя.

## <a name="methods"></a>Методы

Нет.  При [создании акцессревиев](../api/accessreview-create.md)необходимо включить в текст запроса объекты этого типа.

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
|[Добавление рецензента Акцессревиев](../api/accessreview-addreviewer.md) |      Нет.   |   Добавьте проверяющего в объект Акцессревиев. |
|[Удаление рецензента Акцессревиев](../api/accessreview-removereviewer.md) | Нет.  |   Удаление проверяющего из Акцессревиев. |

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
