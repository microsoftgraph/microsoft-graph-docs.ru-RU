---
title: Тип соединителя ресурсов
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 98fa998a37b01ad64e556b229912932f4d1cfc75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884625"
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
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|externalIp|Строка|Внешний IP-адрес как вредоносным службой для этого соединителя компьютера. Только для чтения|
|id|Строка| Идентификатор объекта соединитель. <BR>Только для чтения.|
|имя_компьютера|Строка| Имя компьютера, на котором работает соединитель. <BR>Только для чтения|
|status|string| Указывает состояние соединителя. Возможные значения: `active`, `inactive`. Только для чтения |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
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
