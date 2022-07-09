---
title: Тип userIdentity
description: Представляет Azure AD пользователя для рецензента проверки доступа.
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e42f862cfbb82982ce91a0ed7339f19f9469037b
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698256"
---
# <a name="useridentity-type"></a>Тип userIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для Azure AD [проверки](accessreviews-root.md) доступа этот тип представляет Azure AD удостоверение пользователя для создателя или рецензента проверки доступа.
В контексте журнала аудита Azure AD представляет сведения о пользователе, инициированные или затронутые действием аудита.

Этот тип наследуется от [удостоверения](identity.md) и имеет одно дополнительное свойство — имя участника-пользователя пользователя.

## <a name="methods"></a>Методы

Нет.  Объекты этого типа следует включать в текст запроса при [создании accessReview](../api/accessreview-create.md).

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                                                                            |
|:------------------|:-------|:---------------------------------------------------------------------------------------|
| displayName       | Строка | Отображаемое имя удостоверения. Обратите внимание, что это может быть не всегда доступно или актуально. |
| id                | String | Уникальный идентификатор удостоверения. Допускается значение null.                                                   |
| ipAddress         | String | Указывает IP-адрес клиента, используемый пользователем, выполняющее действие (только журнал аудита). |
| userPrincipalName | String | Атрибут userPrincipalName пользователя.                                           |

### <a name="remarks"></a>Заметки

В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="see-also"></a>См. также

| Метод                                                                | Возвращаемый тип                                | Описание                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [Получение рецензентов accessReview](../api/accessreview-listreviewers.md)    | [Коллекция userIdentity](useridentity.md) | Получение рецензентов accessReview.   |
| [Добавление рецензента accessReview](../api/accessreview-addreviewer.md)       | Нет.                                      | Добавление рецензента в accessReview.      |
| [Удаление рецензента accessReview](../api/accessreview-removereviewer.md) | Нет.                                      | Удаление рецензента из accessReview. |

## <a name="json-representation"></a>Представление JSON

Ниже приведено представление типа в формате JSON.

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


