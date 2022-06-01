---
title: Тип ресурса baseTaskList
description: Содержит один или несколько ресурсов задачи.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9d2ead693e4879f6edf030fb8921c94bdf1d0ea0
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820219"
---
# <a name="basetasklist-resource-type-deprecated"></a>Тип ресурса baseTaskList (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

Содержит один или несколько [ресурсов baseTask](./basetask.md) .

Это базовый ресурс для следующих производных типов списков задач.
* Встроенный список задач ([ресурс wellKnownTaskList](../resources/wellknowntasklist.md) )
* Список задач, созданный пользователем ([ресурс taskList](../resources/tasklist.md) ) 

Это абстрактный тип.

## <a name="methods"></a>Методы
Следующий метод применяется к любому производному типу **baseTaskList** (**wellKnownTaskList,taskList**).

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление элементов baseTaskList](../api/tasks-list-lists.md)|[Коллекция baseTaskList](../resources/basetasklist.md)|Получение списка объектов [baseTaskList](../resources/basetasklist.md) и их свойств.|
|[Получение baseTaskList](../api/basetasklist-get.md)|[baseTaskList](../resources/basetasklist.md)|Чтение свойств и связей объекта [baseTaskList](../resources/basetasklist.md) .|
|[Перечисление задач](../api/basetasklist-list-tasks.md)|[Коллекция baseTask](../resources/basetask.md)|Получите ресурсы baseTask из свойства навигации задач.|
|[Создание baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Создайте объект baseTask.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя списка задач.|
|id|Строка|Идентификатор списка задач, уникальный в почтовом ящике пользователя. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|extensions|Коллекция объектов [extension](../resources/extension.md)|Коллекция открытых расширений, определенных для списка задач. Допускается значение null.|
|tasks|[Коллекция baseTask](../resources/basetask.md)|Задачи в этом списке задач. Только для чтения. Допускается значение null.|

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

