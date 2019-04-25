---
title: Тип ресурса Connector
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: eed936c808e920f35a741a836a1fab64b2754bf8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535539"
---
# <a name="connector-resource-type"></a>Тип ресурса Connector

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение соединителя](../api/connector-get.md) | [PDIF](connector.md) |Чтение свойств и связей объекта Connector.|
|[Список memberOf](../api/connector-list-memberof.md) |Коллекция [коннекторграуп](connectorgroup.md)| Получение объекта Коннекторграуп, связанного с соединителем.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Екстерналип|String|Внешний IP-адрес, обнаруженный службой для соединителного компьютера. Только для чтения|
|id|Строка| Идентификатор объекта Connector. <BR>Только для чтения.|
|ИмяКомпьютера|String| Имя компьютера, на котором работает соединитель. <BR>Только для чтения|
|status|string| Указывает состояние соединителя. Возможные значения: `active`, `inactive`. Только для чтения |

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|memberOf|Коллекция [коннекторграуп](connectorgroup.md)| Коннекторграуп, участником которого является подключение.<br>Только для чтения. |

## <a name="json-representation"></a>Представление в формате JSON

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
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connector.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
