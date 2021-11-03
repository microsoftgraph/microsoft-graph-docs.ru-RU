---
title: Тип ресурса схемы
description: Схема подключения определяет, как содержимое, добавленное в подключение, будет использоваться в различных Graph microsoft.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8dbf6a4df47f9afb3e24effbf9d90759dc87d677
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729208"
---
# <a name="schema-resource-type"></a>Тип ресурса схемы

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Схема [подключения](externalconnectors-externalconnection.md) определяет, как внешний контент будет использоваться в различных Graph Microsoft. Схема — это плоский список всех свойств, которые вы планируете добавить в соединение, а также их атрибуты, метки и псевдонимы. Перед добавлением элементов в соединение вы должны зарегистрировать схему.

## <a name="methods"></a>Методы

| Метод                                                    | Возвращаемый тип                   | Описание |
|:----------------------------------------------------------|:------------------------------|:--|
| [Создание схемы](../api/externalconnectors-externalconnection-post-schema.md) | Нет *или* [схемы](externalconnectors-schema.md) | Схема подключения для регистрации. |
| [Получение схемы](../api/externalconnectors-schema-get.md)                        | [schema](externalconnectors-schema.md)           | Чтение свойств объекта схемы. |

## <a name="properties"></a>Свойства

| Свойство   | Тип                               | Описание                |
|:-----------|:-----------------------------------|:---------------------------|
| baseType   | String                             | Необходимо указать значение `microsoft.graph.externalItem`. Обязательный. |
| properties | [коллекция](externalconnectors-property.md) свойств | Свойства, определенные для элементов в подключении. Минимальное число свойств — одно, максимальное — 128. |

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.externalConnectors.schema",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [
    {
      "name": "String",
      "type": "String"
    }
  ]
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
