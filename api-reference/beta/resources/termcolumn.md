---
author: swapnil1993
title: тип ресурсов termColumn
description: Ресурс termColumn указывает, что значения столбца содержат данные таксономии.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6d29ec570d7f3fad798fb1e2ba213b5a998643dc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447466"
---
# <a name="termcolumn-resource-type"></a><span data-ttu-id="9d50d-103">тип ресурсов termColumn</span><span class="sxs-lookup"><span data-stu-id="9d50d-103">termColumn resource type</span></span>

<span data-ttu-id="9d50d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d50d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="9d50d-105">Указывает, что значения столбца содержат данные таксономии.</span><span class="sxs-lookup"><span data-stu-id="9d50d-105">Indicates that the column's values contains taxonomy data.</span></span>

## <a name="properties"></a><span data-ttu-id="9d50d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d50d-106">Properties</span></span>

| <span data-ttu-id="9d50d-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9d50d-107">Property name</span></span> | <span data-ttu-id="9d50d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9d50d-108">Type</span></span>   | <span data-ttu-id="9d50d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9d50d-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="9d50d-110">allowMultipleValues</span><span class="sxs-lookup"><span data-stu-id="9d50d-110">allowMultipleValues</span></span> | <span data-ttu-id="9d50d-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d50d-111">Boolean</span></span> | <span data-ttu-id="9d50d-112">Указывает, разрешит ли столбец несколько значений</span><span class="sxs-lookup"><span data-stu-id="9d50d-112">Specifies whether the column will allow more than one value</span></span>   
| <span data-ttu-id="9d50d-113">parentTerm</span><span class="sxs-lookup"><span data-stu-id="9d50d-113">parentTerm</span></span>     | <span data-ttu-id="9d50d-114">microsoft.graph.termStore.term</span><span class="sxs-lookup"><span data-stu-id="9d50d-114">microsoft.graph.termStore.term</span></span> | <span data-ttu-id="9d50d-115">Указывает термин guid, чьи дети могут быть выбраны в качестве значения столбца.</span><span class="sxs-lookup"><span data-stu-id="9d50d-115">Specifies the term guid whose children can be selected as column's value.</span></span>  
| <span data-ttu-id="9d50d-116">showFullyQualifiedName</span><span class="sxs-lookup"><span data-stu-id="9d50d-116">showFullyQualifiedName</span></span> | <span data-ttu-id="9d50d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d50d-117">Boolean</span></span> | <span data-ttu-id="9d50d-118">Указывает, отображать ли весь путь терминов или только метку терминов.</span><span class="sxs-lookup"><span data-stu-id="9d50d-118">Specifies whether to display the entire term path or only the term label.</span></span>  
| <span data-ttu-id="9d50d-119">termSet</span><span class="sxs-lookup"><span data-stu-id="9d50d-119">termSet</span></span>      | <span data-ttu-id="9d50d-120">microsoft.graph.termStore.set</span><span class="sxs-lookup"><span data-stu-id="9d50d-120">microsoft.graph.termStore.set</span></span> | <span data-ttu-id="9d50d-121">Termset, чьи дети могут быть выбраны в качестве значения столбца.</span><span class="sxs-lookup"><span data-stu-id="9d50d-121">Termset whose children can be selected as column's value.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="9d50d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d50d-122">JSON representation</span></span>

<span data-ttu-id="9d50d-123">Вот представление JSON ресурса **termColumn.**</span><span class="sxs-lookup"><span data-stu-id="9d50d-123">Here is a JSON representation of a **termColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "parentTerm": { "@type": "microsoft.graph.termStore.term" },
    "showFullyQualifiedName": false,
    "termSet": { "@type": "microsoft.graph.termStore.set" }
}
```

