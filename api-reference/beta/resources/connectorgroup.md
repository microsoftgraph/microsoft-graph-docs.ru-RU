---
title: Тип ресурса connectorGroup
description: Ниже представлено описание ресурса в формате JSON.
ms.openlocfilehash: a3131b887216f1f400f70ed8d607477f65793cc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079875"
---
# <a name="connectorgroup-resource-type"></a>Тип ресурса connectorGroup

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |Чтение свойства и связи объекта connectorGroup.|
|[Создание приложения](../api/connectorgroup-post-applications.md) |[application](application.md)| Свяжите приложение с группой соединителя с учета в коллекцию приложений.|
|[Список приложений](../api/connectorgroup-list-applications.md) |коллекции [приложения](application.md)| Получение коллекции объектов связанного приложения.|
|[Создание соединителя](../api/connectorgroup-post-members.md) |[Соединитель](connector.md)| Добавьте соединитель для соединителя группы, отправку сообщений в коллекцию элементов.|
|[Список членов](../api/connectorgroup-list-members.md) |Коллекция [соединителей](connector.md)| Получите соединитель коллекции объектов.|
|[Update](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)    |Обновление объекта connectorGroup. |
|[Delete](../api/connectorgroup-delete.md) | Нет |Удалите объект connectorGroup. Все соединители должны быть Удаление соединителя группы могут быть удалены. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|connectorGroupType|string| Тип соединителей, которые будут использоваться с этой группой. Возможные значения: `applicationProxy`.|
|id|String| Идентификатор объекта connectorGroup|
|isDefault|Логический| Указывает, является ли connectorGroup соединителя группы по умолчанию. Только один соединитель группы могут быть connectorGroup по умолчанию и устанавливается системой.|
|name|String| Имя, связанное с connectorGroup.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Description|
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
<!-- {
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
