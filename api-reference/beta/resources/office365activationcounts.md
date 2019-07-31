---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: d396ee84e4af6606cfde3e5fc17ef02c0a9594f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966582"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="90c58-103">Тип ресурса office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="90c58-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="90c58-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="90c58-104">Properties</span></span>

| <span data-ttu-id="90c58-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="90c58-105">Property</span></span>          | <span data-ttu-id="90c58-106">Тип</span><span class="sxs-lookup"><span data-stu-id="90c58-106">Type</span></span>   | <span data-ttu-id="90c58-107">Описание</span><span class="sxs-lookup"><span data-stu-id="90c58-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="90c58-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="90c58-108">reportRefreshDate</span></span> | <span data-ttu-id="90c58-109">Дата</span><span class="sxs-lookup"><span data-stu-id="90c58-109">Date</span></span>   | <span data-ttu-id="90c58-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="90c58-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="90c58-111">Продукттипе</span><span class="sxs-lookup"><span data-stu-id="90c58-111">productType</span></span>       | <span data-ttu-id="90c58-112">String</span><span class="sxs-lookup"><span data-stu-id="90c58-112">String</span></span> | <span data-ttu-id="90c58-113">Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="90c58-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="90c58-114">под</span><span class="sxs-lookup"><span data-stu-id="90c58-114">windows</span></span>           | <span data-ttu-id="90c58-115">Int64</span><span class="sxs-lookup"><span data-stu-id="90c58-115">Int64</span></span>  | <span data-ttu-id="90c58-116">Счетчик активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="90c58-116">The activation count on Windows.</span></span> <span data-ttu-id="90c58-117">Это число включает все активации на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="90c58-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="90c58-118">mac</span><span class="sxs-lookup"><span data-stu-id="90c58-118">mac</span></span>               | <span data-ttu-id="90c58-119">Int64</span><span class="sxs-lookup"><span data-stu-id="90c58-119">Int64</span></span>  | <span data-ttu-id="90c58-120">Число активаций в Mac OS.</span><span class="sxs-lookup"><span data-stu-id="90c58-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="90c58-121">ОС</span><span class="sxs-lookup"><span data-stu-id="90c58-121">android</span></span>           | <span data-ttu-id="90c58-122">Int64</span><span class="sxs-lookup"><span data-stu-id="90c58-122">Int64</span></span>  | <span data-ttu-id="90c58-123">Счетчик активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="90c58-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="90c58-124">модуле</span><span class="sxs-lookup"><span data-stu-id="90c58-124">ios</span></span>               | <span data-ttu-id="90c58-125">Int64</span><span class="sxs-lookup"><span data-stu-id="90c58-125">Int64</span></span>  | <span data-ttu-id="90c58-126">Счетчик активаций на iOS.</span><span class="sxs-lookup"><span data-stu-id="90c58-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="90c58-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="90c58-127">windows10Mobile</span></span>   | <span data-ttu-id="90c58-128">Int64</span><span class="sxs-lookup"><span data-stu-id="90c58-128">Int64</span></span>  | <span data-ttu-id="90c58-129">Счетчик активаций для Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="90c58-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="90c58-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90c58-130">JSON representation</span></span>

<span data-ttu-id="90c58-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90c58-131">The following is a JSON representation of the resource.</span></span>

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
