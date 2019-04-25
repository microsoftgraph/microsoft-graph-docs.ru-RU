---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d5ed2af02f429f5fd4d6e92b408d2e8e420f4d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581515"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="42c3d-103">Тип ресурса office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="42c3d-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="42c3d-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="42c3d-104">Properties</span></span>

| <span data-ttu-id="42c3d-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="42c3d-105">Property</span></span>                 | <span data-ttu-id="42c3d-106">Тип</span><span class="sxs-lookup"><span data-stu-id="42c3d-106">Type</span></span>   | <span data-ttu-id="42c3d-107">Описание</span><span class="sxs-lookup"><span data-stu-id="42c3d-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="42c3d-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="42c3d-108">reportRefreshDate</span></span>        | <span data-ttu-id="42c3d-109">Дата</span><span class="sxs-lookup"><span data-stu-id="42c3d-109">Date</span></span>   | <span data-ttu-id="42c3d-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="42c3d-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="42c3d-111">Продукттипе</span><span class="sxs-lookup"><span data-stu-id="42c3d-111">productType</span></span>              | <span data-ttu-id="42c3d-112">String</span><span class="sxs-lookup"><span data-stu-id="42c3d-112">String</span></span> | <span data-ttu-id="42c3d-113">Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="42c3d-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="42c3d-114">ей</span><span class="sxs-lookup"><span data-stu-id="42c3d-114">assigned</span></span>                 | <span data-ttu-id="42c3d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="42c3d-115">Int64</span></span>  | <span data-ttu-id="42c3d-116">Количество пользователей, которым назначена лицензия на продукт.</span><span class="sxs-lookup"><span data-stu-id="42c3d-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="42c3d-117">активной</span><span class="sxs-lookup"><span data-stu-id="42c3d-117">activated</span></span>                | <span data-ttu-id="42c3d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="42c3d-118">Int64</span></span>  | <span data-ttu-id="42c3d-119">Количество пользователей, которые активировали продукт.</span><span class="sxs-lookup"><span data-stu-id="42c3d-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="42c3d-120">Шаредкомпутерактиватион</span><span class="sxs-lookup"><span data-stu-id="42c3d-120">sharedComputerActivation</span></span> | <span data-ttu-id="42c3d-121">Int64</span><span class="sxs-lookup"><span data-stu-id="42c3d-121">Int64</span></span>  | <span data-ttu-id="42c3d-122">Количество пользователей, которые использовали продукт на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="42c3d-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42c3d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42c3d-123">JSON representation</span></span>

<span data-ttu-id="42c3d-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42c3d-124">The following is a JSON representation of the resource.</span></span>

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
