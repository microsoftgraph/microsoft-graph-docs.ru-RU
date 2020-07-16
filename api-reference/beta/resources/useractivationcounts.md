---
title: Тип ресурса Усерактиватионкаунтс
description: Ниже указано представление ресурса в формате JSON.
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6433c1680630b5805cd18a22e550e58a51bcefbc
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898305"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="d3d39-103">Тип ресурса Усерактиватионкаунтс</span><span class="sxs-lookup"><span data-stu-id="d3d39-103">userActivationCounts resource type</span></span>

<span data-ttu-id="d3d39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3d39-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d3d39-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3d39-105">Properties</span></span>

| <span data-ttu-id="d3d39-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3d39-106">Property</span></span>          | <span data-ttu-id="d3d39-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d3d39-107">Type</span></span>   | <span data-ttu-id="d3d39-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d3d39-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d3d39-109">продукттипе</span><span class="sxs-lookup"><span data-stu-id="d3d39-109">productType</span></span>       | <span data-ttu-id="d3d39-110">String</span><span class="sxs-lookup"><span data-stu-id="d3d39-110">String</span></span> | <span data-ttu-id="d3d39-111">Тип продукта, например "Microsoft 365 профессиональный плюс" или "клиент Project".</span><span class="sxs-lookup"><span data-stu-id="d3d39-111">The product type, such as "Microsoft 365 ProPlus"or "Project Client".</span></span> |
| <span data-ttu-id="d3d39-112">ластактиватеддате</span><span class="sxs-lookup"><span data-stu-id="d3d39-112">lastActivatedDate</span></span> | <span data-ttu-id="d3d39-113">Дата</span><span class="sxs-lookup"><span data-stu-id="d3d39-113">Date</span></span>   | <span data-ttu-id="d3d39-114">Дата последней активации.</span><span class="sxs-lookup"><span data-stu-id="d3d39-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="d3d39-115">под</span><span class="sxs-lookup"><span data-stu-id="d3d39-115">windows</span></span>           | <span data-ttu-id="d3d39-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d3d39-116">Int64</span></span>  | <span data-ttu-id="d3d39-117">Счетчик активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="d3d39-117">The activation count on Windows.</span></span> <span data-ttu-id="d3d39-118">Это число включает все активации на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="d3d39-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="d3d39-119">mac</span><span class="sxs-lookup"><span data-stu-id="d3d39-119">mac</span></span>               | <span data-ttu-id="d3d39-120">Int64</span><span class="sxs-lookup"><span data-stu-id="d3d39-120">Int64</span></span>  | <span data-ttu-id="d3d39-121">Число активаций в Mac OS.</span><span class="sxs-lookup"><span data-stu-id="d3d39-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="d3d39-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="d3d39-122">windows10Mobile</span></span>   | <span data-ttu-id="d3d39-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d3d39-123">Int64</span></span>  | <span data-ttu-id="d3d39-124">Счетчик активаций для Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="d3d39-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="d3d39-125">модуле</span><span class="sxs-lookup"><span data-stu-id="d3d39-125">ios</span></span>               | <span data-ttu-id="d3d39-126">Int64</span><span class="sxs-lookup"><span data-stu-id="d3d39-126">Int64</span></span>  | <span data-ttu-id="d3d39-127">Счетчик активаций на iOS.</span><span class="sxs-lookup"><span data-stu-id="d3d39-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="d3d39-128">ОС</span><span class="sxs-lookup"><span data-stu-id="d3d39-128">android</span></span>           | <span data-ttu-id="d3d39-129">Int64</span><span class="sxs-lookup"><span data-stu-id="d3d39-129">Int64</span></span>  | <span data-ttu-id="d3d39-130">Счетчик активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="d3d39-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="d3d39-131">активатедоншаредкомпутер</span><span class="sxs-lookup"><span data-stu-id="d3d39-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="d3d39-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3d39-132">Boolean</span></span> | <span data-ttu-id="d3d39-133">Имеет значение true, если пользователь использовал продукт на общедоступном компьютере.</span><span class="sxs-lookup"><span data-stu-id="d3d39-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3d39-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d3d39-134">JSON representation</span></span>

<span data-ttu-id="d3d39-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3d39-135">The following is a JSON representation of the resource.</span></span>

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
