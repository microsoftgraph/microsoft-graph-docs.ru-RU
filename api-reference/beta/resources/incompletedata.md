---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Инкомплетедата
localization_priority: Normal
ms.openlocfilehash: 40c1b782384076eefc986f67dc1736f191feb7b7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339969"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="01bc3-102">Тип ресурса Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="01bc3-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01bc3-103">Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.</span><span class="sxs-lookup"><span data-stu-id="01bc3-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="01bc3-104">Свойства, содержащиеся в, могут содержать сведения о причине неполных данных.</span><span class="sxs-lookup"><span data-stu-id="01bc3-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01bc3-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01bc3-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="01bc3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="01bc3-106">Properties</span></span>

| <span data-ttu-id="01bc3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="01bc3-107">Property</span></span>                  | <span data-ttu-id="01bc3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="01bc3-108">Type</span></span>           | <span data-ttu-id="01bc3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="01bc3-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="01bc3-110">Миссингдатабефоредатетиме</span><span class="sxs-lookup"><span data-stu-id="01bc3-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="01bc3-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01bc3-111">DateTimeOffset</span></span> | <span data-ttu-id="01bc3-112">В службе нет исходных данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="01bc3-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="01bc3-113">Вассроттлед</span><span class="sxs-lookup"><span data-stu-id="01bc3-113">wasThrottled</span></span>              | <span data-ttu-id="01bc3-114">Логический</span><span class="sxs-lookup"><span data-stu-id="01bc3-114">Boolean</span></span>        | <span data-ttu-id="01bc3-115">Некоторые данные не были записаны из-за чрезмерной активности.</span><span class="sxs-lookup"><span data-stu-id="01bc3-115">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
