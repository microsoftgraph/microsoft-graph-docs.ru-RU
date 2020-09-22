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
# <a name="shareaction-resource-type"></a><span data-ttu-id="aabdb-103">Тип ресурса shareAction</span><span class="sxs-lookup"><span data-stu-id="aabdb-103">shareAction resource type</span></span>

<span data-ttu-id="aabdb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aabdb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aabdb-105">Ресурс **shareAction** предоставляет сведения о [действии][activity] , в котором общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="aabdb-105">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="aabdb-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="aabdb-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="aabdb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aabdb-107">Properties</span></span>

| <span data-ttu-id="aabdb-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="aabdb-108">Property name</span></span> | <span data-ttu-id="aabdb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aabdb-109">Type</span></span>                       | <span data-ttu-id="aabdb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aabdb-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="aabdb-111">recipients</span><span class="sxs-lookup"><span data-stu-id="aabdb-111">recipients</span></span>    | <span data-ttu-id="aabdb-112">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="aabdb-112">[identitySet][] collection</span></span> | <span data-ttu-id="aabdb-113">Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.</span><span class="sxs-lookup"><span data-stu-id="aabdb-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="aabdb-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aabdb-115">JSON representation</span></span>

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

