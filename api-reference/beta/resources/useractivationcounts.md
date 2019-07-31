---
title: Тип ресурса Усерактиватионкаунтс
description: Ниже указано представление ресурса в формате JSON.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9c1dbbaa6a429a90a54f8af5f3b380ff58c86dab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007496"
---
# <a name="useractivationcounts-resource-type"></a><span data-ttu-id="2322f-103">Тип ресурса Усерактиватионкаунтс</span><span class="sxs-lookup"><span data-stu-id="2322f-103">userActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2322f-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="2322f-104">Properties</span></span>

| <span data-ttu-id="2322f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="2322f-105">Property</span></span>          | <span data-ttu-id="2322f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="2322f-106">Type</span></span>   | <span data-ttu-id="2322f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="2322f-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2322f-108">Продукттипе</span><span class="sxs-lookup"><span data-stu-id="2322f-108">productType</span></span>       | <span data-ttu-id="2322f-109">String</span><span class="sxs-lookup"><span data-stu-id="2322f-109">String</span></span> | <span data-ttu-id="2322f-110">Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="2322f-110">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="2322f-111">Ластактиватеддате</span><span class="sxs-lookup"><span data-stu-id="2322f-111">lastActivatedDate</span></span> | <span data-ttu-id="2322f-112">Дата</span><span class="sxs-lookup"><span data-stu-id="2322f-112">Date</span></span>   | <span data-ttu-id="2322f-113">Дата последней активации.</span><span class="sxs-lookup"><span data-stu-id="2322f-113">The date of the latest activation.</span></span>       |
| <span data-ttu-id="2322f-114">под</span><span class="sxs-lookup"><span data-stu-id="2322f-114">windows</span></span>           | <span data-ttu-id="2322f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2322f-115">Int64</span></span>  | <span data-ttu-id="2322f-116">Счетчик активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="2322f-116">The activation count on Windows.</span></span> <span data-ttu-id="2322f-117">Это число включает все активации на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="2322f-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="2322f-118">mac</span><span class="sxs-lookup"><span data-stu-id="2322f-118">mac</span></span>               | <span data-ttu-id="2322f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="2322f-119">Int64</span></span>  | <span data-ttu-id="2322f-120">Число активаций в Mac OS.</span><span class="sxs-lookup"><span data-stu-id="2322f-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="2322f-121">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="2322f-121">windows10Mobile</span></span>   | <span data-ttu-id="2322f-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2322f-122">Int64</span></span>  | <span data-ttu-id="2322f-123">Счетчик активаций для Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="2322f-123">The activation count on Windows 10 mobile.</span></span> |
| <span data-ttu-id="2322f-124">модуле</span><span class="sxs-lookup"><span data-stu-id="2322f-124">ios</span></span>               | <span data-ttu-id="2322f-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2322f-125">Int64</span></span>  | <span data-ttu-id="2322f-126">Счетчик активаций на iOS.</span><span class="sxs-lookup"><span data-stu-id="2322f-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="2322f-127">ОС</span><span class="sxs-lookup"><span data-stu-id="2322f-127">android</span></span>           | <span data-ttu-id="2322f-128">Int64</span><span class="sxs-lookup"><span data-stu-id="2322f-128">Int64</span></span>  | <span data-ttu-id="2322f-129">Счетчик активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="2322f-129">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="2322f-130">Активатедоншаредкомпутер</span><span class="sxs-lookup"><span data-stu-id="2322f-130">activatedOnSharedComputer</span></span>   | <span data-ttu-id="2322f-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="2322f-131">Boolean</span></span> | <span data-ttu-id="2322f-132">Имеет значение true, если пользователь использовал продукт на общедоступном компьютере.</span><span class="sxs-lookup"><span data-stu-id="2322f-132">True if the user used the product on a shared computer before.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2322f-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2322f-133">JSON representation</span></span>

<span data-ttu-id="2322f-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2322f-134">The following is a JSON representation of the resource.</span></span>

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
