---
author: daspek
ms.author: dspektor
title: Тип ресурса shareAction
description: Объект shareAction предоставляет сведения о том, к которому был предоставлен общий доступ к элементу в действии Share.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f8b4870ec82a2f264d6f67cdd02cd22c9747e51e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533739"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="dddf4-103">Тип ресурса shareAction</span><span class="sxs-lookup"><span data-stu-id="dddf4-103">shareAction resource type</span></span>

<span data-ttu-id="dddf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dddf4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dddf4-105">Ресурс **shareAction** предоставляет сведения о [действии][activity] , в котором общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="dddf4-105">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="dddf4-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="dddf4-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="dddf4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dddf4-107">Properties</span></span>

| <span data-ttu-id="dddf4-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dddf4-108">Property name</span></span> | <span data-ttu-id="dddf4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dddf4-109">Type</span></span>                       | <span data-ttu-id="dddf4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dddf4-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="dddf4-111">recipients</span><span class="sxs-lookup"><span data-stu-id="dddf4-111">recipients</span></span>    | <span data-ttu-id="dddf4-112">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dddf4-112">[identitySet][] collection</span></span> | <span data-ttu-id="dddf4-113">Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.</span><span class="sxs-lookup"><span data-stu-id="dddf4-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="dddf4-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dddf4-115">JSON representation</span></span>

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
