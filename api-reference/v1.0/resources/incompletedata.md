---
author: daspek
title: Тип ресурса incompleteData
description: Аспект incompleteData указывает, что ресурс был создан с неполными данными.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 20dda8e9d1cd321a465c7a257cb5cb7bed845351
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239935"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="65634-103">Тип ресурса incompleteData</span><span class="sxs-lookup"><span data-stu-id="65634-103">incompleteData resource type</span></span>

<span data-ttu-id="65634-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65634-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65634-105">Аспект **incompleteData указывает,** что ресурс был создан с неполными данными.</span><span class="sxs-lookup"><span data-stu-id="65634-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="65634-106">Свойства внутри могут предоставлять сведения о том, почему данные неполные.</span><span class="sxs-lookup"><span data-stu-id="65634-106">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="65634-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="65634-107">Properties</span></span>

| <span data-ttu-id="65634-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="65634-108">Property</span></span>                  | <span data-ttu-id="65634-109">Тип</span><span class="sxs-lookup"><span data-stu-id="65634-109">Type</span></span>           | <span data-ttu-id="65634-110">Описание</span><span class="sxs-lookup"><span data-stu-id="65634-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="65634-111">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="65634-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="65634-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65634-112">DateTimeOffset</span></span> | <span data-ttu-id="65634-113">Служба не имеет исходных данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="65634-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="65634-114">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="65634-114">wasThrottled</span></span>              | <span data-ttu-id="65634-115">Логическое</span><span class="sxs-lookup"><span data-stu-id="65634-115">Boolean</span></span>        | <span data-ttu-id="65634-116">Некоторые данные не были записаны из-за чрезмерной активности.</span><span class="sxs-lookup"><span data-stu-id="65634-116">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="65634-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65634-117">JSON representation</span></span>

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

