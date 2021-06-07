---
title: тип userIdentity
description: Представляет идентификатор пользователя Azure AD для рецензента обзора доступа.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 94c0af9a5909966471594ab4c23003282f416849
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750367"
---
# <a name="useridentity-type"></a>тип userIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для обзоров доступа к Azure [AD](accessreviews-root.md)этот тип представляет идентификатор пользователя Azure AD для создателя или рецензента обзора доступа.
В контексте журнала аудита Azure AD это представляет сведения пользователей, которые инициировали или пострадали от действий аудита.

Этот тип наследуется от [удостоверения](identity.md) и имеет одно дополнительное свойство, основное имя пользователя.

## <a name="methods"></a>Methods

Нет.  При создании [accessReview](../api/accessreview-create.md)в тело запроса будут включены объекты этого типа.

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                                                                            |
|:------------------|:-------|:---------------------------------------------------------------------------------------|
| displayName       | String | Отображаемое имя удостоверения. Обратите внимание, что это может быть не всегда доступно или в курсе. |
| id                | String | Уникальный идентификатор удостоверения. Допускается значение NULL.                                                   |
| ipAddress         | String | Указывает IP-адрес клиента, используемый пользователем для выполнения действия (только журнал аудита). |
| userPrincipalName | String | Атрибут userPrincipalName пользователя.                                           |

### <a name="remarks"></a>Заметки

В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="see-also"></a>См. также

| Метод                                                                | Возвращаемый тип                                | Описание                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [Получите рецензенты accessReview](../api/accessreview-listreviewers.md)    | [коллекция userIdentity](useridentity.md) | Получите рецензентов accessReview.   |
| [Добавление рецензента accessReview](../api/accessreview-addreviewer.md)       | Нет.                                      | Добавление рецензента в accessReview.      |
| [Удаление рецензента accessReview](../api/accessreview-removereviewer.md) | Нет.                                      | Удаление рецензента из accessReview. |

## <a name="json-representation"></a>Представление в формате JSON

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


