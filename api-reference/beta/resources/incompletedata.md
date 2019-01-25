---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: f2493263d5293b95cbe386b46c56429d11dda089
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525089"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="3dfae-102">Тип ресурса incompleteData</span><span class="sxs-lookup"><span data-stu-id="3dfae-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dfae-103">Аспекта **incompleteData** указывает, что ресурс был создан с помощью неполные данные.</span><span class="sxs-lookup"><span data-stu-id="3dfae-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="3dfae-104">Свойства в можно указать сведения о, поэтому неполные данные.</span><span class="sxs-lookup"><span data-stu-id="3dfae-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3dfae-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3dfae-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="3dfae-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3dfae-106">Properties</span></span>

| <span data-ttu-id="3dfae-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3dfae-107">Property</span></span>                  | <span data-ttu-id="3dfae-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3dfae-108">Type</span></span>           | <span data-ttu-id="3dfae-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3dfae-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="3dfae-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="3dfae-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="3dfae-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfae-111">DateTimeOffset</span></span> | <span data-ttu-id="3dfae-112">Служба не имеет источника данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="3dfae-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="3dfae-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="3dfae-113">wasThrottled</span></span>              | <span data-ttu-id="3dfae-114">Логическое</span><span class="sxs-lookup"><span data-stu-id="3dfae-114">Boolean</span></span>        | <span data-ttu-id="3dfae-115">Не удалось записать часть данных из-за высокой активности.</span><span class="sxs-lookup"><span data-stu-id="3dfae-115">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": [
    "Error: /api-reference/beta/resources/incompletedata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
