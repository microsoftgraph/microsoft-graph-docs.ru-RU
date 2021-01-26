---
title: Тип ресурса emailActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 73e743bc6409f762a7898ec8037633c7bc3f00e4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981853"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="c490c-103">Тип ресурса emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c490c-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="c490c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c490c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c490c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c490c-105">Properties</span></span>

| <span data-ttu-id="c490c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c490c-106">Property</span></span>          | <span data-ttu-id="c490c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c490c-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="c490c-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c490c-108">reportRefreshDate</span></span> | <span data-ttu-id="c490c-109">Дата</span><span class="sxs-lookup"><span data-stu-id="c490c-109">Date</span></span>              |
| <span data-ttu-id="c490c-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c490c-110">userPrincipalName</span></span> | <span data-ttu-id="c490c-111">String</span><span class="sxs-lookup"><span data-stu-id="c490c-111">String</span></span>            |
| <span data-ttu-id="c490c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c490c-112">displayName</span></span>       | <span data-ttu-id="c490c-113">String</span><span class="sxs-lookup"><span data-stu-id="c490c-113">String</span></span>            |
| <span data-ttu-id="c490c-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c490c-114">isDeleted</span></span>         | <span data-ttu-id="c490c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="c490c-115">Boolean</span></span>           |
| <span data-ttu-id="c490c-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="c490c-116">deletedDate</span></span>       | <span data-ttu-id="c490c-117">Дата</span><span class="sxs-lookup"><span data-stu-id="c490c-117">Date</span></span>              |
| <span data-ttu-id="c490c-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c490c-118">lastActivityDate</span></span>  | <span data-ttu-id="c490c-119">Дата</span><span class="sxs-lookup"><span data-stu-id="c490c-119">Date</span></span>              |
| <span data-ttu-id="c490c-120">sendCount</span><span class="sxs-lookup"><span data-stu-id="c490c-120">sendCount</span></span>         | <span data-ttu-id="c490c-121">Int64</span><span class="sxs-lookup"><span data-stu-id="c490c-121">Int64</span></span>             |
| <span data-ttu-id="c490c-122">receiveCount</span><span class="sxs-lookup"><span data-stu-id="c490c-122">receiveCount</span></span>      | <span data-ttu-id="c490c-123">Int64</span><span class="sxs-lookup"><span data-stu-id="c490c-123">Int64</span></span>             |
| <span data-ttu-id="c490c-124">readCount</span><span class="sxs-lookup"><span data-stu-id="c490c-124">readCount</span></span>         | <span data-ttu-id="c490c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c490c-125">Int64</span></span>             |
| <span data-ttu-id="c490c-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="c490c-126">assignedProducts</span></span>  | <span data-ttu-id="c490c-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c490c-127">String collection</span></span> |
| <span data-ttu-id="c490c-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c490c-128">reportPeriod</span></span>      | <span data-ttu-id="c490c-129">String</span><span class="sxs-lookup"><span data-stu-id="c490c-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="c490c-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c490c-130">JSON representation</span></span>

<span data-ttu-id="c490c-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c490c-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```


