---
author: daspek
ms.author: dspektor
title: Тип ресурса shareAction
description: Объект shareAction предоставляет сведения о том, к которому был предоставлен общий доступ к элементу в действии Share.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a61ec47aae94eb99c2a192c863127d18a80fc087
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970792"
---
# <a name="shareaction-resource-type"></a>Тип ресурса shareAction

Ресурс **shareAction** предоставляет сведения о [действии] [ activity] , в котором общий доступ к элементу.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[activity]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип                       | Описание
|:--------------|:---------------------------|:-----------------------------
| recipients    | Коллекция [identitySet][] | Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.

[identitySet]: identityset.md

## <a name="json-representation"></a>Представление JSON

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

<!--
{
  "type": "#page.annotation",
  "description": "The shareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/shareAction",
  "suppressions": []
}
-->
