---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 1e514eb538b1edc4d9681b9937fe8cfeecc40b23
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896891"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="aa100-103">Тип ресурса office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="aa100-103">office365ActivationCounts resource type</span></span>

<span data-ttu-id="aa100-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa100-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="aa100-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa100-105">Properties</span></span>

| <span data-ttu-id="aa100-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa100-106">Property</span></span>          | <span data-ttu-id="aa100-107">Тип</span><span class="sxs-lookup"><span data-stu-id="aa100-107">Type</span></span>   | <span data-ttu-id="aa100-108">Описание</span><span class="sxs-lookup"><span data-stu-id="aa100-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="aa100-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="aa100-109">reportRefreshDate</span></span> | <span data-ttu-id="aa100-110">Дата</span><span class="sxs-lookup"><span data-stu-id="aa100-110">Date</span></span>   | <span data-ttu-id="aa100-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="aa100-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="aa100-112">продукттипе</span><span class="sxs-lookup"><span data-stu-id="aa100-112">productType</span></span>       | <span data-ttu-id="aa100-113">String</span><span class="sxs-lookup"><span data-stu-id="aa100-113">String</span></span> | <span data-ttu-id="aa100-114">Тип продукта, например "Microsoft 365 профессиональный плюс" или "клиент Project".</span><span class="sxs-lookup"><span data-stu-id="aa100-114">The product type, such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="aa100-115">под</span><span class="sxs-lookup"><span data-stu-id="aa100-115">windows</span></span>           | <span data-ttu-id="aa100-116">Int64</span><span class="sxs-lookup"><span data-stu-id="aa100-116">Int64</span></span>  | <span data-ttu-id="aa100-117">Счетчик активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="aa100-117">The activation count on Windows.</span></span> <span data-ttu-id="aa100-118">Это число включает все активации на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="aa100-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="aa100-119">mac</span><span class="sxs-lookup"><span data-stu-id="aa100-119">mac</span></span>               | <span data-ttu-id="aa100-120">Int64</span><span class="sxs-lookup"><span data-stu-id="aa100-120">Int64</span></span>  | <span data-ttu-id="aa100-121">Число активаций в Mac OS.</span><span class="sxs-lookup"><span data-stu-id="aa100-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="aa100-122">ОС</span><span class="sxs-lookup"><span data-stu-id="aa100-122">android</span></span>           | <span data-ttu-id="aa100-123">Int64</span><span class="sxs-lookup"><span data-stu-id="aa100-123">Int64</span></span>  | <span data-ttu-id="aa100-124">Счетчик активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="aa100-124">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="aa100-125">модуле</span><span class="sxs-lookup"><span data-stu-id="aa100-125">ios</span></span>               | <span data-ttu-id="aa100-126">Int64</span><span class="sxs-lookup"><span data-stu-id="aa100-126">Int64</span></span>  | <span data-ttu-id="aa100-127">Счетчик активаций на iOS.</span><span class="sxs-lookup"><span data-stu-id="aa100-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="aa100-128">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="aa100-128">windows10Mobile</span></span>   | <span data-ttu-id="aa100-129">Int64</span><span class="sxs-lookup"><span data-stu-id="aa100-129">Int64</span></span>  | <span data-ttu-id="aa100-130">Счетчик активаций для Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="aa100-130">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aa100-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aa100-131">JSON representation</span></span>

<span data-ttu-id="aa100-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa100-132">The following is a JSON representation of the resource.</span></span>

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
