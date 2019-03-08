---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Корневой
localization_priority: Normal
ms.openlocfilehash: 8c320a34d22af5fc73a1c5d8c96dce14e176946f
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482373"
---
# <a name="root-resource-type"></a><span data-ttu-id="b5853-102">Тип ресурса Root</span><span class="sxs-lookup"><span data-stu-id="b5853-102">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5853-103">Аспект **Root** указывает, что объект находится на верхнем уровне в иерархии.</span><span class="sxs-lookup"><span data-stu-id="b5853-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="b5853-104">Наличие ненулевого значения этого аспекта указывает, что объект является корневым элементом.</span><span class="sxs-lookup"><span data-stu-id="b5853-104">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="b5853-105">Значение null (или отсутствующее значение) указывает, что объект не является корневым.</span><span class="sxs-lookup"><span data-stu-id="b5853-105">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="b5853-106">**Примечание.** В настоящее время этот аспект пуст, но в будущих редакциях API он может быть дополнен другими свойствами.</span><span class="sxs-lookup"><span data-stu-id="b5853-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5853-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5853-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="b5853-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5853-108">Properties</span></span>

<span data-ttu-id="b5853-109">У ресурса **Root** отсутствуют свойства.</span><span class="sxs-lookup"><span data-stu-id="b5853-109">The **Root** resource has no properties.</span></span>


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
