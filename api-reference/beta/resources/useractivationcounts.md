---
title: Тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 022b73310a54877889efebabbb6e8fc4ab71fb65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077807"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="d9d2b-103">Тип ресурса userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="d9d2b-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d9d2b-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9d2b-104">Properties</span></span>

| <span data-ttu-id="d9d2b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9d2b-105">Property</span></span>          | <span data-ttu-id="d9d2b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d9d2b-106">Type</span></span>   | <span data-ttu-id="d9d2b-107">Description</span><span class="sxs-lookup"><span data-stu-id="d9d2b-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d9d2b-108">productType</span><span class="sxs-lookup"><span data-stu-id="d9d2b-108">productType</span></span>       | <span data-ttu-id="d9d2b-109">String</span><span class="sxs-lookup"><span data-stu-id="d9d2b-109">String</span></span> | <span data-ttu-id="d9d2b-110">Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="d9d2b-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="d9d2b-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="d9d2b-111">lastActivatedDate</span></span> | <span data-ttu-id="d9d2b-112">Date</span><span class="sxs-lookup"><span data-stu-id="d9d2b-112">Date</span></span>   | <span data-ttu-id="d9d2b-113">Дата последней активации.</span><span class="sxs-lookup"><span data-stu-id="d9d2b-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="d9d2b-114">Windows</span><span class="sxs-lookup"><span data-stu-id="d9d2b-114">windows</span></span>           | <span data-ttu-id="d9d2b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d9d2b-115">Int64</span></span>  | <span data-ttu-id="d9d2b-116">Число активации в Windows.</span><span class="sxs-lookup"><span data-stu-id="d9d2b-116">The activation count on Windows.</span></span> <span data-ttu-id="d9d2b-117">Эта цифра включает в себя каждые активации на компьютерах под управлением Windows.</span><span class="sxs-lookup"><span data-stu-id="d9d2b-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="d9d2b-118">mac</span><span class="sxs-lookup"><span data-stu-id="d9d2b-118">mac</span></span>               | <span data-ttu-id="d9d2b-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d9d2b-119">Int64</span></span>  | <span data-ttu-id="d9d2b-120">Число активации на Mac OS.</span><span class="sxs-lookup"><span data-stu-id="d9d2b-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="d9d2b-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="d9d2b-121">windows10Mobile</span></span>   | <span data-ttu-id="d9d2b-122">Int64</span><span class="sxs-lookup"><span data-stu-id="d9d2b-122">Int64</span></span>  | <span data-ttu-id="d9d2b-123">Активация на количество Windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="d9d2b-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="d9d2b-124">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="d9d2b-124">ios</span></span>               | <span data-ttu-id="d9d2b-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d9d2b-125">Int64</span></span>  | <span data-ttu-id="d9d2b-126">Число активации на операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="d9d2b-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="d9d2b-127">Android (en)</span><span class="sxs-lookup"><span data-stu-id="d9d2b-127">android</span></span>           | <span data-ttu-id="d9d2b-128">Int64</span><span class="sxs-lookup"><span data-stu-id="d9d2b-128">Int64</span></span>  | <span data-ttu-id="d9d2b-129">Число активации на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="d9d2b-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="d9d2b-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="d9d2b-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="d9d2b-131">Логический</span><span class="sxs-lookup"><span data-stu-id="d9d2b-131">Boolean</span></span> | <span data-ttu-id="d9d2b-132">Значение true, если пользователь продукта на совместно используемый компьютер перед.</span><span class="sxs-lookup"><span data-stu-id="d9d2b-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d9d2b-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9d2b-133">JSON representation</span></span>

<span data-ttu-id="d9d2b-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9d2b-134">The following is a JSON representation of the resource.</span></span>

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
