---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (Коллекция объектов outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c9f9958750cca1aaa40ba9394832e5974bed8cc3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998364"
---
# <a name="outlooktaskfolder-resource-type-deprecated"></a>Тип ресурса outlookTaskFolder (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


Папка, содержащая задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ). 

В Outlook группа задач по умолчанию, `My Tasks` которая содержит папку задач по умолчанию, `Tasks` для почтового ящика пользователя. Вы не можете переименовывать или удалять эти группы задач и папки по умолчанию, но вы можете создавать дополнительные группы задач и папки задач.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение outlookTaskFolder](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |Получение свойств и связей указанной папки задач Outlook.|
|[Создание объекта outlookTask](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| Создание задачи Outlook в указанной папке задач.|
|[Список задач](../api/outlooktaskfolder-list-tasks.md) |Коллекция объектов [outlookTask](outlooktask.md)| Получение всех задач Outlook в указанной папке.|
|[обновление](../api/outlooktaskfolder-update.md). | [outlookTaskFolder](outlooktaskfolder.md)   |Обновление свойств, доступных для записи, папки задач Outlook. |
|[удаление](../api/outlooktaskfolder-delete.md); | Нет |Удаление указанной папки задач Outlook.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |Создайте одно или несколько расширенных свойств с одним значением в новой или существующей папке задач Outlook.   |
|[Получение папки задач с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Получение папок задач Outlook, которые содержат расширенное свойство с одним значением, с помощью `$expand` или `$filter` . |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | Создайте одно или несколько расширенных свойств с несколькими значениями в новой или существующей папке задач Outlook.  |
|[Получение папки задач с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Получение папки задач Outlook, которая содержит расширенное свойство с несколькими значениями, с помощью `$expand` . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|changeKey|String|Версия папки задач.|
|id|String|Идентификатор папки задач, уникальный в почтовом ящике пользователя. Только для чтения.|
|исдефаултфолдер|Boolean|Значение true, если папка является папкой задач по умолчанию.|
|name|String|Имя папки задач.|
|парентграупкэй|Guid|Уникальный идентификатор GUID родительской группы папок задач.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)|Коллекция расширенных свойств с несколькими значениями, определенных для папки задач. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)|Коллекция расширенных свойств с одним значением, определенных для папки задач. Только для чтения. Допускается значение null.|
|tasks|Коллекция объектов [outlookTask](outlooktask.md)|Задачи в этой папке задач. Только для чтения. Допускается значение null.|

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


