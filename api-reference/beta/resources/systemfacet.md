---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: Аспект System
localization_priority: Normal
ms.openlocfilehash: afafb69e9d887d2cb8d9537dd7ef9d3a712f3333
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528552"
---
# <a name="system-facet"></a><span data-ttu-id="4ff51-102">Аспект System</span><span class="sxs-lookup"><span data-stu-id="4ff51-102">System facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ff51-103">Аспект **System** указывает, что объект управляется системой, выполняющей необходимые ей операции.</span><span class="sxs-lookup"><span data-stu-id="4ff51-103">The **System** facet indicates that the object is managed by the system for its own operation.</span></span>
<span data-ttu-id="4ff51-104">Большинству приложений следует игнорировать элементы, содержащие аспект System.</span><span class="sxs-lookup"><span data-stu-id="4ff51-104">Most apps should ignore items that have a System facet.</span></span>

<span data-ttu-id="4ff51-105">**Примечание.** В настоящее время этот аспект пуст, но в будущих редакциях API он может быть дополнен другими свойствами.</span><span class="sxs-lookup"><span data-stu-id="4ff51-105">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ff51-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ff51-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.systemFacet", "@type.aka": "microsoft.graph.systemFacet" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="4ff51-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ff51-107">Properties</span></span>

<span data-ttu-id="4ff51-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ff51-108">None.</span></span> <span data-ttu-id="4ff51-109">Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.</span><span class="sxs-lookup"><span data-stu-id="4ff51-109">This facet is a null or not-null value and contains no properties.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/System",
  "suppressions": [
    "Error: /api-reference/beta/resources/systemfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
