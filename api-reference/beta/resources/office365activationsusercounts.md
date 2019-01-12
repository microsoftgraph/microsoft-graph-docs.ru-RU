---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3dc497e516f95f1e05167703f2b9f8aea6363a64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917722"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="63bae-103">Тип ресурса office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="63bae-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="63bae-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="63bae-104">Properties</span></span>

| <span data-ttu-id="63bae-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="63bae-105">Property</span></span>                 | <span data-ttu-id="63bae-106">Тип</span><span class="sxs-lookup"><span data-stu-id="63bae-106">Type</span></span>   | <span data-ttu-id="63bae-107">Описание</span><span class="sxs-lookup"><span data-stu-id="63bae-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="63bae-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="63bae-108">reportRefreshDate</span></span>        | <span data-ttu-id="63bae-109">Date</span><span class="sxs-lookup"><span data-stu-id="63bae-109">Date</span></span>   | <span data-ttu-id="63bae-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="63bae-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="63bae-111">productType</span><span class="sxs-lookup"><span data-stu-id="63bae-111">productType</span></span>              | <span data-ttu-id="63bae-112">Строка</span><span class="sxs-lookup"><span data-stu-id="63bae-112">String</span></span> | <span data-ttu-id="63bae-113">Тип продукта, например «Office 365 профессиональный плюс», «Клиент Project», или «Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="63bae-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="63bae-114">назначенные</span><span class="sxs-lookup"><span data-stu-id="63bae-114">assigned</span></span>                 | <span data-ttu-id="63bae-115">Int64</span><span class="sxs-lookup"><span data-stu-id="63bae-115">Int64</span></span>  | <span data-ttu-id="63bae-116">Число пользователей, которым был назначен для лицензии.</span><span class="sxs-lookup"><span data-stu-id="63bae-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="63bae-117">активирован</span><span class="sxs-lookup"><span data-stu-id="63bae-117">activated</span></span>                | <span data-ttu-id="63bae-118">Int64</span><span class="sxs-lookup"><span data-stu-id="63bae-118">Int64</span></span>  | <span data-ttu-id="63bae-119">Количество пользователей, активации продукта.</span><span class="sxs-lookup"><span data-stu-id="63bae-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="63bae-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="63bae-120">sharedComputerActivation</span></span> | <span data-ttu-id="63bae-121">Int64</span><span class="sxs-lookup"><span data-stu-id="63bae-121">Int64</span></span>  | <span data-ttu-id="63bae-122">Количество пользователей, которые используются продукта на совместно используемый компьютер.</span><span class="sxs-lookup"><span data-stu-id="63bae-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="63bae-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63bae-123">JSON representation</span></span>

<span data-ttu-id="63bae-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63bae-124">The following is a JSON representation of the resource.</span></span>

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
