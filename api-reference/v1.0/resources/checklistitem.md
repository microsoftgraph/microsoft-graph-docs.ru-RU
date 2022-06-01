---
title: Тип ресурса checklistItem
description: Представляет коллекцию элементов контрольного списка для задачи
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0c60add74b11b245c1fdf732ae1458fd2ed07bf0
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821326"
---
# <a name="checklistitem-resource-type"></a>Тип ресурса checklistItem

Пространство имен: microsoft.graph

Представляет подзадачу в [todoTask большего размера](./todotask.md). **ChecklistItem** позволяет разбить сложную задачу на более интерактивные и небольшие задачи. 

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление контрольных элементов](../api/todotask-list-checklistitems.md)|[Коллекция checklistItem](../resources/checklistitem.md)|Получение списка объектов [checklistItem](../resources/checklistitem.md) и их свойств.|
|[Создание checklistItem](../api/todotask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Создайте объект [checklistItem](../resources/checklistitem.md) .|
|[Получение checklistItem](../api/checklistitem-get.md)|[checklistItem](../resources/checklistitem.md)|Чтение свойств и связей объекта [checklistItem](../resources/checklistitem.md) .|
|[Обновление checklistItem](../api/checklistitem-update.md)|[checklistItem](../resources/checklistitem.md)|Обновление свойств объекта [checklistItem](../resources/checklistitem.md) .|
|[Удаление checklistItem](../api/checklistitem-delete.md)|Нет|Удаляет объект [checklistItem](../resources/checklistitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|checkedDateTime|DateTimeOffset|Дата и время завершения **checklistItem** .|
|createdDateTime|DateTimeOffset|Дата и время создания **объекта checklistItem** .|
|displayName|Строка|Поле, указывающее **заголовок checklistItem**.|
|id|Строка|Идентификатор, созданный сервером для **checkListItem**|
|Ischecked|Логическое|Состояние, указывающее, был ли элемент извлечен или нет.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.checklistItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.checklistItem",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "checkedDateTime": "String (timestamp)",
  "isChecked": "Boolean",
  "id": "String (identifier)"
}
```

