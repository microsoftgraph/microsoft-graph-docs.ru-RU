---
title: тип ресурса baseTaskList
description: Содержит один или несколько ресурсов задач.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7a0774bf6d51eba2bc55f67c58c2d7de5a0c3312
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61425135"
---
# <a name="basetasklist-resource-type"></a>тип ресурса baseTaskList

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит один или [несколько ресурсов задач.](./basetask.md)

Это базовый ресурс для следующих производных типов списков задач.
* Встроенный список задач[(ресурс wellKnownTaskList)](../resources/wellknowntasklist.md)
* Созданный пользователем список задач[(ресурс taskList)](../resources/tasklist.md) 

Это абстрактный тип.

## <a name="methods"></a>Методы
Следующий метод применяется к любому из производных типов **baseTaskList** **(wellKnownTaskList**,**taskList**)

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список baseTaskLists](../api/tasks-list-lists.md)|[коллекция baseTaskList](../resources/basetasklist.md)|Получите список объектов [baseTaskList](../resources/basetasklist.md) и их свойств.|
|[Get baseTaskList](../api/basetasklist-get.md)|[baseTaskList](../resources/basetasklist.md)|Ознакомьтесь с свойствами и отношениями объекта [baseTaskList.](../resources/basetasklist.md)|
|[Перечисление задач](../api/basetasklist-list-tasks.md)|[коллекция baseTask](../resources/basetask.md)|Получите ресурсы baseTask из свойства навигации задач.|
|[Создание baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Создайте новый объект baseTask.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя списка задач.|
|id|Строка|Идентификатор списка задач, уникальный в почтовом ящике пользователя. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|extensions|Коллекция [extension](../resources/extension.md)|Коллекция открытых расширений, определенных для списка задач. Допускается значение null.|
|tasks|[коллекция baseTask](../resources/basetask.md)|Задачи в этом списке задач. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseTaskList",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.baseTaskList",
  "displayName": "String",
  "id": "String (identifier)"
}
```

