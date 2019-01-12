---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 4787672df6462e8d1f343e4dace43ede7c79ff37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991183"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="692cb-103">Тип ресурса office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="692cb-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="692cb-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="692cb-104">Properties</span></span>

| <span data-ttu-id="692cb-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="692cb-105">Property</span></span>          | <span data-ttu-id="692cb-106">Тип</span><span class="sxs-lookup"><span data-stu-id="692cb-106">Type</span></span>   | <span data-ttu-id="692cb-107">Описание</span><span class="sxs-lookup"><span data-stu-id="692cb-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="692cb-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="692cb-108">reportRefreshDate</span></span> | <span data-ttu-id="692cb-109">Date</span><span class="sxs-lookup"><span data-stu-id="692cb-109">Date</span></span>   | <span data-ttu-id="692cb-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="692cb-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="692cb-111">productType</span><span class="sxs-lookup"><span data-stu-id="692cb-111">productType</span></span>       | <span data-ttu-id="692cb-112">String</span><span class="sxs-lookup"><span data-stu-id="692cb-112">String</span></span> | <span data-ttu-id="692cb-113">Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="692cb-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="692cb-114">Windows</span><span class="sxs-lookup"><span data-stu-id="692cb-114">windows</span></span>           | <span data-ttu-id="692cb-115">Int64</span><span class="sxs-lookup"><span data-stu-id="692cb-115">Int64</span></span>  | <span data-ttu-id="692cb-116">Число активации в Windows.</span><span class="sxs-lookup"><span data-stu-id="692cb-116">The activation count on Windows.</span></span> <span data-ttu-id="692cb-117">Эта цифра включает в себя каждые активации на компьютерах под управлением Windows.</span><span class="sxs-lookup"><span data-stu-id="692cb-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="692cb-118">mac</span><span class="sxs-lookup"><span data-stu-id="692cb-118">mac</span></span>               | <span data-ttu-id="692cb-119">Int64</span><span class="sxs-lookup"><span data-stu-id="692cb-119">Int64</span></span>  | <span data-ttu-id="692cb-120">Число активации на Mac OS.</span><span class="sxs-lookup"><span data-stu-id="692cb-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="692cb-121">Android (en)</span><span class="sxs-lookup"><span data-stu-id="692cb-121">android</span></span>           | <span data-ttu-id="692cb-122">Int64</span><span class="sxs-lookup"><span data-stu-id="692cb-122">Int64</span></span>  | <span data-ttu-id="692cb-123">Число активации на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="692cb-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="692cb-124">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="692cb-124">ios</span></span>               | <span data-ttu-id="692cb-125">Int64</span><span class="sxs-lookup"><span data-stu-id="692cb-125">Int64</span></span>  | <span data-ttu-id="692cb-126">Число активации на операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="692cb-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="692cb-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="692cb-127">windows10Mobile</span></span>   | <span data-ttu-id="692cb-128">Int64</span><span class="sxs-lookup"><span data-stu-id="692cb-128">Int64</span></span>  | <span data-ttu-id="692cb-129">Активация на количество Windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="692cb-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="692cb-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="692cb-130">JSON representation</span></span>

<span data-ttu-id="692cb-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="692cb-131">The following is a JSON representation of the resource.</span></span>

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
