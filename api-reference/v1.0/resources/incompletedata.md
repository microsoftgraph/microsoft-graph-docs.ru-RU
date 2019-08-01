---
author: daspek
ms.author: dspektor
title: Тип ресурса Инкомплетедата
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0ac77c5dc4daed9330c4fb71185e9505feee5048
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029241"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="c21a2-103">Тип ресурса Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="c21a2-103">incompleteData resource type</span></span>

<span data-ttu-id="c21a2-104">Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.</span><span class="sxs-lookup"><span data-stu-id="c21a2-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="c21a2-105">В свойствах могут содержаться сведения о причине неполных данных.</span><span class="sxs-lookup"><span data-stu-id="c21a2-105">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="c21a2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c21a2-106">Properties</span></span>

| <span data-ttu-id="c21a2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c21a2-107">Property</span></span>                  | <span data-ttu-id="c21a2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c21a2-108">Type</span></span>           | <span data-ttu-id="c21a2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c21a2-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="c21a2-110">Миссингдатабефоредатетиме</span><span class="sxs-lookup"><span data-stu-id="c21a2-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="c21a2-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c21a2-111">DateTimeOffset</span></span> | <span data-ttu-id="c21a2-112">В службе нет исходных данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="c21a2-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="c21a2-113">Вассроттлед</span><span class="sxs-lookup"><span data-stu-id="c21a2-113">wasThrottled</span></span>              | <span data-ttu-id="c21a2-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="c21a2-114">Boolean</span></span>        | <span data-ttu-id="c21a2-115">Некоторые данные не были записаны из-за чрезмерной активности.</span><span class="sxs-lookup"><span data-stu-id="c21a2-115">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c21a2-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c21a2-116">JSON representation</span></span>

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
