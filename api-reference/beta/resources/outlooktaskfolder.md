---
title: Тип ресурса outlookTaskFolder
description: 'Папка, содержащая задачи Outlook (Коллекция объектов outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eb61936b9ede67d35127db07c92ba8b7517fe623
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568621"
---
# <a name="outlooktaskfolder-resource-type"></a>Тип ресурса outlookTaskFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Папка, содержащая задачи Outlook (Коллекция объектов [outlookTask](outlooktask.md) ). 

В Outlook группа `My Tasks`задач по умолчанию, которая содержит папку `Tasks`задач по умолчанию, для почтового ящика пользователя. Вы не можете переименовывать или удалять эти группы задач и папки по умолчанию, но вы можете создавать дополнительные группы задач и папки задач.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение outlookTaskFolder](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |Получение свойств и связей указанной папки задач Outlook.|
|[Создание outlookTask](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| Создание задачи Outlook в указанной папке задач.|
|[Перечисление задач](../api/outlooktaskfolder-list-tasks.md) |Коллекция [outlookTask](outlooktask.md)| Получение всех задач Outlook в указанной папке.|
|[Обновление](../api/outlooktaskfolder-update.md) | [outlookTaskFolder](outlooktaskfolder.md)   |Обновление свойств, доступных для записи, папки задач Outlook. |
|[Удаление](../api/outlooktaskfolder-delete.md) | Нет |Удаление указанной папки задач Outlook.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |Создайте одно или несколько расширенных свойств с одним значением в новой или существующей папке задач Outlook.   |
|[Получение папки задач с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Получение папок задач Outlook, которые содержат расширенное свойство с одним значением, `$expand` с `$filter`помощью или. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | Создайте одно или несколько расширенных свойств с несколькими значениями в новой или существующей папке задач Outlook.  |
|[Получение папки задач с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Получение папки задач Outlook, которая содержит расширенное свойство с несколькими значениями, с `$expand`помощью. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|changeKey|String|Версия папки задач.|
|id|Строка|Идентификатор папки задач, уникальный в почтовом ящике пользователя. Только для чтения.|
|Исдефаултфолдер|Boolean|Значение true, если папка является папкой задач по умолчанию.|
|name|String|Имя папки задач.|
|Парентграупкэй|Guid|Уникальный идентификатор GUID родительской группы папок задач.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)|Коллекция расширенных свойств с несколькими значениями, определенных для папки задач. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)|Коллекция расширенных свойств с одним значением, определенных для папки задач. Только для чтения. Допускается значение null.|
|tasks|Коллекция [outlookTask](outlooktask.md)|Задачи в этой папке задач. Только для чтения. Допускается значение null.|

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
