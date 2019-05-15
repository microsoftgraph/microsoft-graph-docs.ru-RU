---
author: daspek
ms.author: dspektor
title: Тип ресурса Инкомплетедата
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f26317cf16f0773852df35941c00e88df145cc31
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970815"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="990c3-103">Тип ресурса Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="990c3-103">incompleteData resource type</span></span>

<span data-ttu-id="990c3-104">Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.</span><span class="sxs-lookup"><span data-stu-id="990c3-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="990c3-105">В свойствах могут содержаться сведения о причине неполных данных.</span><span class="sxs-lookup"><span data-stu-id="990c3-105">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="990c3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="990c3-106">Properties</span></span>

| <span data-ttu-id="990c3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="990c3-107">Property</span></span>                  | <span data-ttu-id="990c3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="990c3-108">Type</span></span>           | <span data-ttu-id="990c3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="990c3-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="990c3-110">Миссингдатабефоредатетиме</span><span class="sxs-lookup"><span data-stu-id="990c3-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="990c3-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="990c3-111">DateTimeOffset</span></span> | <span data-ttu-id="990c3-112">В службе нет исходных данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="990c3-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="990c3-113">Вассроттлед</span><span class="sxs-lookup"><span data-stu-id="990c3-113">wasThrottled</span></span>              | <span data-ttu-id="990c3-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="990c3-114">Boolean</span></span>        | <span data-ttu-id="990c3-115">Некоторые данные не были записаны из-за чрезмерной активности.</span><span class="sxs-lookup"><span data-stu-id="990c3-115">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="990c3-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="990c3-116">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/incompleteData",
  "suppressions": []
}
-->
