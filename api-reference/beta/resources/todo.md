---
title: Тип ресурса TODO
description: Представляет службы To Do, доступные пользователю.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: aa468c6d6556ad70d3650e40fb3fd01c46ccdb35
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971477"
---
# <a name="todo-resource-type"></a>Тип ресурса TODO

Пространство имен: microsoft.graph

Представляет службы To Do, доступные пользователю.

Наследуется от [объекта Entity](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление списков](../api/todo-list-lists.md) | Коллекция [todoTaskList](todotasklist.md) | Получение всех списков задач в почтовом ящике пользователя. |
|[Создание Тодотасклист](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Создание списка задач To Do в почтовом ящике пользователя. |

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|lists|Коллекция [todoTaskList](../resources/todotasklist.md)| Списки задач в почтовом ящике пользователя. |

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



