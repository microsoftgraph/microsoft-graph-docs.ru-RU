---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (коллекция объектов outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f950028bef8bcdcdcd8252ca16348c235ef31d3f
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849793"
---
# <a name="outlooktaskfolder-resource-type"></a>Тип ресурса outlookTaskFolder

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


Папка, содержащая задачи Outlook [(коллекция объектов outlookTask).](outlooktask.md) 

В Outlook группа задач по умолчанию `My Tasks` содержит папку задач по умолчанию, `Tasks` для почтового ящика пользователя. Эти группы и папки задач по умолчанию не переименовывать или удалять невозможно, но можно создать дополнительные группы задач и папки задач.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get outlookTaskFolder](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |Получение свойств и связей указанной папки задач Outlook.|
|[Создание объекта outlookTask](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| Создание задачи Outlook в указанной папке задач.|
|[Список задач](../api/outlooktaskfolder-list-tasks.md) |Коллекция объектов [outlookTask](outlooktask.md)| Получение всех задач Outlook в указанной папке.|
|[обновление](../api/outlooktaskfolder-update.md). | [outlookTaskFolder](outlooktaskfolder.md)   |Обновление записываемых свойств папки задач Outlook. |
|[удаление](../api/outlooktaskfolder-delete.md); | Нет |Удаление указанной папки задач Outlook.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |Создание одного или нескольких расширенных свойств с одним значением в новой или существующей папке задач Outlook.   |
|[Получение папки задачстов с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Получение папок задач Outlook, которые содержат расширенное свойство с одним значением, `$expand` используя `$filter` или. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новой или существующей папке задач Outlook.  |
|[Получение папки задач с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Получение папки задач Outlook, которая содержит расширенное свойство с несколькими значениями, с `$expand` помощью. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|changeKey|String|Версия папки задач.|
|id|String|Идентификатор папки задач, уникальный в почтовом ящике пользователя. Только для чтения.|
|isDefaultFolder|Boolean|True, если папка является папкой задач по умолчанию.|
|name|String|Имя папки задач.|
|parentGroupKey|Guid|Уникальный идентификатор GUID родительской группы папки задачи.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)|Коллекция расширенных свойств с несколькими значениями, определенных для папки задач. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)|Коллекция расширенных свойств с одним значением, определенных для папки задач. Только для чтения. Допускается значение null.|
|tasks|Коллекция объектов [outlookTask](outlooktask.md)|Задачи из этой папки задач. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
