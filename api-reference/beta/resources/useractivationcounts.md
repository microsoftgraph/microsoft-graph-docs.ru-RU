---
title: Тип ресурса Усерактиватионкаунтс
description: Ниже указано представление ресурса в формате JSON.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 535355d6be3f6b617d7eb293890aa05a517cfc3b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581284"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="71ad6-103">Тип ресурса Усерактиватионкаунтс</span><span class="sxs-lookup"><span data-stu-id="71ad6-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="71ad6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="71ad6-104">Properties</span></span>

| <span data-ttu-id="71ad6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="71ad6-105">Property</span></span>          | <span data-ttu-id="71ad6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="71ad6-106">Type</span></span>   | <span data-ttu-id="71ad6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="71ad6-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="71ad6-108">Продукттипе</span><span class="sxs-lookup"><span data-stu-id="71ad6-108">productType</span></span>       | <span data-ttu-id="71ad6-109">String</span><span class="sxs-lookup"><span data-stu-id="71ad6-109">String</span></span> | <span data-ttu-id="71ad6-110">Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="71ad6-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="71ad6-111">Ластактиватеддате</span><span class="sxs-lookup"><span data-stu-id="71ad6-111">lastActivatedDate</span></span> | <span data-ttu-id="71ad6-112">Дата</span><span class="sxs-lookup"><span data-stu-id="71ad6-112">Date</span></span>   | <span data-ttu-id="71ad6-113">Дата последней активации.</span><span class="sxs-lookup"><span data-stu-id="71ad6-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="71ad6-114">под</span><span class="sxs-lookup"><span data-stu-id="71ad6-114">windows</span></span>           | <span data-ttu-id="71ad6-115">Int64</span><span class="sxs-lookup"><span data-stu-id="71ad6-115">Int64</span></span>  | <span data-ttu-id="71ad6-116">Счетчик активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="71ad6-116">The activation count on Windows.</span></span> <span data-ttu-id="71ad6-117">Это число включает все активации на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="71ad6-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="71ad6-118">mac</span><span class="sxs-lookup"><span data-stu-id="71ad6-118">mac</span></span>               | <span data-ttu-id="71ad6-119">Int64</span><span class="sxs-lookup"><span data-stu-id="71ad6-119">Int64</span></span>  | <span data-ttu-id="71ad6-120">Число активаций в Mac OS.</span><span class="sxs-lookup"><span data-stu-id="71ad6-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="71ad6-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="71ad6-121">windows10Mobile</span></span>   | <span data-ttu-id="71ad6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="71ad6-122">Int64</span></span>  | <span data-ttu-id="71ad6-123">Счетчик активаций для Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="71ad6-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="71ad6-124">модуле</span><span class="sxs-lookup"><span data-stu-id="71ad6-124">ios</span></span>               | <span data-ttu-id="71ad6-125">Int64</span><span class="sxs-lookup"><span data-stu-id="71ad6-125">Int64</span></span>  | <span data-ttu-id="71ad6-126">Счетчик активаций на iOS.</span><span class="sxs-lookup"><span data-stu-id="71ad6-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="71ad6-127">ОС</span><span class="sxs-lookup"><span data-stu-id="71ad6-127">android</span></span>           | <span data-ttu-id="71ad6-128">Int64</span><span class="sxs-lookup"><span data-stu-id="71ad6-128">Int64</span></span>  | <span data-ttu-id="71ad6-129">Счетчик активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="71ad6-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="71ad6-130">Активатедоншаредкомпутер</span><span class="sxs-lookup"><span data-stu-id="71ad6-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="71ad6-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ad6-131">Boolean</span></span> | <span data-ttu-id="71ad6-132">Имеет значение true, если пользователь использовал продукт на общедоступном компьютере.</span><span class="sxs-lookup"><span data-stu-id="71ad6-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="71ad6-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71ad6-133">JSON representation</span></span>

<span data-ttu-id="71ad6-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71ad6-134">The following is a JSON representation of the resource.</span></span>

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
