---
title: Тип ресурса connectorGroup
description: Представляет соединители соединители прокси приложения.
localization_priority: Normal
ms.prod: applications
author: japere
doc_type: resourcePageType
ms.openlocfilehash: 78716646f4bf5cbba7a66da4cdef88d94d1984aa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132327"
---
# <a name="connectorgroup-resource-type"></a>Тип ресурса connectorGroup

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Каждый [прокси-сервер приложения Azure AD](https://aka.ms/whyappproxy) всегда является частью группы соединители. Все соединители, принадлежащие одной группе соединитеителей, выступают в качестве отдельной единицы для высокой доступности и балансировки нагрузки. Если группы соединители не создаются, все соединители будут в нее в составе группы по умолчанию. При настройке приложения с помощью прокси приложения необходимо также указать группу соединители, которой необходимо назначить приложение.

После создания группы соединителю можно добавить или переместить соединители в группу соединителю с помощью [соединителю "Добавить".](../api/connectorgroup-post-members.md) Вы также можете использовать [приложение "Добавить",](../api/connectorgroup-post-applications.md) чтобы назначить приложение группе соединителю.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[List connectorGroup](../api/connectorgroup-list.md) |[Коллекция connectorGroup](connectorgroup.md) | Получить список объектов connectorGroup. |
|[Создание connectorGroup](../api/connectorgroup-post.md) |[Коллекция connectorGroup](connectorgroup.md) | Создание объекта connectorGroup. |
|[Получение connectorGroup](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) | Чтение свойств и связей объекта connectorGroup. |
|[Обновление connectorGroup](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)| Обновление объекта connectorGroup. |
|[Удаление connectorGroup](../api/connectorgroup-delete.md) | Нет | Удаление объекта connectorGroup. Перед удалением connectorGroup необходимо удалить все соединители из connectorGroup. |
|[Перечисление участников](../api/connectorgroup-list-members.md) |[коллекция соединители](connector.md)| Получите коллекцию объектов соединители. |
|[Перечисление приложений](../api/connectorgroup-list-applications.md) |Коллекция [application](application.md)| Получение коллекции объектов приложения, связанной с connectorGroup. |
|[Добавление приложения](../api/connectorgroup-post-applications.md) |[application](application.md)| Связывать приложение с connectorGroup путем публикации в коллекции приложений. |
|[Добавление соединителя](../api/connectorgroup-post-members.md) |[connector](connector.md)| Добавление соединителя в connectorGroup путем добавления в коллекцию connectorGroup. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|connectorGroupType|string| Указывает тип гибридного агента. Это предварительно заданной системой. Только для чтения. |
|id|string| Уникальный идентификатор для этого соединителаGroup. Только для чтения. |
|isDefault|boolean| Указывает, является ли connectorGroup соединитетелем по умолчанию. Только одна группа соединительных соединительных подключений может быть соединитеной группой по умолчанию, которая предварительно заданной системой. Только для чтения. |
|name|string| Имя, связанное с соединитетелемGroup. |
|region|string| Регион, для который назначен соединительГрупп и для который будет оптимизирована трафик. Этот регион можно установить только в **том** случае, если соединители или приложения не назначены соединительной группе. Доступны следующие регионы: Северная Америка, Европа, Австралия, Азия и Индия. Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|applications|Коллекция [application](application.md)| Только для чтения. Допускается значение null.|
|members|[коллекция соединители](connector.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String",
  "region": "string"
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
  "suppressions": []
}
-->



