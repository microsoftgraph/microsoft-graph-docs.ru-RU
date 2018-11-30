---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: e53a979ac627735ef63a24e1823d83f4c9fe9f7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081428"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="7af11-103">Тип ресурса office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="7af11-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7af11-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7af11-104">Properties</span></span>

| <span data-ttu-id="7af11-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7af11-105">Property</span></span>          | <span data-ttu-id="7af11-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7af11-106">Type</span></span>   | <span data-ttu-id="7af11-107">Description</span><span class="sxs-lookup"><span data-stu-id="7af11-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="7af11-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7af11-108">reportRefreshDate</span></span> | <span data-ttu-id="7af11-109">Date</span><span class="sxs-lookup"><span data-stu-id="7af11-109">Date</span></span>   | <span data-ttu-id="7af11-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="7af11-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="7af11-111">productType</span><span class="sxs-lookup"><span data-stu-id="7af11-111">productType</span></span>       | <span data-ttu-id="7af11-112">String</span><span class="sxs-lookup"><span data-stu-id="7af11-112">String</span></span> | <span data-ttu-id="7af11-113">Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="7af11-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="7af11-114">Windows</span><span class="sxs-lookup"><span data-stu-id="7af11-114">windows</span></span>           | <span data-ttu-id="7af11-115">Int64</span><span class="sxs-lookup"><span data-stu-id="7af11-115">Int64</span></span>  | <span data-ttu-id="7af11-116">Число активации в Windows.</span><span class="sxs-lookup"><span data-stu-id="7af11-116">The activation count on Windows.</span></span> <span data-ttu-id="7af11-117">Эта цифра включает в себя каждые активации на компьютерах под управлением Windows.</span><span class="sxs-lookup"><span data-stu-id="7af11-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="7af11-118">mac</span><span class="sxs-lookup"><span data-stu-id="7af11-118">mac</span></span>               | <span data-ttu-id="7af11-119">Int64</span><span class="sxs-lookup"><span data-stu-id="7af11-119">Int64</span></span>  | <span data-ttu-id="7af11-120">Число активации на Mac OS.</span><span class="sxs-lookup"><span data-stu-id="7af11-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="7af11-121">Android (en)</span><span class="sxs-lookup"><span data-stu-id="7af11-121">android</span></span>           | <span data-ttu-id="7af11-122">Int64</span><span class="sxs-lookup"><span data-stu-id="7af11-122">Int64</span></span>  | <span data-ttu-id="7af11-123">Число активации на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="7af11-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="7af11-124">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="7af11-124">ios</span></span>               | <span data-ttu-id="7af11-125">Int64</span><span class="sxs-lookup"><span data-stu-id="7af11-125">Int64</span></span>  | <span data-ttu-id="7af11-126">Число активации на операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="7af11-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="7af11-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="7af11-127">windows10Mobile</span></span>   | <span data-ttu-id="7af11-128">Int64</span><span class="sxs-lookup"><span data-stu-id="7af11-128">Int64</span></span>  | <span data-ttu-id="7af11-129">Активация на количество Windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="7af11-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7af11-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7af11-130">JSON representation</span></span>

<span data-ttu-id="7af11-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7af11-131">The following is a JSON representation of the resource.</span></span>

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
