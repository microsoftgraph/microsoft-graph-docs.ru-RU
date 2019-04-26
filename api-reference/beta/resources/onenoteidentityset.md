---
title: Тип ресурса Оненотеидентитисет
description: '**Поддержка скоро**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 49aadd4609e214937e02dd21238110addb9ed2ea
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341808"
---
# <a name="onenoteidentityset-resource-type"></a>Тип ресурса Оненотеидентитисет

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Поддержка скоро**

Тип Оненотеидентитисет является коллекцией с ключами объектов [оненотеидентити](onenoteidentity.md) .
Он используется для представления набора удостоверений, связанных с различными событиями для _записНой книжки_, _раздела_ или _страницы_, например _созданных автором_ или автором _последнего изменения_. 
 
В настоящее время он содержит один ключ, _**User**_.  В дальнейшем можно добавить такие ключи, как устройство или приложение для изменения элемента.

В дальнейшем этот тип будет объединен с [Identity](identityset.md)

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.onenoteIdentity"}
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|user|[Оненотеидентити](onenoteidentity.md)|Ресурс Оненотеидентити, представляющий пользователя.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
