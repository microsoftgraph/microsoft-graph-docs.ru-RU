---
title: Тип ресурса схемы
description: Схема подключения определяет, как содержимое, добавленное в подключение, будет использоваться в различных Graph microsoft.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: cb3d89c9ab3903519376e4fdf0dd55dec8eba746
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266014"
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
| [Обновление схемы](../api/externalconnectors-schema-update.md) | Нет *или* [схемы](externalconnectors-schema.md) | Обновление свойств объекта схемы. |

## <a name="properties"></a>Свойства

| Свойство   | Тип                               | Описание                |
|:-----------|:-----------------------------------|:---------------------------|
| baseType   | Строка                             | Необходимо указать значение `microsoft.graph.externalItem`. Обязательный. |
| properties | [коллекция](externalconnectors-property.md) свойств | Свойства, определенные для элементов в подключении. Минимальное число свойств — одно, максимальное — 128. |

## <a name="relationships"></a>Связи

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
