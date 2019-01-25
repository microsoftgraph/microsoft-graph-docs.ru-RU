---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Root
localization_priority: Normal
ms.openlocfilehash: dda2de3e92128a9813f923d9acfef0eec94680e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510304"
---
# <a name="root-resource-type"></a><span data-ttu-id="67751-102">Тип ресурса Root</span><span class="sxs-lookup"><span data-stu-id="67751-102">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67751-103">Аспект **Root** указывает, что объект находится на верхнем уровне в иерархии.</span><span class="sxs-lookup"><span data-stu-id="67751-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="67751-104">Наличие ненулевого значения этого аспекта указывает, что объект является корневым элементом.</span><span class="sxs-lookup"><span data-stu-id="67751-104">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="67751-105">Значение null (или отсутствующее значение) указывает, что объект не является корневым.</span><span class="sxs-lookup"><span data-stu-id="67751-105">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="67751-106">**Примечание.** В настоящее время этот аспект пуст, но в будущих редакциях API он может быть дополнен другими свойствами.</span><span class="sxs-lookup"><span data-stu-id="67751-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67751-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67751-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="67751-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="67751-108">Properties</span></span>

<span data-ttu-id="67751-109">У ресурса **Root** отсутствуют свойства.</span><span class="sxs-lookup"><span data-stu-id="67751-109">The **Root** resource has no properties.</span></span>


<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root",
  "suppressions": [
    "Error: /api-reference/beta/resources/root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
