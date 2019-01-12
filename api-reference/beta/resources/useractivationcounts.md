---
title: Тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 535355d6be3f6b617d7eb293890aa05a517cfc3b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980351"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="363bf-103">Тип ресурса userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="363bf-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="363bf-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="363bf-104">Properties</span></span>

| <span data-ttu-id="363bf-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="363bf-105">Property</span></span>          | <span data-ttu-id="363bf-106">Тип</span><span class="sxs-lookup"><span data-stu-id="363bf-106">Type</span></span>   | <span data-ttu-id="363bf-107">Описание</span><span class="sxs-lookup"><span data-stu-id="363bf-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="363bf-108">productType</span><span class="sxs-lookup"><span data-stu-id="363bf-108">productType</span></span>       | <span data-ttu-id="363bf-109">Строка</span><span class="sxs-lookup"><span data-stu-id="363bf-109">String</span></span> | <span data-ttu-id="363bf-110">Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="363bf-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="363bf-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="363bf-111">lastActivatedDate</span></span> | <span data-ttu-id="363bf-112">Date</span><span class="sxs-lookup"><span data-stu-id="363bf-112">Date</span></span>   | <span data-ttu-id="363bf-113">Дата последней активации.</span><span class="sxs-lookup"><span data-stu-id="363bf-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="363bf-114">Windows</span><span class="sxs-lookup"><span data-stu-id="363bf-114">windows</span></span>           | <span data-ttu-id="363bf-115">Int64</span><span class="sxs-lookup"><span data-stu-id="363bf-115">Int64</span></span>  | <span data-ttu-id="363bf-116">Число активации в Windows.</span><span class="sxs-lookup"><span data-stu-id="363bf-116">The activation count on Windows.</span></span> <span data-ttu-id="363bf-117">Эта цифра включает в себя каждые активации на компьютерах под управлением Windows.</span><span class="sxs-lookup"><span data-stu-id="363bf-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="363bf-118">mac</span><span class="sxs-lookup"><span data-stu-id="363bf-118">mac</span></span>               | <span data-ttu-id="363bf-119">Int64</span><span class="sxs-lookup"><span data-stu-id="363bf-119">Int64</span></span>  | <span data-ttu-id="363bf-120">Число активации на Mac OS.</span><span class="sxs-lookup"><span data-stu-id="363bf-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="363bf-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="363bf-121">windows10Mobile</span></span>   | <span data-ttu-id="363bf-122">Int64</span><span class="sxs-lookup"><span data-stu-id="363bf-122">Int64</span></span>  | <span data-ttu-id="363bf-123">Активация на количество Windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="363bf-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="363bf-124">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="363bf-124">ios</span></span>               | <span data-ttu-id="363bf-125">Int64</span><span class="sxs-lookup"><span data-stu-id="363bf-125">Int64</span></span>  | <span data-ttu-id="363bf-126">Число активации на операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="363bf-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="363bf-127">Android (en)</span><span class="sxs-lookup"><span data-stu-id="363bf-127">android</span></span>           | <span data-ttu-id="363bf-128">Int64</span><span class="sxs-lookup"><span data-stu-id="363bf-128">Int64</span></span>  | <span data-ttu-id="363bf-129">Число активации на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="363bf-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="363bf-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="363bf-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="363bf-131">Логический</span><span class="sxs-lookup"><span data-stu-id="363bf-131">Boolean</span></span> | <span data-ttu-id="363bf-132">Значение true, если пользователь продукта на совместно используемый компьютер перед.</span><span class="sxs-lookup"><span data-stu-id="363bf-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="363bf-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="363bf-133">JSON representation</span></span>

<span data-ttu-id="363bf-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="363bf-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
} -->

```json
{
  "productType": "String", 
  "lastActivatedDate": "Date", 
  "windows": 1024, 
  "mac": 1024, 
  "windows10Mobile": 1024, 
  "ios": 1024, 
  "android": 1024,
  "activatedOnSharedComputer": true 
}
```
