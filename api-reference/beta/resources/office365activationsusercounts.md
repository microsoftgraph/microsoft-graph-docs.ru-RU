---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: a6b97aa8b74ad51158c151e9d3723ea5d1ef191b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980754"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="ff0a0-103">Тип ресурса office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="ff0a0-103">office365ActivationsUserCounts resource type</span></span>

<span data-ttu-id="ff0a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff0a0-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="ff0a0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff0a0-105">Properties</span></span>

| <span data-ttu-id="ff0a0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff0a0-106">Property</span></span>                 | <span data-ttu-id="ff0a0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ff0a0-107">Type</span></span>   | <span data-ttu-id="ff0a0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ff0a0-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="ff0a0-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ff0a0-109">reportRefreshDate</span></span>        | <span data-ttu-id="ff0a0-110">Дата</span><span class="sxs-lookup"><span data-stu-id="ff0a0-110">Date</span></span>   | <span data-ttu-id="ff0a0-111">Последняя дата содержимого.</span><span class="sxs-lookup"><span data-stu-id="ff0a0-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="ff0a0-112">productType</span><span class="sxs-lookup"><span data-stu-id="ff0a0-112">productType</span></span>              | <span data-ttu-id="ff0a0-113">String</span><span class="sxs-lookup"><span data-stu-id="ff0a0-113">String</span></span> | <span data-ttu-id="ff0a0-114">Тип продукта, такой как "Microsoft 365 профессиональныйplus" или "Project Client".</span><span class="sxs-lookup"><span data-stu-id="ff0a0-114">The product type such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="ff0a0-115">assigned</span><span class="sxs-lookup"><span data-stu-id="ff0a0-115">assigned</span></span>                 | <span data-ttu-id="ff0a0-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ff0a0-116">Int64</span></span>  | <span data-ttu-id="ff0a0-117">Количество пользователей, которые были назначены лицензии на продукт.</span><span class="sxs-lookup"><span data-stu-id="ff0a0-117">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="ff0a0-118">activated</span><span class="sxs-lookup"><span data-stu-id="ff0a0-118">activated</span></span>                | <span data-ttu-id="ff0a0-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ff0a0-119">Int64</span></span>  | <span data-ttu-id="ff0a0-120">Количество пользователей, активировавших продукт.</span><span class="sxs-lookup"><span data-stu-id="ff0a0-120">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="ff0a0-121">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="ff0a0-121">sharedComputerActivation</span></span> | <span data-ttu-id="ff0a0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ff0a0-122">Int64</span></span>  | <span data-ttu-id="ff0a0-123">Количество пользователей, которые использовали продукт на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="ff0a0-123">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff0a0-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff0a0-124">JSON representation</span></span>

<span data-ttu-id="ff0a0-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff0a0-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```


