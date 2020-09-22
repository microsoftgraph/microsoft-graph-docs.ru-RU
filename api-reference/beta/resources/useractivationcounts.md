---
title: Тип ресурса Усерактиватионкаунтс
description: Ниже указано представление ресурса в формате JSON.
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d81e8078d785761c09aa1070120924b2318415a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057887"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="357ed-103">Тип ресурса Усерактиватионкаунтс</span><span class="sxs-lookup"><span data-stu-id="357ed-103">userActivationCounts resource type</span></span>

<span data-ttu-id="357ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="357ed-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="357ed-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="357ed-105">Properties</span></span>

| <span data-ttu-id="357ed-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="357ed-106">Property</span></span>          | <span data-ttu-id="357ed-107">Тип</span><span class="sxs-lookup"><span data-stu-id="357ed-107">Type</span></span>   | <span data-ttu-id="357ed-108">Описание</span><span class="sxs-lookup"><span data-stu-id="357ed-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="357ed-109">продукттипе</span><span class="sxs-lookup"><span data-stu-id="357ed-109">productType</span></span>       | <span data-ttu-id="357ed-110">String</span><span class="sxs-lookup"><span data-stu-id="357ed-110">String</span></span> | <span data-ttu-id="357ed-111">Тип продукта, например "Microsoft 365 профессиональный плюс" или "клиент Project".</span><span class="sxs-lookup"><span data-stu-id="357ed-111">The product type, such as "Microsoft 365 ProPlus"or "Project Client".</span></span> |
| <span data-ttu-id="357ed-112">ластактиватеддате</span><span class="sxs-lookup"><span data-stu-id="357ed-112">lastActivatedDate</span></span> | <span data-ttu-id="357ed-113">Дата</span><span class="sxs-lookup"><span data-stu-id="357ed-113">Date</span></span>   | <span data-ttu-id="357ed-114">Дата последней активации.</span><span class="sxs-lookup"><span data-stu-id="357ed-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="357ed-115">под</span><span class="sxs-lookup"><span data-stu-id="357ed-115">windows</span></span>           | <span data-ttu-id="357ed-116">Int64</span><span class="sxs-lookup"><span data-stu-id="357ed-116">Int64</span></span>  | <span data-ttu-id="357ed-117">Счетчик активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="357ed-117">The activation count on Windows.</span></span> <span data-ttu-id="357ed-118">Это число включает все активации на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="357ed-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="357ed-119">mac</span><span class="sxs-lookup"><span data-stu-id="357ed-119">mac</span></span>               | <span data-ttu-id="357ed-120">Int64</span><span class="sxs-lookup"><span data-stu-id="357ed-120">Int64</span></span>  | <span data-ttu-id="357ed-121">Число активаций в Mac OS.</span><span class="sxs-lookup"><span data-stu-id="357ed-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="357ed-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="357ed-122">windows10Mobile</span></span>   | <span data-ttu-id="357ed-123">Int64</span><span class="sxs-lookup"><span data-stu-id="357ed-123">Int64</span></span>  | <span data-ttu-id="357ed-124">Счетчик активаций для Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="357ed-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="357ed-125">модуле</span><span class="sxs-lookup"><span data-stu-id="357ed-125">ios</span></span>               | <span data-ttu-id="357ed-126">Int64</span><span class="sxs-lookup"><span data-stu-id="357ed-126">Int64</span></span>  | <span data-ttu-id="357ed-127">Счетчик активаций на iOS.</span><span class="sxs-lookup"><span data-stu-id="357ed-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="357ed-128">ОС</span><span class="sxs-lookup"><span data-stu-id="357ed-128">android</span></span>           | <span data-ttu-id="357ed-129">Int64</span><span class="sxs-lookup"><span data-stu-id="357ed-129">Int64</span></span>  | <span data-ttu-id="357ed-130">Счетчик активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="357ed-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="357ed-131">активатедоншаредкомпутер</span><span class="sxs-lookup"><span data-stu-id="357ed-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="357ed-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="357ed-132">Boolean</span></span> | <span data-ttu-id="357ed-133">Имеет значение true, если пользователь использовал продукт на общедоступном компьютере.</span><span class="sxs-lookup"><span data-stu-id="357ed-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="357ed-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="357ed-134">JSON representation</span></span>

<span data-ttu-id="357ed-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="357ed-135">The following is a JSON representation of the resource.</span></span>

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


