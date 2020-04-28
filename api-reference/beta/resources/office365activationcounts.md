---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 1a45aa058a5186e87d11eed5199b51abf709879b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522493"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="7b5a2-103">Тип ресурса office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="7b5a2-103">office365ActivationCounts resource type</span></span>

<span data-ttu-id="7b5a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b5a2-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="7b5a2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b5a2-105">Properties</span></span>

| <span data-ttu-id="7b5a2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b5a2-106">Property</span></span>          | <span data-ttu-id="7b5a2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7b5a2-107">Type</span></span>   | <span data-ttu-id="7b5a2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7b5a2-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="7b5a2-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="7b5a2-109">reportRefreshDate</span></span> | <span data-ttu-id="7b5a2-110">Дата</span><span class="sxs-lookup"><span data-stu-id="7b5a2-110">Date</span></span>   | <span data-ttu-id="7b5a2-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="7b5a2-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="7b5a2-112">продукттипе</span><span class="sxs-lookup"><span data-stu-id="7b5a2-112">productType</span></span>       | <span data-ttu-id="7b5a2-113">String</span><span class="sxs-lookup"><span data-stu-id="7b5a2-113">String</span></span> | <span data-ttu-id="7b5a2-114">Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="7b5a2-114">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="7b5a2-115">под</span><span class="sxs-lookup"><span data-stu-id="7b5a2-115">windows</span></span>           | <span data-ttu-id="7b5a2-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7b5a2-116">Int64</span></span>  | <span data-ttu-id="7b5a2-117">Счетчик активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="7b5a2-117">The activation count on Windows.</span></span> <span data-ttu-id="7b5a2-118">Это число включает все активации на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="7b5a2-118">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="7b5a2-119">mac</span><span class="sxs-lookup"><span data-stu-id="7b5a2-119">mac</span></span>               | <span data-ttu-id="7b5a2-120">Int64</span><span class="sxs-lookup"><span data-stu-id="7b5a2-120">Int64</span></span>  | <span data-ttu-id="7b5a2-121">Число активаций в Mac OS.</span><span class="sxs-lookup"><span data-stu-id="7b5a2-121">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="7b5a2-122">ОС</span><span class="sxs-lookup"><span data-stu-id="7b5a2-122">android</span></span>           | <span data-ttu-id="7b5a2-123">Int64</span><span class="sxs-lookup"><span data-stu-id="7b5a2-123">Int64</span></span>  | <span data-ttu-id="7b5a2-124">Счетчик активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="7b5a2-124">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="7b5a2-125">модуле</span><span class="sxs-lookup"><span data-stu-id="7b5a2-125">ios</span></span>               | <span data-ttu-id="7b5a2-126">Int64</span><span class="sxs-lookup"><span data-stu-id="7b5a2-126">Int64</span></span>  | <span data-ttu-id="7b5a2-127">Счетчик активаций на iOS.</span><span class="sxs-lookup"><span data-stu-id="7b5a2-127">The activation count on iOS.</span></span>             |
| <span data-ttu-id="7b5a2-128">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="7b5a2-128">windows10Mobile</span></span>   | <span data-ttu-id="7b5a2-129">Int64</span><span class="sxs-lookup"><span data-stu-id="7b5a2-129">Int64</span></span>  | <span data-ttu-id="7b5a2-130">Счетчик активаций для Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="7b5a2-130">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b5a2-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b5a2-131">JSON representation</span></span>

<span data-ttu-id="7b5a2-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b5a2-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
