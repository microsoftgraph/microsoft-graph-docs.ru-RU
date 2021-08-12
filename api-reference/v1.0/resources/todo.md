---
title: тип ресурса todo
description: Представляет службы To Do, доступные пользователю.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 89bbdd1bd3d91c5114850ffad8afc3aeec90e8bf3bbfb0b65e540444c2022b7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235263"
---
# <a name="todo-resource-type"></a>тип ресурса todo

Пространство имен: microsoft.graph

Представляет службы To Do, доступные пользователю.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление списков](../api/todo-list-lists.md) | Коллекция [todoTaskList](todotasklist.md) | Получение всех списков задач в почтовом ящике пользователя. |
|[Создание todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Создание списка задач To Do в почтовом ящике пользователя. |

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|lists|Коллекция [todoTaskList](../resources/todotasklist.md)| Списки задач в почтовом ящике пользователей. |

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



