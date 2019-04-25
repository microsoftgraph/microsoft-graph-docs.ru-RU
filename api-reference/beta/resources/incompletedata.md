---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Инкомплетедата
localization_priority: Normal
ms.openlocfilehash: f2493263d5293b95cbe386b46c56429d11dda089
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549036"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="f45ac-102">Тип ресурса Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="f45ac-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f45ac-103">Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.</span><span class="sxs-lookup"><span data-stu-id="f45ac-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="f45ac-104">Свойства, содержащиеся в, могут содержать сведения о причине неполных данных.</span><span class="sxs-lookup"><span data-stu-id="f45ac-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f45ac-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f45ac-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="f45ac-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f45ac-106">Properties</span></span>

| <span data-ttu-id="f45ac-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f45ac-107">Property</span></span>                  | <span data-ttu-id="f45ac-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f45ac-108">Type</span></span>           | <span data-ttu-id="f45ac-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f45ac-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="f45ac-110">Миссингдатабефоредатетиме</span><span class="sxs-lookup"><span data-stu-id="f45ac-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="f45ac-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f45ac-111">DateTimeOffset</span></span> | <span data-ttu-id="f45ac-112">В службе нет исходных данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="f45ac-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="f45ac-113">Вассроттлед</span><span class="sxs-lookup"><span data-stu-id="f45ac-113">wasThrottled</span></span>              | <span data-ttu-id="f45ac-114">Логический</span><span class="sxs-lookup"><span data-stu-id="f45ac-114">Boolean</span></span>        | <span data-ttu-id="f45ac-115">Некоторые данные не были записаны из-за чрезмерной активности.</span><span class="sxs-lookup"><span data-stu-id="f45ac-115">Some data was not recorded due to excessive activity.</span></span>

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
