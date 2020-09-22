---
title: Тип ресурса Connector
description: Представляет соединитель прокси приложения.
author: japere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e42bc42c1989e530f7b7f307da3963407ded112
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027169"
---
# <a name="connector-resource-type"></a>Тип ресурса Connector

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Соединители это простые агенты, которые размещаются локально и упрощают исходящее подключение к службе [прокси приложения Azure AD](https://aka.ms/whyappproxy) . Каждый соединитель является частью [коннекторграуп](connectorgroup.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление соединителей](../api/connector-list.md) | Коллекция [соединителей](connector.md) | Получение списка объектов Connector. | 
| [Получение соединителя](../api/connector-get.md) | [PDIF](connector.md) | Чтение свойств и связей объекта Connector. |
| [Перечисление memberOf](../api/connector-list-memberof.md) | Коллекция [коннекторграуп](connectorgroup.md) | Список коллекций объектов Коннекторграуп, участником которых является соединитель. |
| [Добавление соединителя для connectorGroup](../api/connector-post-memberof.md)| [connectorGroup](connectorgroup.md) | Добавление соединителя в Коннекторграуп. |


## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|екстерналип|String| Внешний IP-адрес, обнаруженный сервером соединителей. Только для чтения. |
|id|String| Уникальный идентификатор соединителя. Только для чтения. |
|ИмяКомпьютера|String| Имя компьютера, на котором установлен и запущен соединитель. |
|status|string| Указывает состояние соединителя. Возможные значения: `active`, `inactive`. Только для чтения. |

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|memberOf|Коллекция [коннекторграуп](connectorgroup.md)| Коннекторграуп, участником которого является соединитель. Только для чтения. |

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


