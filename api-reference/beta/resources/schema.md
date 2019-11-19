---
title: Тип ресурса схемы
description: Описывает тип контента и способ индексирования каждого свойства элементов в подключении Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 77c17345a6a9408a8208f73f03dd98033f2b6a36
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704138"
---
# <a name="schema-resource-type"></a>Тип ресурса схемы

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает тип контента и способ индексирования каждого свойства элементов в [подключении](externalconnection.md)Microsoft Search.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод                                                    | Возвращаемый тип                   | Описание |
|:----------------------------------------------------------|:------------------------------|:--|
| [Создание схемы](../api/externalconnection-post-schema.md) | Нет *или* [схема](schema.md) | Регистрация схемы подключения. |
| [Получение схемы](../api/schema-get.md)                        | [schema](schema.md)           | Чтение свойств объекта Schema. |

## <a name="properties"></a>Свойства

| Свойство   | Тип                               | Описание                |
|:-----------|:-----------------------------------|:---------------------------|
| baseType   | String                             | Возможные значения: `microsoft.graph.externalItem` и `microsoft.graph.externalFile`. Обязательно. |
| properties | Коллекция [свойств](property.md) | Свойства, заданные для элементов в подключении. Минимальное число свойств — 1, максимальное — 64. Является обязательным `baseType` , если задано значение `microsoft.graph.externalItem`. Игнорируется `baseType` , если задано значение `microsoft.graph.externalFile`. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [{"@odata.type": "microsoft.graph.property"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
