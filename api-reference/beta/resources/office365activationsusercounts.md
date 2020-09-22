---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 21e18b35dc4e4ff639087617d679ae1583516026
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021226"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="32966-103">Тип ресурса office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="32966-103">office365ActivationsUserCounts resource type</span></span>

<span data-ttu-id="32966-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32966-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="32966-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="32966-105">Properties</span></span>

| <span data-ttu-id="32966-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="32966-106">Property</span></span>                 | <span data-ttu-id="32966-107">Тип</span><span class="sxs-lookup"><span data-stu-id="32966-107">Type</span></span>   | <span data-ttu-id="32966-108">Описание</span><span class="sxs-lookup"><span data-stu-id="32966-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="32966-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="32966-109">reportRefreshDate</span></span>        | <span data-ttu-id="32966-110">Дата</span><span class="sxs-lookup"><span data-stu-id="32966-110">Date</span></span>   | <span data-ttu-id="32966-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="32966-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="32966-112">продукттипе</span><span class="sxs-lookup"><span data-stu-id="32966-112">productType</span></span>              | <span data-ttu-id="32966-113">String</span><span class="sxs-lookup"><span data-stu-id="32966-113">String</span></span> | <span data-ttu-id="32966-114">Тип продукта, например "Microsoft 365 профессиональный плюс" или "клиент Project".</span><span class="sxs-lookup"><span data-stu-id="32966-114">The product type such as "Microsoft 365 ProPlus" or "Project Client".</span></span> |
| <span data-ttu-id="32966-115">ей</span><span class="sxs-lookup"><span data-stu-id="32966-115">assigned</span></span>                 | <span data-ttu-id="32966-116">Int64</span><span class="sxs-lookup"><span data-stu-id="32966-116">Int64</span></span>  | <span data-ttu-id="32966-117">Количество пользователей, которым назначена лицензия на продукт.</span><span class="sxs-lookup"><span data-stu-id="32966-117">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="32966-118">активной</span><span class="sxs-lookup"><span data-stu-id="32966-118">activated</span></span>                | <span data-ttu-id="32966-119">Int64</span><span class="sxs-lookup"><span data-stu-id="32966-119">Int64</span></span>  | <span data-ttu-id="32966-120">Количество пользователей, которые активировали продукт.</span><span class="sxs-lookup"><span data-stu-id="32966-120">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="32966-121">шаредкомпутерактиватион</span><span class="sxs-lookup"><span data-stu-id="32966-121">sharedComputerActivation</span></span> | <span data-ttu-id="32966-122">Int64</span><span class="sxs-lookup"><span data-stu-id="32966-122">Int64</span></span>  | <span data-ttu-id="32966-123">Количество пользователей, которые использовали продукт на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="32966-123">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="32966-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32966-124">JSON representation</span></span>

<span data-ttu-id="32966-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32966-125">The following is a JSON representation of the resource.</span></span>

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


