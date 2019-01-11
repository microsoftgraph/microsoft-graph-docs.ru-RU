---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: f57393a538631664be8845fdaeda9f35d07c986f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849310"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="814b6-103">Тип ресурса office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="814b6-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="814b6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="814b6-104">Properties</span></span>

| <span data-ttu-id="814b6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="814b6-105">Property</span></span>                 | <span data-ttu-id="814b6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="814b6-106">Type</span></span>   | <span data-ttu-id="814b6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="814b6-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="814b6-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="814b6-108">reportRefreshDate</span></span>        | <span data-ttu-id="814b6-109">Date</span><span class="sxs-lookup"><span data-stu-id="814b6-109">Date</span></span>   | <span data-ttu-id="814b6-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="814b6-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="814b6-111">productType</span><span class="sxs-lookup"><span data-stu-id="814b6-111">productType</span></span>              | <span data-ttu-id="814b6-112">Строка</span><span class="sxs-lookup"><span data-stu-id="814b6-112">String</span></span> | <span data-ttu-id="814b6-113">Тип продукта, например «Office 365 профессиональный плюс», «Клиент Project», или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="814b6-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="814b6-114">назначенные</span><span class="sxs-lookup"><span data-stu-id="814b6-114">assigned</span></span>                 | <span data-ttu-id="814b6-115">Int64</span><span class="sxs-lookup"><span data-stu-id="814b6-115">Int64</span></span>  | <span data-ttu-id="814b6-116">Число пользователей, которым был назначен для лицензии.</span><span class="sxs-lookup"><span data-stu-id="814b6-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="814b6-117">активирован</span><span class="sxs-lookup"><span data-stu-id="814b6-117">activated</span></span>                | <span data-ttu-id="814b6-118">Int64</span><span class="sxs-lookup"><span data-stu-id="814b6-118">Int64</span></span>  | <span data-ttu-id="814b6-119">Количество пользователей, активации продукта.</span><span class="sxs-lookup"><span data-stu-id="814b6-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="814b6-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="814b6-120">sharedComputerActivation</span></span> | <span data-ttu-id="814b6-121">Int64</span><span class="sxs-lookup"><span data-stu-id="814b6-121">Int64</span></span>  | <span data-ttu-id="814b6-122">Количество пользователей, которые используются продукта на совместно используемый компьютер.</span><span class="sxs-lookup"><span data-stu-id="814b6-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="814b6-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="814b6-123">JSON representation</span></span>

<span data-ttu-id="814b6-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="814b6-124">The following is a JSON representation of the resource.</span></span>

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
