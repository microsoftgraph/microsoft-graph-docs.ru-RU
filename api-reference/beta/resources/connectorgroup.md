---
title: Тип ресурса connectorGroup
description: Ниже показано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517500"
---
# <a name="connectorgroup-resource-type"></a>Тип ресурса connectorGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |Чтение свойства и связи объекта connectorGroup.|
|[Создание приложения](../api/connectorgroup-post-applications.md) |[application](application.md)| Свяжите приложение с группой соединителя с учета в коллекцию приложений.|
|[Список приложений](../api/connectorgroup-list-applications.md) |коллекции [приложения](application.md)| Получение коллекции объектов связанного приложения.|
|[Создание соединителя](../api/connectorgroup-post-members.md) |[Connector](connector.md)| Добавьте соединитель для соединителя группы, отправку сообщений в коллекцию элементов.|
|[Перечисление участников](../api/connectorgroup-list-members.md) |Коллекция [соединителей](connector.md)| Получите соединитель коллекции объектов.|
|[Update](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)    |Обновление объекта connectorGroup. |
|[Delete](../api/connectorgroup-delete.md) | Нет |Удалите объект connectorGroup. Все соединители должны быть Удаление соединителя группы могут быть удалены. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|connectorGroupType|string| Тип соединителей, которые будут использоваться с этой группой. Возможные значения: `applicationProxy`.|
|id|String| Идентификатор объекта connectorGroup|
|isDefault|Boolean| Указывает, является ли connectorGroup соединителя группы по умолчанию. Только один соединитель группы могут быть connectorGroup по умолчанию и устанавливается системой.|
|name|String| Имя, связанное с connectorGroup.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|приложения|коллекции [приложения](application.md)| Только для чтения. Допускается значение null.|
|members|Коллекция [соединителей](connector.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connectorgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
