---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 90d9d2d8616f166eb9d8b87967898daa0468db54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081406"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="d9d1b-103">Тип ресурса office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="d9d1b-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d9d1b-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9d1b-104">Properties</span></span>

| <span data-ttu-id="d9d1b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9d1b-105">Property</span></span>                 | <span data-ttu-id="d9d1b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d9d1b-106">Type</span></span>   | <span data-ttu-id="d9d1b-107">Description</span><span class="sxs-lookup"><span data-stu-id="d9d1b-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d9d1b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d9d1b-108">reportRefreshDate</span></span>        | <span data-ttu-id="d9d1b-109">Date</span><span class="sxs-lookup"><span data-stu-id="d9d1b-109">Date</span></span>   | <span data-ttu-id="d9d1b-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="d9d1b-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d9d1b-111">productType</span><span class="sxs-lookup"><span data-stu-id="d9d1b-111">productType</span></span>              | <span data-ttu-id="d9d1b-112">String</span><span class="sxs-lookup"><span data-stu-id="d9d1b-112">String</span></span> | <span data-ttu-id="d9d1b-113">Тип продукта, например «Office 365 профессиональный плюс», «Клиент Project», или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="d9d1b-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="d9d1b-114">назначенные</span><span class="sxs-lookup"><span data-stu-id="d9d1b-114">assigned</span></span>                 | <span data-ttu-id="d9d1b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d9d1b-115">Int64</span></span>  | <span data-ttu-id="d9d1b-116">Число пользователей, которым был назначен для лицензии.</span><span class="sxs-lookup"><span data-stu-id="d9d1b-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="d9d1b-117">активирован</span><span class="sxs-lookup"><span data-stu-id="d9d1b-117">activated</span></span>                | <span data-ttu-id="d9d1b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d9d1b-118">Int64</span></span>  | <span data-ttu-id="d9d1b-119">Количество пользователей, активации продукта.</span><span class="sxs-lookup"><span data-stu-id="d9d1b-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="d9d1b-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="d9d1b-120">sharedComputerActivation</span></span> | <span data-ttu-id="d9d1b-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d9d1b-121">Int64</span></span>  | <span data-ttu-id="d9d1b-122">Количество пользователей, которые используются продукта на совместно используемый компьютер.</span><span class="sxs-lookup"><span data-stu-id="d9d1b-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d9d1b-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9d1b-123">JSON representation</span></span>

<span data-ttu-id="d9d1b-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9d1b-124">The following is a JSON representation of the resource.</span></span>

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
