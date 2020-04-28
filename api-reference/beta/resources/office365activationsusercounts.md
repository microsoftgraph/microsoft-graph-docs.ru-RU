---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 78c21f33352e5f6357638de8dacc4b628b6ef93b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522486"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="899dc-103">Тип ресурса office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="899dc-103">office365ActivationsUserCounts resource type</span></span>

<span data-ttu-id="899dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="899dc-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="899dc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="899dc-105">Properties</span></span>

| <span data-ttu-id="899dc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="899dc-106">Property</span></span>                 | <span data-ttu-id="899dc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="899dc-107">Type</span></span>   | <span data-ttu-id="899dc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="899dc-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="899dc-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="899dc-109">reportRefreshDate</span></span>        | <span data-ttu-id="899dc-110">Дата</span><span class="sxs-lookup"><span data-stu-id="899dc-110">Date</span></span>   | <span data-ttu-id="899dc-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="899dc-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="899dc-112">продукттипе</span><span class="sxs-lookup"><span data-stu-id="899dc-112">productType</span></span>              | <span data-ttu-id="899dc-113">String</span><span class="sxs-lookup"><span data-stu-id="899dc-113">String</span></span> | <span data-ttu-id="899dc-114">Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365".</span><span class="sxs-lookup"><span data-stu-id="899dc-114">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="899dc-115">ей</span><span class="sxs-lookup"><span data-stu-id="899dc-115">assigned</span></span>                 | <span data-ttu-id="899dc-116">Int64</span><span class="sxs-lookup"><span data-stu-id="899dc-116">Int64</span></span>  | <span data-ttu-id="899dc-117">Количество пользователей, которым назначена лицензия на продукт.</span><span class="sxs-lookup"><span data-stu-id="899dc-117">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="899dc-118">активной</span><span class="sxs-lookup"><span data-stu-id="899dc-118">activated</span></span>                | <span data-ttu-id="899dc-119">Int64</span><span class="sxs-lookup"><span data-stu-id="899dc-119">Int64</span></span>  | <span data-ttu-id="899dc-120">Количество пользователей, которые активировали продукт.</span><span class="sxs-lookup"><span data-stu-id="899dc-120">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="899dc-121">шаредкомпутерактиватион</span><span class="sxs-lookup"><span data-stu-id="899dc-121">sharedComputerActivation</span></span> | <span data-ttu-id="899dc-122">Int64</span><span class="sxs-lookup"><span data-stu-id="899dc-122">Int64</span></span>  | <span data-ttu-id="899dc-123">Количество пользователей, которые использовали продукт на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="899dc-123">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="899dc-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="899dc-124">JSON representation</span></span>

<span data-ttu-id="899dc-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="899dc-125">The following is a JSON representation of the resource.</span></span>

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
