---
title: тип ресурса checklistItem
description: Представляет коллекцию элементов контрольного списка для задачи
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 01cca362ac85b10cb4bf141908d2b5dac309c9cd
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61425153"
---
# <a name="checklistitem-resource-type"></a>тип ресурса checklistItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию элементов контрольного списка для задачи. **ChecklistItem помогает** разделить сложные задачи на более мелкие действия.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Контрольные списки спискаItems](../api/basetask-list-checklistitems.md)|[коллекция checklistItem](../resources/checklistitem.md)|Получите список объектов [checklistItem](../resources/checklistitem.md) и их свойств.|
|[Создание контрольного спискаItem](../api/basetask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Создайте [новый объект checklistItem.](../resources/checklistitem.md)|
|[Get checklistItem](../api/checklistitem-get.md)|[checklistItem](../resources/checklistitem.md)|Ознакомьтесь с свойствами и отношениями [объекта checklistItem.](../resources/checklistitem.md)|
|[Обновление контрольного спискаItem](../api/checklistitem-update.md)|[checklistItem](../resources/checklistitem.md)|Обновление свойств объекта [checklistItem.](../resources/checklistitem.md)|
|[Удаление контрольного спискаItem](../api/checklistitem-delete.md)|Нет|Удаляет объект [checklistItem.](../resources/checklistitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|checkedDateTime|DateTimeOffset|Дата и время завершения **контрольного спискаItem.**|
|createdDateTime|DateTimeOffset|Дата и время создания **контрольного спискаItem.**|
|displayName|Строка|Поле, указывающее название **checklistItem**.|
|id|Строка|Созданный сервером ID для **checkListItem**|
|isChecked|Boolean|Состояние, указывающее, отключается элемент или нет.|

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

