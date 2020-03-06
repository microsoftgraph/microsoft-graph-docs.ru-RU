---
author: daspek
ms.author: dspektor
title: Тип ресурса Инкомплетедата
description: Аспект Инкомплетедата указывает, что ресурс был создан с неполными данными.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5fdf78b0fdb0a34e87296619c477d9f868d0756e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531321"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="b61a3-103">Тип ресурса Инкомплетедата</span><span class="sxs-lookup"><span data-stu-id="b61a3-103">incompleteData resource type</span></span>

<span data-ttu-id="b61a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b61a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b61a3-105">Аспект **инкомплетедата** указывает, что ресурс был создан с неполными данными.</span><span class="sxs-lookup"><span data-stu-id="b61a3-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="b61a3-106">В свойствах могут содержаться сведения о причине неполных данных.</span><span class="sxs-lookup"><span data-stu-id="b61a3-106">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="b61a3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b61a3-107">Properties</span></span>

| <span data-ttu-id="b61a3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b61a3-108">Property</span></span>                  | <span data-ttu-id="b61a3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b61a3-109">Type</span></span>           | <span data-ttu-id="b61a3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b61a3-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="b61a3-111">миссингдатабефоредатетиме</span><span class="sxs-lookup"><span data-stu-id="b61a3-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="b61a3-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b61a3-112">DateTimeOffset</span></span> | <span data-ttu-id="b61a3-113">В службе нет исходных данных до указанного времени.</span><span class="sxs-lookup"><span data-stu-id="b61a3-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="b61a3-114">вассроттлед</span><span class="sxs-lookup"><span data-stu-id="b61a3-114">wasThrottled</span></span>              | <span data-ttu-id="b61a3-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b61a3-115">Boolean</span></span>        | <span data-ttu-id="b61a3-116">Некоторые данные не были записаны из-за чрезмерной активности.</span><span class="sxs-lookup"><span data-stu-id="b61a3-116">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b61a3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b61a3-117">JSON representation</span></span>

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
