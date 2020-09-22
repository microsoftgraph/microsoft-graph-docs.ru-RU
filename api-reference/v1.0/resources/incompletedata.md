---
author: daspek
ms.author: dspektor
title: Тип ресурса Инкомплетедата
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 424a857468473532dc6f2a39c4c13dc94b52406c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054891"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="4cebc-103">Тип ресурса Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="4cebc-103">incompleteData resource type</span></span>

<span data-ttu-id="4cebc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cebc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cebc-105">Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.</span><span class="sxs-lookup"><span data-stu-id="4cebc-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="4cebc-106">В свойствах могут содержаться сведения о причине неполных данных.</span><span class="sxs-lookup"><span data-stu-id="4cebc-106">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="4cebc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cebc-107">Properties</span></span>

| <span data-ttu-id="4cebc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cebc-108">Property</span></span>                  | <span data-ttu-id="4cebc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4cebc-109">Type</span></span>           | <span data-ttu-id="4cebc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4cebc-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="4cebc-111">миссингдатабефоредатетиме</span><span class="sxs-lookup"><span data-stu-id="4cebc-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="4cebc-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cebc-112">DateTimeOffset</span></span> | <span data-ttu-id="4cebc-113">В службе нет исходных данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="4cebc-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="4cebc-114">вассроттлед</span><span class="sxs-lookup"><span data-stu-id="4cebc-114">wasThrottled</span></span>              | <span data-ttu-id="4cebc-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cebc-115">Boolean</span></span>        | <span data-ttu-id="4cebc-116">Некоторые данные не были записаны из-за чрезмерной активности.</span><span class="sxs-lookup"><span data-stu-id="4cebc-116">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cebc-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4cebc-117">JSON representation</span></span>

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

