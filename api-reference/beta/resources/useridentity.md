---
title: Тип userIdentity
description: Представляет удостоверение пользователя Azure AD для проверяющего, проверяющего доступ.
localization_priority: Normal
author: krbain
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1ab0a102cf430a98a0a5662af30cdd8cd36a3430
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846074"
---
# <a name="useridentity-type"></a>Тип userIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для [просмотров Access](accessreviews-root.md)Azure AD этот тип представляет собой удостоверение пользователя Azure AD для создателя или рецензента проверки доступа.
В контексте журнала аудита Azure AD — это сведения о пользователях, которые были инициированы или затронуты действием аудита.

Этот тип наследуется от [Identity](identity.md) и имеет одно дополнительное свойство, имя участника пользователя.

## <a name="methods"></a>Methods

Отсутствуют.  При [создании акцессревиев](../api/accessreview-create.md)необходимо включить в текст запроса объекты этого типа.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание|
|:---------------|:--------|:----------|
| `displayName` | `String` | Отображаемое имя удостоверения. Обратите внимание, что эта возможность не всегда доступна или не актуальна.    |
| `id`          | `String` | Уникальный идентификатор удостоверения.  |
| `ipAddress`| `String`| IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита).|
| `userPrincipalName`|`String` | Атрибут userPrincipalName пользователя. |

## <a name="remarks"></a>Заметки

In some circumstances, the unique identifier for the actor may not be available.
In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="see-also"></a>См. также

| Метод                                                                | Возвращаемый тип                                | Описание                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [Получение рецензентов Акцессревиев](../api/accessreview-listreviewers.md)    | Коллекция [userIdentity](useridentity.md) | Получение рецензентов объекта Акцессревиев.   |
| [Добавление рецензента Акцессревиев](../api/accessreview-addreviewer.md)       | Отсутствуют.                                      | Добавьте проверяющего в объект Акцессревиев.      |
| [Удаление рецензента Акцессревиев](../api/accessreview-removereviewer.md) | Отсутствуют.                                      | Удаление проверяющего из Акцессревиев. |

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
