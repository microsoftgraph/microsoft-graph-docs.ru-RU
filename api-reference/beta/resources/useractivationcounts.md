---
title: Тип ресурса Усерактиватионкаунтс
description: Ниже указано представление ресурса в формате JSON.
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91366f9d2b2308c997c111123d856581db7c00c6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384956"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="2550a-103">Тип ресурса Усерактиватионкаунтс</span><span class="sxs-lookup"><span data-stu-id="2550a-103">userActivationCounts resource type</span></span>

<span data-ttu-id="2550a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2550a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2550a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2550a-105">Properties</span></span>

| <span data-ttu-id="2550a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2550a-106">Property</span></span>          | <span data-ttu-id="2550a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2550a-107">Type</span></span>   | <span data-ttu-id="2550a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2550a-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2550a-109">продукттипе</span><span class="sxs-lookup"><span data-stu-id="2550a-109">productType</span></span>       | <span data-ttu-id="2550a-110">String</span><span class="sxs-lookup"><span data-stu-id="2550a-110">String</span></span> | <span data-ttu-id="2550a-111">Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="2550a-111">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="2550a-112">ластактиватеддате</span><span class="sxs-lookup"><span data-stu-id="2550a-112">lastActivatedDate</span></span> | <span data-ttu-id="2550a-113">Дата</span><span class="sxs-lookup"><span data-stu-id="2550a-113">Date</span></span>   | <span data-ttu-id="2550a-114">Дата последней активации.</span><span class="sxs-lookup"><span data-stu-id="2550a-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="2550a-115">под</span><span class="sxs-lookup"><span data-stu-id="2550a-115">windows</span></span>           | <span data-ttu-id="2550a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2550a-116">Int64</span></span>  | <span data-ttu-id="2550a-117">Счетчик активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="2550a-117">The activation count on Windows.</span></span> <span data-ttu-id="2550a-118">Это число включает все активации на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="2550a-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="2550a-119">mac</span><span class="sxs-lookup"><span data-stu-id="2550a-119">mac</span></span>               | <span data-ttu-id="2550a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2550a-120">Int64</span></span>  | <span data-ttu-id="2550a-121">Число активаций в Mac OS.</span><span class="sxs-lookup"><span data-stu-id="2550a-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="2550a-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="2550a-122">windows10Mobile</span></span>   | <span data-ttu-id="2550a-123">Int64</span><span class="sxs-lookup"><span data-stu-id="2550a-123">Int64</span></span>  | <span data-ttu-id="2550a-124">Счетчик активаций для Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="2550a-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="2550a-125">модуле</span><span class="sxs-lookup"><span data-stu-id="2550a-125">ios</span></span>               | <span data-ttu-id="2550a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="2550a-126">Int64</span></span>  | <span data-ttu-id="2550a-127">Счетчик активаций на iOS.</span><span class="sxs-lookup"><span data-stu-id="2550a-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="2550a-128">ОС</span><span class="sxs-lookup"><span data-stu-id="2550a-128">android</span></span>           | <span data-ttu-id="2550a-129">Int64</span><span class="sxs-lookup"><span data-stu-id="2550a-129">Int64</span></span>  | <span data-ttu-id="2550a-130">Счетчик активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="2550a-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="2550a-131">активатедоншаредкомпутер</span><span class="sxs-lookup"><span data-stu-id="2550a-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="2550a-132">Логическое</span><span class="sxs-lookup"><span data-stu-id="2550a-132">Boolean</span></span> | <span data-ttu-id="2550a-133">Имеет значение true, если пользователь использовал продукт на общедоступном компьютере.</span><span class="sxs-lookup"><span data-stu-id="2550a-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2550a-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2550a-134">JSON representation</span></span>

<span data-ttu-id="2550a-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2550a-135">The following is a JSON representation of the resource.</span></span>

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
