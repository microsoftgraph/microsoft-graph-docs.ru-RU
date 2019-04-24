---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7bc21be693a5c68ecd5c6a1e4e44d53c9261acdb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505468"
---
# <a name="office365activationcounts-resource-type"></a><span data-ttu-id="11736-103">Тип ресурса office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="11736-103">office365ActivationCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="11736-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="11736-104">Properties</span></span>

| <span data-ttu-id="11736-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="11736-105">Property</span></span>          | <span data-ttu-id="11736-106">Тип</span><span class="sxs-lookup"><span data-stu-id="11736-106">Type</span></span>   | <span data-ttu-id="11736-107">Описание</span><span class="sxs-lookup"><span data-stu-id="11736-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="11736-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="11736-108">reportRefreshDate</span></span> | <span data-ttu-id="11736-109">Дата</span><span class="sxs-lookup"><span data-stu-id="11736-109">Date</span></span>   | <span data-ttu-id="11736-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="11736-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="11736-111">Продукттипе</span><span class="sxs-lookup"><span data-stu-id="11736-111">productType</span></span>       | <span data-ttu-id="11736-112">String</span><span class="sxs-lookup"><span data-stu-id="11736-112">String</span></span> | <span data-ttu-id="11736-113">Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="11736-113">The product type, such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="11736-114">под</span><span class="sxs-lookup"><span data-stu-id="11736-114">windows</span></span>           | <span data-ttu-id="11736-115">Int64</span><span class="sxs-lookup"><span data-stu-id="11736-115">Int64</span></span>  | <span data-ttu-id="11736-116">Счетчик активаций в Windows.</span><span class="sxs-lookup"><span data-stu-id="11736-116">The activation count on Windows.</span></span> <span data-ttu-id="11736-117">Это число включает все активации на любом компьютере с Windows.</span><span class="sxs-lookup"><span data-stu-id="11736-117">This number includes every activation on any Windows computer.</span></span> |
| <span data-ttu-id="11736-118">mac</span><span class="sxs-lookup"><span data-stu-id="11736-118">mac</span></span>               | <span data-ttu-id="11736-119">Int64</span><span class="sxs-lookup"><span data-stu-id="11736-119">Int64</span></span>  | <span data-ttu-id="11736-120">Число активаций в Mac OS.</span><span class="sxs-lookup"><span data-stu-id="11736-120">The activation count on Mac OS.</span></span>          |
| <span data-ttu-id="11736-121">ОС</span><span class="sxs-lookup"><span data-stu-id="11736-121">android</span></span>           | <span data-ttu-id="11736-122">Int64</span><span class="sxs-lookup"><span data-stu-id="11736-122">Int64</span></span>  | <span data-ttu-id="11736-123">Счетчик активаций на устройстве с Android.</span><span class="sxs-lookup"><span data-stu-id="11736-123">The activation count on an Android device.</span></span>  |
| <span data-ttu-id="11736-124">модуле</span><span class="sxs-lookup"><span data-stu-id="11736-124">ios</span></span>               | <span data-ttu-id="11736-125">Int64</span><span class="sxs-lookup"><span data-stu-id="11736-125">Int64</span></span>  | <span data-ttu-id="11736-126">Счетчик активаций на iOS.</span><span class="sxs-lookup"><span data-stu-id="11736-126">The activation count on iOS.</span></span>             |
| <span data-ttu-id="11736-127">windows10Mobile</span><span class="sxs-lookup"><span data-stu-id="11736-127">windows10Mobile</span></span>   | <span data-ttu-id="11736-128">Int64</span><span class="sxs-lookup"><span data-stu-id="11736-128">Int64</span></span>  | <span data-ttu-id="11736-129">Счетчик активаций для Windows 10 Mobile.</span><span class="sxs-lookup"><span data-stu-id="11736-129">The activation count on Windows 10 mobile.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="11736-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11736-130">JSON representation</span></span>

<span data-ttu-id="11736-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11736-131">The following is a JSON representation of the resource.</span></span>

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
