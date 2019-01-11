---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 30386b3833b8140d4c602e27cb3a78f3a68670dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824992"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="4a049-103">Тип ресурса office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="4a049-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4a049-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a049-104">Properties</span></span>

| <span data-ttu-id="4a049-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a049-105">Property</span></span>          | <span data-ttu-id="4a049-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4a049-106">Type</span></span>   | <span data-ttu-id="4a049-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4a049-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="4a049-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4a049-108">reportRefreshDate</span></span> | <span data-ttu-id="4a049-109">Date</span><span class="sxs-lookup"><span data-stu-id="4a049-109">Date</span></span>   | <span data-ttu-id="4a049-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="4a049-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="4a049-111">productType</span><span class="sxs-lookup"><span data-stu-id="4a049-111">productType</span></span>       | <span data-ttu-id="4a049-112">Строка</span><span class="sxs-lookup"><span data-stu-id="4a049-112">String</span></span> | <span data-ttu-id="4a049-113">Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="4a049-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="4a049-114">Windows</span><span class="sxs-lookup"><span data-stu-id="4a049-114">windows</span></span>           | <span data-ttu-id="4a049-115">Int64</span><span class="sxs-lookup"><span data-stu-id="4a049-115">Int64</span></span>  | <span data-ttu-id="4a049-116">Число активации в Windows.</span><span class="sxs-lookup"><span data-stu-id="4a049-116">The activation count on Windows.</span></span> <span data-ttu-id="4a049-117">Эта цифра включает в себя каждые активации на компьютерах под управлением Windows.</span><span class="sxs-lookup"><span data-stu-id="4a049-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="4a049-118">mac</span><span class="sxs-lookup"><span data-stu-id="4a049-118">mac</span></span>               | <span data-ttu-id="4a049-119">Int64</span><span class="sxs-lookup"><span data-stu-id="4a049-119">Int64</span></span>  | <span data-ttu-id="4a049-120">Число активации на Mac OS.</span><span class="sxs-lookup"><span data-stu-id="4a049-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="4a049-121">Android (en)</span><span class="sxs-lookup"><span data-stu-id="4a049-121">android</span></span>           | <span data-ttu-id="4a049-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4a049-122">Int64</span></span>  | <span data-ttu-id="4a049-123">Число активации на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="4a049-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="4a049-124">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="4a049-124">ios</span></span>               | <span data-ttu-id="4a049-125">Int64</span><span class="sxs-lookup"><span data-stu-id="4a049-125">Int64</span></span>  | <span data-ttu-id="4a049-126">Число активации на операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="4a049-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="4a049-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="4a049-127">windows10Mobile</span></span>   | <span data-ttu-id="4a049-128">Int64</span><span class="sxs-lookup"><span data-stu-id="4a049-128">Int64</span></span>  | <span data-ttu-id="4a049-129">Активация на количество Windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="4a049-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a049-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a049-130">JSON representation</span></span>

<span data-ttu-id="4a049-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a049-131">The following is a JSON representation of the resource.</span></span>

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
