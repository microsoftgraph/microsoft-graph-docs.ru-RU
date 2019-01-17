---
title: Тип ресурса oneNoteIdentitySet
description: '**Поддержка готовится к выпуску**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 9043b08a8586bcc9a0043a2fde13f0d5d9eea4a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947171"
---
# <a name="onenoteidentityset-resource-type"></a>Тип ресурса oneNoteIdentitySet

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

**Поддержка готовится к выпуску**

Тип OneNoteIdentitySet — с ключом коллекцию объектов [OneNoteIdentity](onenoteidentity.md) .
Он используется для представления набора удостоверения, связанные с различные события для _записной книжки_, _раздел_ или _страницы_, например, _созданные_ или _Кем изменено_. 
 
В настоящее время в нем ключей и одного _**пользователя**_.  В будущем могут быть добавлены разделы, такие как устройство или приложение для изменения элемента.

В будущем этого типа будут объединены с [IdentitySet](identityset.md)

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.oneNoteIdentity"}
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|user|[oneNoteIdentity](onenoteidentity.md)|Ресурс OneNoteIdentity, представляющий пользователя.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
