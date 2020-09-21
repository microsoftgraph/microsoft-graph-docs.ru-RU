---
title: Тип ресурса схемы
description: Описывает тип контента и способ индексирования каждого свойства элементов в подключении Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0d5182e68fd1b1d53abb5b3fa623f3048abfe723
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083969"
---
# <a name="schema-resource-type"></a>Тип ресурса схемы

Пространство имен: microsoft.graph

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
| baseType   | Строка                             | Необходимо указать значение `microsoft.graph.externalItem`. Обязательный. |
| properties | Коллекция [свойств](property.md) | Свойства, заданные для элементов в подключении. Минимальное число свойств — 1, максимальное — 128. |

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


