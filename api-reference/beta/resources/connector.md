---
title: Тип ресурса connector
description: Представляет соединители прокси приложения.
author: japere
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 53a5726456ce3d03ea537e87ec0dddb901623601
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136781"
---
# <a name="connector-resource-type"></a>Тип ресурса connector

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Соединители — это облегченные агенты, которые находятся локально и облегчают исходящие подключения к службе прокси приложения [Azure AD.](https://aka.ms/whyappproxy) Каждый соединители являются частью [connectorGroup.](connectorgroup.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление соединителей](../api/connector-list.md) | [коллекция соединители](connector.md) | Получить список объектов соединители. | 
| [Получение соединителя](../api/connector-get.md) | [connector](connector.md) | Чтение свойств и связей объекта соединители. |
| [Перечисление memberOf](../api/connector-list-memberof.md) | [Коллекция connectorGroup](connectorgroup.md) | Укажете коллекцию объектов connectorGroup, участником группы. |
| [Добавление соединителя для connectorGroup](../api/connector-post-memberof.md)| [connectorGroup](connectorgroup.md) | Добавление соединителю в connectorGroup. |


## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|externalIp|Строка| Внешний IP-адрес, обнаруженный сервером соединители. Только для чтения. |
|id|Строка| Уникальный идентификатор соединители. Только для чтения. |
|machineName|Строка| Имя компьютера, на который установлен и запущен соедините. |
|status|string| Указывает состояние соединители. Возможные значения: `active`, `inactive`. Только для чтения. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|memberOf|[Коллекция connectorGroup](connectorgroup.md)| СоединителиГруппы, в которые входит соединитестройка. Только для чтения. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connector"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



