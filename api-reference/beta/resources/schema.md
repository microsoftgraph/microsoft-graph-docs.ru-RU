---
title: Тип ресурса схемы
description: Описывает тип контента и способ индексирования каждого свойства элементов в подключении Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c7780cd7c31da98a618053febba1b75c5e318931
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990275"
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
| baseType   | String                             | Необходимо указать значение `microsoft.graph.externalItem`. Обязательный. |
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
