---
title: тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 48adb73bac65ddced88aea3edb18deae7653f5b3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761795"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="f086b-103">тип ресурса userActivationCounts</span><span class="sxs-lookup"><span data-stu-id="f086b-103">userActivationCounts resource type</span></span>

<span data-ttu-id="f086b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f086b-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f086b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f086b-105">Properties</span></span>

| <span data-ttu-id="f086b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f086b-106">Property</span></span>          | <span data-ttu-id="f086b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f086b-107">Type</span></span>   | <span data-ttu-id="f086b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f086b-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="f086b-109">productType</span><span class="sxs-lookup"><span data-stu-id="f086b-109">productType</span></span>       | <span data-ttu-id="f086b-110">String</span><span class="sxs-lookup"><span data-stu-id="f086b-110">String</span></span> | <span data-ttu-id="f086b-111">Тип продукта, например "Microsoft 365 ProPlus" или "Project Client".</span><span class="sxs-lookup"><span data-stu-id="f086b-111">The product type, such as "Microsoft 365 ProPlus"or "Project Client".</span></span> |
| <span data-ttu-id="f086b-112">lastActivatedDate</span><span class="sxs-lookup"><span data-stu-id="f086b-112">lastActivatedDate</span></span> | <span data-ttu-id="f086b-113">Дата</span><span class="sxs-lookup"><span data-stu-id="f086b-113">Date</span></span>   | <span data-ttu-id="f086b-114">Дата последней активации.</span><span class="sxs-lookup"><span data-stu-id="f086b-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="f086b-115">Windows</span><span class="sxs-lookup"><span data-stu-id="f086b-115">windows</span></span>           | <span data-ttu-id="f086b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f086b-116">Int64</span></span>  | <span data-ttu-id="f086b-117">Активация рассчитывается на Windows.</span><span class="sxs-lookup"><span data-stu-id="f086b-117">The activation count on Windows.</span></span> <span data-ttu-id="f086b-118">Этот номер включает каждую активацию на любом компьютере Windows.</span><span class="sxs-lookup"><span data-stu-id="f086b-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="f086b-119">mac</span><span class="sxs-lookup"><span data-stu-id="f086b-119">mac</span></span>               | <span data-ttu-id="f086b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f086b-120">Int64</span></span>  | <span data-ttu-id="f086b-121">Активация рассчитывается на ОС Mac.</span><span class="sxs-lookup"><span data-stu-id="f086b-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="f086b-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="f086b-122">windows10Mobile</span></span>   | <span data-ttu-id="f086b-123">Int64</span><span class="sxs-lookup"><span data-stu-id="f086b-123">Int64</span></span>  | <span data-ttu-id="f086b-124">Активация рассчитывается на windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="f086b-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="f086b-125">ios</span><span class="sxs-lookup"><span data-stu-id="f086b-125">ios</span></span>               | <span data-ttu-id="f086b-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f086b-126">Int64</span></span>  | <span data-ttu-id="f086b-127">Активация рассчитывается на iOS.</span><span class="sxs-lookup"><span data-stu-id="f086b-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="f086b-128">Android</span><span class="sxs-lookup"><span data-stu-id="f086b-128">android</span></span>           | <span data-ttu-id="f086b-129">Int64</span><span class="sxs-lookup"><span data-stu-id="f086b-129">Int64</span></span>  | <span data-ttu-id="f086b-130">Активация рассчитывается на устройстве Android.</span><span class="sxs-lookup"><span data-stu-id="f086b-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="f086b-131">activatedOnSharedComputer</span><span class="sxs-lookup"><span data-stu-id="f086b-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="f086b-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="f086b-132">Boolean</span></span> | <span data-ttu-id="f086b-133">True, если пользователь использовал продукт на общем компьютере раньше.</span><span class="sxs-lookup"><span data-stu-id="f086b-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f086b-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f086b-134">JSON representation</span></span>

<span data-ttu-id="f086b-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f086b-135">The following is a JSON representation of the resource.</span></span>

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


