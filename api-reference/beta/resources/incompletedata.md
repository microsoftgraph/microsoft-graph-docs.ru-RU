---
author: daspek
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
ms.date: 10/06/2017
title: инкомплетедата
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6505d02ee7436e02d90627cfd38a83e3e436706a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016568"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="cd780-103">Тип ресурса Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="cd780-103">incompleteData resource type</span></span>

<span data-ttu-id="cd780-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd780-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd780-105">Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.</span><span class="sxs-lookup"><span data-stu-id="cd780-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="cd780-106">Свойства, содержащиеся в, могут содержать сведения о причине неполных данных.</span><span class="sxs-lookup"><span data-stu-id="cd780-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd780-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd780-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="cd780-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd780-108">Properties</span></span>

| <span data-ttu-id="cd780-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd780-109">Property</span></span>                  | <span data-ttu-id="cd780-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cd780-110">Type</span></span>           | <span data-ttu-id="cd780-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cd780-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="cd780-112">миссингдатабефоредатетиме</span><span class="sxs-lookup"><span data-stu-id="cd780-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="cd780-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd780-113">DateTimeOffset</span></span> | <span data-ttu-id="cd780-114">В службе нет исходных данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="cd780-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="cd780-115">вассроттлед</span><span class="sxs-lookup"><span data-stu-id="cd780-115">wasThrottled</span></span>              | <span data-ttu-id="cd780-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd780-116">Boolean</span></span>        | <span data-ttu-id="cd780-117">Некоторые данные не были записаны из-за чрезмерной активности.</span><span class="sxs-lookup"><span data-stu-id="cd780-117">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->


