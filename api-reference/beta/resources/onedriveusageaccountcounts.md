---
title: Тип ресурса Онедривеусажеаккаунткаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 759f231181da13cc2d115ff332e909e3a8387474
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522388"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="705a8-103">Тип ресурса Онедривеусажеаккаунткаунтс</span><span class="sxs-lookup"><span data-stu-id="705a8-103">oneDriveUsageAccountCounts resource type</span></span>

<span data-ttu-id="705a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="705a8-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="705a8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="705a8-105">Properties</span></span>

| <span data-ttu-id="705a8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="705a8-106">Property</span></span>          | <span data-ttu-id="705a8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="705a8-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="705a8-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="705a8-108">reportRefreshDate</span></span> | <span data-ttu-id="705a8-109">Дата</span><span class="sxs-lookup"><span data-stu-id="705a8-109">Date</span></span>   |
| <span data-ttu-id="705a8-110">ситетипе</span><span class="sxs-lookup"><span data-stu-id="705a8-110">siteType</span></span>          | <span data-ttu-id="705a8-111">String</span><span class="sxs-lookup"><span data-stu-id="705a8-111">String</span></span> |
| <span data-ttu-id="705a8-112">total</span><span class="sxs-lookup"><span data-stu-id="705a8-112">total</span></span>             | <span data-ttu-id="705a8-113">Int64</span><span class="sxs-lookup"><span data-stu-id="705a8-113">Int64</span></span>  |
| <span data-ttu-id="705a8-114">ASP</span><span class="sxs-lookup"><span data-stu-id="705a8-114">active</span></span>            | <span data-ttu-id="705a8-115">Int64</span><span class="sxs-lookup"><span data-stu-id="705a8-115">Int64</span></span>  |
| <span data-ttu-id="705a8-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="705a8-116">reportDate</span></span>        | <span data-ttu-id="705a8-117">Дата</span><span class="sxs-lookup"><span data-stu-id="705a8-117">Date</span></span>   |
| <span data-ttu-id="705a8-118">репортпериод</span><span class="sxs-lookup"><span data-stu-id="705a8-118">reportPeriod</span></span>      | <span data-ttu-id="705a8-119">String</span><span class="sxs-lookup"><span data-stu-id="705a8-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="705a8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="705a8-120">JSON representation</span></span>

<span data-ttu-id="705a8-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="705a8-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
