---
title: Тип ресурса схемы
description: Описывает тип контента и способ индексирования каждого свойства элементов в подключении Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8bd5d47f444d7054aecbf7b0a63e57643837a340
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938788"
---
# <a name="schema-resource-type"></a>Тип ресурса схемы

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает тип контента и способ индексирования каждого свойства элементов в [подключении](externalconnection.md)Microsoft Search.

## <a name="methods"></a>Методы

| Метод                                                    | Возвращаемый тип                   | Описание |
|:----------------------------------------------------------|:------------------------------|:--|
| [Создание схемы](../api/externalconnection-post-schema.md) | Нет *или* [схема](schema.md) | Регистрация схемы подключения. |
| [Получение схемы](../api/schema-get.md)                        | [схемы](schema.md)           | Чтение свойств объекта Schema. |

## <a name="properties"></a>Свойства

| Свойство   | Тип                               | Описание                |
|:-----------|:-----------------------------------|:---------------------------|
| baseType   | Строка                             | Возможные значения: `microsoft.graph.externalItem` и `microsoft.graph.externalFile`. Обязательный элемент. |
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
