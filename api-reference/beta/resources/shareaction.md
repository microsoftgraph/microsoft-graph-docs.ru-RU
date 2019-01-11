---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
ms.openlocfilehash: 16bc590fcfe14f9ce7f6f1bbe38492225cce099c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828660"
---
# <a name="shareaction-resource-type"></a>Тип ресурса ShareAction

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **ShareAction** содержит сведения о [действии][activity], в результате выполнения которого был предоставлен общий доступ к элементу.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип                       | Описание
|:--------------|:---------------------------|:-----------------------------
| recipients    | Коллекция [identitySet][] | Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.

[identitySet]: identityset.md

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!-- {
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction"
} -->
