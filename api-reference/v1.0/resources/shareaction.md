---
author: daspek
ms.author: dspektor
title: Тип ресурса shareAction
description: Объект shareAction предоставляет сведения о том, к которому был предоставлен общий доступ к элементу в действии Share.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 90d1d05a16130109dcef200938640e88e63e393a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009207"
---
# <a name="shareaction-resource-type"></a>Тип ресурса shareAction

Пространство имен: microsoft.graph

Ресурс **shareAction** предоставляет сведения о [действии][activity] , в котором общий доступ к элементу.

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

