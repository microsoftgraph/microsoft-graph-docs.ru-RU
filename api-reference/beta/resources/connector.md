---
title: Тип соединителя ресурсов
description: Ниже представлено описание ресурса в формате JSON.
ms.openlocfilehash: 6d4cb7e5ca1a5384dbb6c8be92e7ce4eb107388a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081266"
---
# <a name="connector-resource-type"></a>Тип соединителя ресурсов

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение соединителя](../api/connector-get.md) | [Соединитель](connector.md) |Чтение свойства и связи объекта соединителя.|
|[Перечисление memberOf](../api/connector-list-memberof.md) |[connectorGroup](connectorgroup.md) коллекции| Получите объект connectorGroup, связанный с соединителем.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|externalIp|String|Внешний IP-адрес как вредоносным службой для этого соединителя компьютера. Только для чтения|
|id|String| Идентификатор объекта соединитель. <BR>Только для чтения.|
|имя_компьютера|String| Имя компьютера, на котором работает соединитель. <BR>Только для чтения|
|status|string| Указывает состояние соединителя. Возможные значения: `active`, `inactive`. Только для чтения |

## <a name="relationships"></a>Связи
| Связь | Тип   |Description|
|:---------------|:--------|:----------|
|memberOf|[connectorGroup](connectorgroup.md) коллекции| ConnectorGroup, который является членом подключиться.<br>Только для чтения. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
