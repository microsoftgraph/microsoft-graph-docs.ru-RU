---
title: Тип ресурса todo
description: Представляет службы дел, доступные пользователю.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 99b2936cf84c5cfdc25a39ff6f0e35518658d0ff
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850048"
---
# <a name="todo-resource-type"></a>Тип ресурса todo

Пространство имен: microsoft.graph

Представляет службы дел, доступные пользователю.

Наследуется от [объекта.](../resources/entity.md)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Списки](../api/todo-list-lists.md) | [Коллекция todoTaskList](todotasklist.md) | Получение всех списков задач в почтовом ящике пользователя. |
|[Создание объекта todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Создание списка задач в почтовом ящике пользователя. |

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|lists|[Коллекция todoTaskList](../resources/todotasklist.md)| Списки задач в почтовом ящике пользователей. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todo",
  "id": "String"
}
```

