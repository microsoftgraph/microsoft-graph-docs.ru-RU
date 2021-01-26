---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7ac3b6bb14b347f4ab273bbf65ce767f1ae6e1a2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983205"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="53524-103">Тип ресурса office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="53524-103">office365ActivationCounts resource type</span></span>

<span data-ttu-id="53524-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53524-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="53524-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="53524-105">Properties</span></span>

| <span data-ttu-id="53524-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="53524-106">Property</span></span>          | <span data-ttu-id="53524-107">Тип</span><span class="sxs-lookup"><span data-stu-id="53524-107">Type</span></span>   | <span data-ttu-id="53524-108">Описание</span><span class="sxs-lookup"><span data-stu-id="53524-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="53524-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="53524-109">reportRefreshDate</span></span> | <span data-ttu-id="53524-110">Дата</span><span class="sxs-lookup"><span data-stu-id="53524-110">Date</span></span>   | <span data-ttu-id="53524-111">Последняя дата содержимого.</span><span class="sxs-lookup"><span data-stu-id="53524-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="53524-112">productType</span><span class="sxs-lookup"><span data-stu-id="53524-112">productType</span></span>       | <span data-ttu-id="53524-113">String</span><span class="sxs-lookup"><span data-stu-id="53524-113">String</span></span> | <span data-ttu-id="53524-114">Тип продукта, например "Microsoft 365 профессиональныйplus" или "Project Client".</span><span class="sxs-lookup"><span data-stu-id="53524-114">The product type, such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="53524-115">windows</span><span class="sxs-lookup"><span data-stu-id="53524-115">windows</span></span>           | <span data-ttu-id="53524-116">Int64</span><span class="sxs-lookup"><span data-stu-id="53524-116">Int64</span></span>  | <span data-ttu-id="53524-117">Количество активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="53524-117">The activation count on Windows.</span></span> <span data-ttu-id="53524-118">Это число включает каждую активацию на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="53524-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="53524-119">mac</span><span class="sxs-lookup"><span data-stu-id="53524-119">mac</span></span>               | <span data-ttu-id="53524-120">Int64</span><span class="sxs-lookup"><span data-stu-id="53524-120">Int64</span></span>  | <span data-ttu-id="53524-121">Количество активаций для Mac OS.</span><span class="sxs-lookup"><span data-stu-id="53524-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="53524-122">android</span><span class="sxs-lookup"><span data-stu-id="53524-122">android</span></span>           | <span data-ttu-id="53524-123">Int64</span><span class="sxs-lookup"><span data-stu-id="53524-123">Int64</span></span>  | <span data-ttu-id="53524-124">Количество активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="53524-124">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="53524-125">ios</span><span class="sxs-lookup"><span data-stu-id="53524-125">ios</span></span>               | <span data-ttu-id="53524-126">Int64</span><span class="sxs-lookup"><span data-stu-id="53524-126">Int64</span></span>  | <span data-ttu-id="53524-127">Количество активаций для iOS.</span><span class="sxs-lookup"><span data-stu-id="53524-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="53524-128">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="53524-128">windows10Mobile</span></span>   | <span data-ttu-id="53524-129">Int64</span><span class="sxs-lookup"><span data-stu-id="53524-129">Int64</span></span>  | <span data-ttu-id="53524-130">Количество активаций в Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="53524-130">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="53524-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53524-131">JSON representation</span></span>

<span data-ttu-id="53524-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53524-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```


