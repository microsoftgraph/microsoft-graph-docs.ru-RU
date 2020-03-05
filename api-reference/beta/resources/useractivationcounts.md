---
title: Тип ресурса Усерактиватионкаунтс
description: Ниже указано представление ресурса в формате JSON.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 65554254260d640638e7cbbbb2d0a0076e209f22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519549"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="265dc-103">Тип ресурса Усерактиватионкаунтс</span><span class="sxs-lookup"><span data-stu-id="265dc-103">userActivationCounts resource type</span></span>

<span data-ttu-id="265dc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="265dc-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="265dc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="265dc-105">Properties</span></span>

| <span data-ttu-id="265dc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="265dc-106">Property</span></span>          | <span data-ttu-id="265dc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="265dc-107">Type</span></span>   | <span data-ttu-id="265dc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="265dc-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="265dc-109">продукттипе</span><span class="sxs-lookup"><span data-stu-id="265dc-109">productType</span></span>       | <span data-ttu-id="265dc-110">String</span><span class="sxs-lookup"><span data-stu-id="265dc-110">String</span></span> | <span data-ttu-id="265dc-111">Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="265dc-111">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="265dc-112">ластактиватеддате</span><span class="sxs-lookup"><span data-stu-id="265dc-112">lastActivatedDate</span></span> | <span data-ttu-id="265dc-113">Дата</span><span class="sxs-lookup"><span data-stu-id="265dc-113">Date</span></span>   | <span data-ttu-id="265dc-114">Дата последней активации.</span><span class="sxs-lookup"><span data-stu-id="265dc-114">The date of the latest activation.</span></span>       |
| <span data-ttu-id="265dc-115">под</span><span class="sxs-lookup"><span data-stu-id="265dc-115">windows</span></span>           | <span data-ttu-id="265dc-116">Int64</span><span class="sxs-lookup"><span data-stu-id="265dc-116">Int64</span></span>  | <span data-ttu-id="265dc-117">Счетчик активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="265dc-117">The activation count on Windows.</span></span> <span data-ttu-id="265dc-118">Это число включает все активации на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="265dc-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="265dc-119">mac</span><span class="sxs-lookup"><span data-stu-id="265dc-119">mac</span></span>               | <span data-ttu-id="265dc-120">Int64</span><span class="sxs-lookup"><span data-stu-id="265dc-120">Int64</span></span>  | <span data-ttu-id="265dc-121">Число активаций в Mac OS.</span><span class="sxs-lookup"><span data-stu-id="265dc-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="265dc-122">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="265dc-122">windows10Mobile</span></span>   | <span data-ttu-id="265dc-123">Int64</span><span class="sxs-lookup"><span data-stu-id="265dc-123">Int64</span></span>  | <span data-ttu-id="265dc-124">Счетчик активаций для Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="265dc-124">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="265dc-125">модуле</span><span class="sxs-lookup"><span data-stu-id="265dc-125">ios</span></span>               | <span data-ttu-id="265dc-126">Int64</span><span class="sxs-lookup"><span data-stu-id="265dc-126">Int64</span></span>  | <span data-ttu-id="265dc-127">Счетчик активаций на iOS.</span><span class="sxs-lookup"><span data-stu-id="265dc-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="265dc-128">ОС</span><span class="sxs-lookup"><span data-stu-id="265dc-128">android</span></span>           | <span data-ttu-id="265dc-129">Int64</span><span class="sxs-lookup"><span data-stu-id="265dc-129">Int64</span></span>  | <span data-ttu-id="265dc-130">Счетчик активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="265dc-130">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="265dc-131">активатедоншаредкомпутер</span><span class="sxs-lookup"><span data-stu-id="265dc-131">activatedOnSharedComputer</span></span>   | <span data-ttu-id="265dc-132">Логический</span><span class="sxs-lookup"><span data-stu-id="265dc-132">Boolean</span></span> | <span data-ttu-id="265dc-133">Имеет значение true, если пользователь использовал продукт на общедоступном компьютере.</span><span class="sxs-lookup"><span data-stu-id="265dc-133">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="265dc-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="265dc-134">JSON representation</span></span>

<span data-ttu-id="265dc-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="265dc-135">The following is a JSON representation of the resource.</span></span>

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
