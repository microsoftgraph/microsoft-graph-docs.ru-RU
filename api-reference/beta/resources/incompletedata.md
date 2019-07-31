---
author: daspek
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
ms.date: 10/06/2017
title: Инкомплетедата
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 23d78fa3605259031fc2c408e93a0461bb12cb28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006285"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="2b070-103">Тип ресурса Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="2b070-103">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b070-104">Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.</span><span class="sxs-lookup"><span data-stu-id="2b070-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="2b070-105">Свойства, содержащиеся в, могут содержать сведения о причине неполных данных.</span><span class="sxs-lookup"><span data-stu-id="2b070-105">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b070-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b070-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="2b070-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b070-107">Properties</span></span>

| <span data-ttu-id="2b070-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b070-108">Property</span></span>                  | <span data-ttu-id="2b070-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2b070-109">Type</span></span>           | <span data-ttu-id="2b070-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2b070-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="2b070-111">Миссингдатабефоредатетиме</span><span class="sxs-lookup"><span data-stu-id="2b070-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="2b070-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b070-112">DateTimeOffset</span></span> | <span data-ttu-id="2b070-113">В службе нет исходных данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="2b070-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="2b070-114">Вассроттлед</span><span class="sxs-lookup"><span data-stu-id="2b070-114">wasThrottled</span></span>              | <span data-ttu-id="2b070-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b070-115">Boolean</span></span>        | <span data-ttu-id="2b070-116">Некоторые данные не были записаны из-за чрезмерной активности.</span><span class="sxs-lookup"><span data-stu-id="2b070-116">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
