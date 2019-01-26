---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7bc21be693a5c68ecd5c6a1e4e44d53c9261acdb
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575529"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="fbb1e-103">Тип ресурса office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="fbb1e-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fbb1e-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbb1e-104">Properties</span></span>

| <span data-ttu-id="fbb1e-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbb1e-105">Property</span></span>          | <span data-ttu-id="fbb1e-106">Тип</span><span class="sxs-lookup"><span data-stu-id="fbb1e-106">Type</span></span>   | <span data-ttu-id="fbb1e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="fbb1e-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="fbb1e-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fbb1e-108">reportRefreshDate</span></span> | <span data-ttu-id="fbb1e-109">Date</span><span class="sxs-lookup"><span data-stu-id="fbb1e-109">Date</span></span>   | <span data-ttu-id="fbb1e-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="fbb1e-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="fbb1e-111">productType</span><span class="sxs-lookup"><span data-stu-id="fbb1e-111">productType</span></span>       | <span data-ttu-id="fbb1e-112">Строка</span><span class="sxs-lookup"><span data-stu-id="fbb1e-112">String</span></span> | <span data-ttu-id="fbb1e-113">Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="fbb1e-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="fbb1e-114">Windows</span><span class="sxs-lookup"><span data-stu-id="fbb1e-114">windows</span></span>           | <span data-ttu-id="fbb1e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="fbb1e-115">Int64</span></span>  | <span data-ttu-id="fbb1e-116">Число активации в Windows.</span><span class="sxs-lookup"><span data-stu-id="fbb1e-116">The activation count on Windows.</span></span> <span data-ttu-id="fbb1e-117">Эта цифра включает в себя каждые активации на компьютерах под управлением Windows.</span><span class="sxs-lookup"><span data-stu-id="fbb1e-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="fbb1e-118">mac</span><span class="sxs-lookup"><span data-stu-id="fbb1e-118">mac</span></span>               | <span data-ttu-id="fbb1e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="fbb1e-119">Int64</span></span>  | <span data-ttu-id="fbb1e-120">Число активации на Mac OS.</span><span class="sxs-lookup"><span data-stu-id="fbb1e-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="fbb1e-121">Android (en)</span><span class="sxs-lookup"><span data-stu-id="fbb1e-121">android</span></span>           | <span data-ttu-id="fbb1e-122">Int64</span><span class="sxs-lookup"><span data-stu-id="fbb1e-122">Int64</span></span>  | <span data-ttu-id="fbb1e-123">Число активации на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="fbb1e-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="fbb1e-124">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="fbb1e-124">ios</span></span>               | <span data-ttu-id="fbb1e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="fbb1e-125">Int64</span></span>  | <span data-ttu-id="fbb1e-126">Число активации на операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="fbb1e-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="fbb1e-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="fbb1e-127">windows10Mobile</span></span>   | <span data-ttu-id="fbb1e-128">Int64</span><span class="sxs-lookup"><span data-stu-id="fbb1e-128">Int64</span></span>  | <span data-ttu-id="fbb1e-129">Активация на количество Windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="fbb1e-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fbb1e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbb1e-130">JSON representation</span></span>

<span data-ttu-id="fbb1e-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbb1e-131">The following is a JSON representation of the resource.</span></span>

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
