---
title: Тип ресурса outlookCategory
description: Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события. В Outlook пользователь определяет категории в главном списке и может применить одну или несколько из этих определяемых пользователем категорий.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f88c5df573e52e852311f71eb08781cd8061d503
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820926"
---
# <a name="outlookcategory-resource-type"></a>Тип ресурса outlookCategory

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события. В Outlook пользователь определяет категории в главном списке и может применить к элементу одну или несколько из этих пользовательских категорий. 

С помощью REST API вы можете [создавать](../api/outlookuser-post-mastercategories.md) и определять категории в основном списке категорий для пользователя. Вы также можете [получить этот основной список категорий](../api/outlookuser-list-mastercategories.md), [получить определенную категорию](../api/outlookcategory-get.md), [изменить](../api/outlookcategory-update.md) цвет, связанный с категорией, или [удалить](../api/outlookcategory-delete.md) категорию. Вы можете применить категорию к списку, добавив значение свойства **displayName** категории в коллекцию **categories** элемента.
К ресурсам, которые могут быть назначены категории, относятся [контакт](contact.md), [событие](event.md), [сообщение](message.md), [outlookTask](outlooktask.md), [post](post.md) и [todoTask](todotask.md).   

Каждой категории назначается 2 свойства: **displayName** и **color**. Значение **displayName** должно быть уникальным в основном списке пользователя. Однако значение свойства **color** может не быть уникальным. Несколько категорий в основном списке можно сопоставить с одним цветом. Вы можете сопоставить до 25 различных цветов с категориями в основном списке пользователя.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Уникальное имя, обозначающее категорию в почтовом ящике пользователя. После создания категории изменить имя невозможно. Только для чтения.|
|color|String|Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов. См. примечание ниже. |

> **Примечание**. Допустимые значения свойства **color** — предустановленные константы, например `None`, `preset0` и `preset1`. Каждая предустановленная константа сопоставлена с цветом. Фактический цвет зависит от клиента Outlook, в котором отображаются категории. В приведенной ниже таблице показаны цвета, сопоставленные с каждой предустановленной константой для классического клиента Outlook. 


| Предустановленная константа  | Соответствующий цвет в Outlook |
|:---------------|:--------|
| None | Цвет не задан |
| Preset0 | Красный |
| Preset1 | Оранжевый |
| Preset2 | Коричневый |
| Preset3 | Желтый |
| Preset4 | Зеленый |
| Preset5 | Сине-зеленый |
| Preset6 | Оливковый |
| Preset7 | Синий |
| Preset8 | Сиреневый |
| Preset9 | Клюквенный |
| Preset10 | Стальной |
| Preset11 | Темно-стальной |
| Preset12 | Серый |
| Preset13 | Темно-серый |
| Preset14 | Черный |
| Preset15 | Темно-красный |
| Preset16 | Темно-оранжевый |
| Preset17 | Темно-коричневый |
| Preset18 | Темно-желтый |
| Preset19 | Темно-зеленый |
| Preset20 | Темно-бирюзовый |
| Preset21 | Темно-оливковый |
| Preset22 | Темно-синий |
| Preset23 | Темно-фиолетовый |
| Preset24 | Темно-клюквенный |

## <a name="json-representation"></a>Представление JSON
Ниже показано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление категорий](../api/outlookuser-list-mastercategories.md) | Коллекция [outlookCategory](../resources/outlookcategory.md) |Получение всех категорий, определенных для пользователя.|
|[Получение категории](../api/outlookcategory-get.md) | [outlookCategory](../resources/outlookcategory.md) |Получение свойств и отношений указанного объекта **outlookCategory**.|
|[Создание](../api/outlookuser-post-mastercategories.md) | [outlookCategory](../resources/outlookcategory.md) |Создание объекта **outlookCategory** в основном списке категорий пользователя.|
|[Обновление](../api/outlookcategory-update.md) | [outlookCategory](../resources/outlookcategory.md) |Обновление перезаписываемого свойства **color** указанного объекта **outlookCategory**. |
|[Delete](../api/outlookcategory-delete.md) | Нет |Удаление указанного объекта **outlookCategory**. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
 


