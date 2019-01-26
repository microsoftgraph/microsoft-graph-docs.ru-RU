---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d5ed2af02f429f5fd4d6e92b408d2e8e420f4d0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574546"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="73382-103">Тип ресурса office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="73382-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="73382-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="73382-104">Properties</span></span>

| <span data-ttu-id="73382-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="73382-105">Property</span></span>                 | <span data-ttu-id="73382-106">Тип</span><span class="sxs-lookup"><span data-stu-id="73382-106">Type</span></span>   | <span data-ttu-id="73382-107">Описание</span><span class="sxs-lookup"><span data-stu-id="73382-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="73382-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="73382-108">reportRefreshDate</span></span>        | <span data-ttu-id="73382-109">Date</span><span class="sxs-lookup"><span data-stu-id="73382-109">Date</span></span>   | <span data-ttu-id="73382-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="73382-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="73382-111">productType</span><span class="sxs-lookup"><span data-stu-id="73382-111">productType</span></span>              | <span data-ttu-id="73382-112">Строка</span><span class="sxs-lookup"><span data-stu-id="73382-112">String</span></span> | <span data-ttu-id="73382-113">Тип продукта, например «Office 365 профессиональный плюс», «Клиент Project», или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="73382-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="73382-114">назначенные</span><span class="sxs-lookup"><span data-stu-id="73382-114">assigned</span></span>                 | <span data-ttu-id="73382-115">Int64</span><span class="sxs-lookup"><span data-stu-id="73382-115">Int64</span></span>  | <span data-ttu-id="73382-116">Число пользователей, которым был назначен для лицензии.</span><span class="sxs-lookup"><span data-stu-id="73382-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="73382-117">активирован</span><span class="sxs-lookup"><span data-stu-id="73382-117">activated</span></span>                | <span data-ttu-id="73382-118">Int64</span><span class="sxs-lookup"><span data-stu-id="73382-118">Int64</span></span>  | <span data-ttu-id="73382-119">Количество пользователей, активации продукта.</span><span class="sxs-lookup"><span data-stu-id="73382-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="73382-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="73382-120">sharedComputerActivation</span></span> | <span data-ttu-id="73382-121">Int64</span><span class="sxs-lookup"><span data-stu-id="73382-121">Int64</span></span>  | <span data-ttu-id="73382-122">Количество пользователей, которые используются продукта на совместно используемый компьютер.</span><span class="sxs-lookup"><span data-stu-id="73382-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="73382-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73382-123">JSON representation</span></span>

<span data-ttu-id="73382-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73382-124">The following is a JSON representation of the resource.</span></span>

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
