---
title: Тип ресурса outlookCategory
description: Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события. Пользователь определяет категории в основном списке и может применять один или несколько пользовательских
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: da65d6f2445a037ae4fcbbc8aaf05906bc0ae5c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534115"
---
# <a name="outlookcategory-resource-type"></a>Тип ресурса outlookCategory

Пространство имен: microsoft.graph


Представляет категорию, по которой пользователь может группировать такие элементы Outlook, как сообщения и события. Пользователь определяет категории в основном списке и может применить одну или несколько из них к элементу. 

С помощью REST API вы можете [создавать](../api/outlookuser-post-mastercategories.md) и определять категории в основном списке категорий для пользователя. Вы также можете [получить этот основной список категорий](../api/outlookuser-list-mastercategories.md), [получить определенную категорию](../api/outlookcategory-get.md), [изменить](../api/outlookcategory-update.md) цвет, связанный с категорией, или [удалить](../api/outlookcategory-delete.md) категорию. Вы можете применить категорию к списку, добавив значение свойства **displayName** категории в коллекцию **categories** элемента.
К ресурсам, которым можно назначать категории, относятся [contact](contact.md), [event](event.md), [message](message.md) и [post](post.md).   

Каждой категории назначается 2 свойства: **displayName** и **color**. Значение **displayName** должно быть уникальным в основном списке пользователя. Однако значение свойства **color** может не быть уникальным. Несколько категорий в основном списке можно сопоставить с одним цветом. Вы можете сопоставить до 25 различных цветов с категориями в основном списке пользователя.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Уникальное имя, обозначающее категорию в почтовом ящике пользователя. После создания категории изменить имя невозможно. Только для чтения.|
|color|категориколор|Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов. См. примечание ниже. |

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
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
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
|[Удаление](../api/outlookcategory-delete.md) | Нет |Удаление указанного объекта **outlookCategory**. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/resources/outlookcategory.md:
      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ],
  "tocPath": ""
}-->
 
