---
title: тип ресурса соединитетеля
description: Представляет соединители прокси-сервер приложений.
author: japere
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: d88d7468872fb4e0e6b8d6ae5dd84346ba7de36a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136689"
---
# <a name="connector-resource-type"></a>тип ресурса соединитетеля

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Соединители — это легкие агенты, которые находятся на месте и облегчают исходящие подключения к прокси-службе [приложения Azure AD.](/azure/active-directory/app-proxy/what-is-application-proxy) Каждый соединитектор является частью [соединителиГруп](connectorgroup.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление соединителей](../api/connector-list.md) | [коллекция соединители](connector.md) | Извлечение списка объектов соединители. | 
| [Получение соединителя](../api/connector-get.md) | [connector](connector.md) | Чтение свойств и связей соединитеного объекта. |
| [Список memberOf](../api/connector-list-memberof.md) | [коллекция connectorGroup](connectorgroup.md) | Укажете коллекцию объектов connectorGroup, членом в которая является соедините. |
| [Добавление соединителя для connectorGroup](../api/connector-post-memberof.md)| [connectorGroup](connectorgroup.md) | Добавьте соединителю в соединителюGroup. |


## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|externalIp|Строка| Внешний IP-адрес, обнаруженный сервером соединители. Только для чтения. |
|id|Строка| Уникальный идентификатор соединитетеля. Только для чтения. |
|machineName|Строка| Имя машины, на которое установлен соединитатель, и запущено. |
|status|connectorStatus| Указывает состояние соединитетеля. Возможные значения: `active`, `inactive`. Только для чтения. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|memberOf|[коллекция connectorGroup](connectorgroup.md)| СоединитекторGroup, членом который является соединитектор. Только для чтения. |

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