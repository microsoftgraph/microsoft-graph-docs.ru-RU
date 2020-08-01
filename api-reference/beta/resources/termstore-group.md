---
author: mohitpcad
title: Тип ресурса Group
doc_type: resourcePageType
description: Представляет группу, используемую в банке терминов.
localization_priority: Normal
ms.prod: Sharepoint
ms.openlocfilehash: 91ad02722bcbddb1d21222381ced7cabc531f3fc
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539391"
---
# <a name="group-resource-type"></a>Тип ресурса Group

Пространство имен: Microsoft. Graph. банка

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Представляет группу, используемую в [банке](../resources/termstore-store.md)терминов. Группа — это логическая иерархия, содержащая коллекцию наборов. 

Наследуется от [объекта Entity](../resources/entity.md).


## <a name="methods"></a>Методы

| Метод                                                   | Тип возвращаемых данных       |    Описание
|:---------------------------------------------------------|:------------------|:---------------------
| [Создание группы](../api/termstore-group-post.md)                     | [Microsoft. Graph. Банк.] | Создайте группу в [банке]терминов.
| [Получение группы](../api/termstore-store-get-group.md)                           | [Microsoft. Graph. Банк.] | Получение данных группы в [банке]терминов.
| [Удаление группы](../api/termstore-group-delete.md)                     | Нет |  Удаление группы в [банке]терминов.

## <a name="properties"></a>Свойства

| Свойство             | Тип               | Описание
|:---------------------|:-------------------|:------------------------------------
| createdDateTime      | DateTimeOffset     | Дата и время создания группы. Только для чтения.
| description          | string             | Описание, содержащее сведения об использовании терминов.
| id                   | строка             | Уникальный идентификатор группы. Только для чтения.
| displayName          | string             | Имя группы.
| scope                | string              | Возвращает тип группы. Возможные значения: "Global", "System" и "siteCollection".

## <a name="relationships"></a>Связи
| Связь       | Тип                        | Описание
|:-------------------|:----------------------------|:--------------------------
| предваритель           | Коллекция [Microsoft. Graph. Банк. Set для Microsoft. Graph.][] | Все наборы в группе в [банке]терминов.

## <a name="json-representation"></a>Представление JSON

Ниже представлено представление ресурса **Group** в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.group",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
```json
{
  "@odata.type": "#microsoft.graph.termStore.group",
  "id": "string",
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "scope" : "microsoft.graph.termStore.groupScope",
  "displayName": "string",  
}
```



[identitySet]: identitySet.md
[Microsoft. Graph. банка. Set]: termstore-set.md
[Microsoft. Graph. Банк.]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
[восстановлен]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
<!--
{
  "type": "#page.annotation",
  "description": "TermGroup is the entity used for managing permissions for the termSets in termStore",
  "keywords": "termGroup,facet,resource",
  "section": "documentation",
  "tocPath": "TermGroup",
  "tocBookmarks": {
    "Resources/termStore.group": "#"
  },
  "suppressions": []
}
-->
