---
author: daspek
title: тип ресурса shareAction
description: Объект shareAction предоставляет сведения о том, кому элемент был общим в действии общего обмена.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b9d252df884e90d7351edb9544a354d88fbc78baebcc5926686b016c38e58f37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251780"
---
# <a name="shareaction-resource-type"></a>тип ресурса shareAction

Пространство имен: microsoft.graph

Ресурс **shareAction** предоставляет сведения о [действии, которое][activity] разделяет элемент.

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
  "@type&quot;: &quot;microsoft.graph.shareAction"
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

