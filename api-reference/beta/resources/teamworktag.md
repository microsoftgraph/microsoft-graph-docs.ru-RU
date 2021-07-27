---
title: тип ресурса teamworkTag
description: Представляет тег, связанный с командой.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 677ddc348d1cd3ae152d7b777a6b29319839266c
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533901"
---
# <a name="teamworktag-resource-type"></a>тип ресурса teamworkTag

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тег, связанный с командой. 

Теги предоставляют пользователям гибкий способ классификации пользователей или групп на основе общего атрибута в команде. Например, тег Nurse, Manager или Designer позволит пользователям достигать групп людей в Teams без необходимости ввести каждое имя.

При добавлении тега пользователи могут @mention его в канале. Каждый, кому назначен этот тег, получит уведомление точно так же, как если бы он @mentioned по отдельности. Пользователи также могут использовать тег для запуска нового чата с участниками этого тега.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список teamworkTags](../api/teamworktag-list.md)|[**коллекция teamworkTag**](teamworktag.md)|Получите список объектов **teamworkTag** и их свойств.|
|[Создание командной работы](../api/teamworktag-post.md)|[**teamworkTag**](teamworktag.md)|Создание нового **объекта teamworkTag.**|
|[Командная работа](../api/teamworktag-get.md)|[**teamworkTag**](teamworktag.md)|Ознакомьтесь с свойствами и отношениями объекта **teamworkTag.**|
|[Обновление командной работы](../api/teamworktag-update.md)|[**teamworkTag**](teamworktag.md)|Обновление свойств объекта **teamworkTag.**|
|[Удаление командной работы](../api/teamworktag-delete.md)|Нет|Удаление **объекта teamworkTag.**|
|[Список командной работыTagMembers](../api/teamworktagmember-list.md)|[**коллекция teamworkTagMember**](teamworktagmember.md)|Получите список участников стандартного тега в команде и их свойства.|
|[Создание командной работыTagMember](../api/teamworktagmember-post.md)|[**teamworkTagMember**](teamworktagmember.md)|Создайте новый **объект teamworkTagMember.**|
|[Получить командную работуTagMember](../api/teamworktagmember-get.md)|[**teamworkTagMember**](teamworktagmember.md)|Получите свойства и отношения участника стандартного тега в команде.|
|[Удаление командной работыTagMember](../api/teamworktagmember-delete.md)|Нет|Удаление участника из стандартного тега в команде.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание тега, как оно будет отображаться пользователю в Microsoft Teams.|
|displayName|Строка|Тег имя, как это будет отображаться пользователю в Microsoft Teams.|
|id|Строка|ID тега.|
|memberCount|Int32|Количество пользователей, назначенных тегу.|
|tagType|teamworkTagType|Тип тега. По умолчанию это стандарт.|
|teamId|Строка|ID команды, в которой определен тег.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|members|[коллекция teamworkTagMember](../resources/teamworktagmember.md)|Пользователи, назначенные тегу.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkTag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "String (identifier)",
  "teamId": "String",
  "displayName": "String",
  "memberCount": "Integer",
  "tagType": "String"
}
```

