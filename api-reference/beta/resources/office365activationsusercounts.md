---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 33339578f498460aacd24481f166ab717138f8fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966568"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="be473-103">Тип ресурса office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="be473-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="be473-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="be473-104">Properties</span></span>

| <span data-ttu-id="be473-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="be473-105">Property</span></span>                 | <span data-ttu-id="be473-106">Тип</span><span class="sxs-lookup"><span data-stu-id="be473-106">Type</span></span>   | <span data-ttu-id="be473-107">Описание</span><span class="sxs-lookup"><span data-stu-id="be473-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="be473-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="be473-108">reportRefreshDate</span></span>        | <span data-ttu-id="be473-109">Дата</span><span class="sxs-lookup"><span data-stu-id="be473-109">Date</span></span>   | <span data-ttu-id="be473-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="be473-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="be473-111">Продукттипе</span><span class="sxs-lookup"><span data-stu-id="be473-111">productType</span></span>              | <span data-ttu-id="be473-112">String</span><span class="sxs-lookup"><span data-stu-id="be473-112">String</span></span> | <span data-ttu-id="be473-113">Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="be473-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="be473-114">ей</span><span class="sxs-lookup"><span data-stu-id="be473-114">assigned</span></span>                 | <span data-ttu-id="be473-115">Int64</span><span class="sxs-lookup"><span data-stu-id="be473-115">Int64</span></span>  | <span data-ttu-id="be473-116">Количество пользователей, которым назначена лицензия на продукт.</span><span class="sxs-lookup"><span data-stu-id="be473-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="be473-117">активной</span><span class="sxs-lookup"><span data-stu-id="be473-117">activated</span></span>                | <span data-ttu-id="be473-118">Int64</span><span class="sxs-lookup"><span data-stu-id="be473-118">Int64</span></span>  | <span data-ttu-id="be473-119">Количество пользователей, которые активировали продукт.</span><span class="sxs-lookup"><span data-stu-id="be473-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="be473-120">Шаредкомпутерактиватион</span><span class="sxs-lookup"><span data-stu-id="be473-120">sharedComputerActivation</span></span> | <span data-ttu-id="be473-121">Int64</span><span class="sxs-lookup"><span data-stu-id="be473-121">Int64</span></span>  | <span data-ttu-id="be473-122">Количество пользователей, которые использовали продукт на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="be473-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="be473-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be473-123">JSON representation</span></span>

<span data-ttu-id="be473-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be473-124">The following is a JSON representation of the resource.</span></span>

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
