---
title: Тип ресурса схемы
description: Схема подключения определяет, как контент, добавляемый в подключение, будет использоваться в различных интерфейсах Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ff14f04adb31d99aadec15cb9368e09a098c7a26
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192870"
---
# <a name="schema-resource-type"></a>Тип ресурса схемы

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Схема [подключения](externalconnection.md) определяет, как внешнее содержимое будет использоваться в различных интерфейсах Microsoft Graph. Schema — это плоский список всех свойств, которые вы планируете добавить к подключению вместе с их атрибутами, метками и псевдонимами. Перед добавлением элементов в подключение необходимо зарегистрировать схему.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод                                                    | Возвращаемый тип                   | Описание |
|:----------------------------------------------------------|:------------------------------|:--|
| [Создание схемы](../api/externalconnection-post-schema.md) | Нет *или* [схема](schema.md) | Регистрация схемы подключения. |
| [Получение схемы](../api/schema-get.md)                        | [schema](schema.md)           | Чтение свойств объекта Schema. |

## <a name="properties"></a>Свойства

| Свойство   | Тип                               | Описание                |
|:-----------|:-----------------------------------|:---------------------------|
| baseType   | String                             | Необходимо указать значение `microsoft.graph.externalItem`. Обязательно. |
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


