---
title: Тип ресурса Connector
description: Представляет соединитель прокси приложения.
author: japere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 864d76d7e6a7cb3724a91a753e5c5198e274780a
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556179"
---
# <a name="connector-resource-type"></a>Тип ресурса Connector

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Соединители это простые агенты, которые размещаются локально и упрощают исходящее подключение к службе [прокси приложения Azure AD](https://aka.ms/whyappproxy) . Каждый соединитель является частью [коннекторграуп](connectorgroup.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список соединителей](../api/connector-list.md) | Коллекция [соединителей](connector.md) | Получение списка объектов Connector. | 
| [Получение соединителя](../api/connector-get.md) | [PDIF](connector.md) | Чтение свойств и связей объекта Connector. |
| [Перечисление memberOf](../api/connector-list-memberof.md) | Коллекция [коннекторграуп](connectorgroup.md) | Список коллекций объектов Коннекторграуп, участником которых является соединитель. |
| [Добавление соединителя в Коннекторграуп](../api/connector-post-memberof.md)| [connectorGroup](connectorgroup.md) | Добавление соединителя в Коннекторграуп. |


## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|екстерналип|String| Внешний IP-адрес, обнаруженный сервером соединителей. Только для чтения. |
|id|Строка| Уникальный идентификатор соединителя. Только для чтения. |
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
