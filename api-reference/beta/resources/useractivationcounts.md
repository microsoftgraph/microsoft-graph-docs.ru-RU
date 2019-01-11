---
title: Тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: cae194545f13d312ee78b572659017752e43a6a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845292"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="c4a74-103">Тип ресурса userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="c4a74-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c4a74-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4a74-104">Properties</span></span>

| <span data-ttu-id="c4a74-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4a74-105">Property</span></span>          | <span data-ttu-id="c4a74-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c4a74-106">Type</span></span>   | <span data-ttu-id="c4a74-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c4a74-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="c4a74-108">productType</span><span class="sxs-lookup"><span data-stu-id="c4a74-108">productType</span></span>       | <span data-ttu-id="c4a74-109">Строка</span><span class="sxs-lookup"><span data-stu-id="c4a74-109">String</span></span> | <span data-ttu-id="c4a74-110">Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="c4a74-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="c4a74-111">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="c4a74-111">lastActivatedDate</span></span> | <span data-ttu-id="c4a74-112">Date</span><span class="sxs-lookup"><span data-stu-id="c4a74-112">Date</span></span>   | <span data-ttu-id="c4a74-113">Дата последней активации.</span><span class="sxs-lookup"><span data-stu-id="c4a74-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="c4a74-114">Windows</span><span class="sxs-lookup"><span data-stu-id="c4a74-114">windows</span></span>           | <span data-ttu-id="c4a74-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c4a74-115">Int64</span></span>  | <span data-ttu-id="c4a74-116">Число активации в Windows.</span><span class="sxs-lookup"><span data-stu-id="c4a74-116">The activation count on Windows.</span></span> <span data-ttu-id="c4a74-117">Эта цифра включает в себя каждые активации на компьютерах под управлением Windows.</span><span class="sxs-lookup"><span data-stu-id="c4a74-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="c4a74-118">mac</span><span class="sxs-lookup"><span data-stu-id="c4a74-118">mac</span></span>               | <span data-ttu-id="c4a74-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c4a74-119">Int64</span></span>  | <span data-ttu-id="c4a74-120">Число активации на Mac OS.</span><span class="sxs-lookup"><span data-stu-id="c4a74-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="c4a74-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="c4a74-121">windows10Mobile</span></span>   | <span data-ttu-id="c4a74-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c4a74-122">Int64</span></span>  | <span data-ttu-id="c4a74-123">Активация на количество Windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="c4a74-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="c4a74-124">операций ввода-вывода</span><span class="sxs-lookup"><span data-stu-id="c4a74-124">ios</span></span>               | <span data-ttu-id="c4a74-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c4a74-125">Int64</span></span>  | <span data-ttu-id="c4a74-126">Число активации на операций ввода-вывода.</span><span class="sxs-lookup"><span data-stu-id="c4a74-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="c4a74-127">Android (en)</span><span class="sxs-lookup"><span data-stu-id="c4a74-127">android</span></span>           | <span data-ttu-id="c4a74-128">Int64</span><span class="sxs-lookup"><span data-stu-id="c4a74-128">Int64</span></span>  | <span data-ttu-id="c4a74-129">Число активации на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="c4a74-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="c4a74-130">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="c4a74-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="c4a74-131">Логический</span><span class="sxs-lookup"><span data-stu-id="c4a74-131">Boolean</span></span> | <span data-ttu-id="c4a74-132">Значение true, если пользователь продукта на совместно используемый компьютер перед.</span><span class="sxs-lookup"><span data-stu-id="c4a74-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c4a74-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4a74-133">JSON representation</span></span>

<span data-ttu-id="c4a74-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4a74-134">The following is a JSON representation of the resource.</span></span>

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
