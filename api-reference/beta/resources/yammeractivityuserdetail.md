---
title: Тип ресурса yammerActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 749076f407b49ff4fd408a095312ac49ea008bc1
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982399"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="d6148-103">Тип ресурса yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d6148-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="d6148-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6148-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d6148-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6148-105">Properties</span></span>

| <span data-ttu-id="d6148-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6148-106">Property</span></span>          | <span data-ttu-id="d6148-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d6148-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="d6148-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d6148-108">reportRefreshDate</span></span> | <span data-ttu-id="d6148-109">Дата</span><span class="sxs-lookup"><span data-stu-id="d6148-109">Date</span></span>              |
| <span data-ttu-id="d6148-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d6148-110">userPrincipalName</span></span> | <span data-ttu-id="d6148-111">String</span><span class="sxs-lookup"><span data-stu-id="d6148-111">String</span></span>            |
| <span data-ttu-id="d6148-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d6148-112">displayName</span></span>       | <span data-ttu-id="d6148-113">String</span><span class="sxs-lookup"><span data-stu-id="d6148-113">String</span></span>            |
| <span data-ttu-id="d6148-114">userState</span><span class="sxs-lookup"><span data-stu-id="d6148-114">userState</span></span>         | <span data-ttu-id="d6148-115">String</span><span class="sxs-lookup"><span data-stu-id="d6148-115">String</span></span>            |
| <span data-ttu-id="d6148-116">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="d6148-116">stateChangeDate</span></span>   | <span data-ttu-id="d6148-117">Дата</span><span class="sxs-lookup"><span data-stu-id="d6148-117">Date</span></span>              |
| <span data-ttu-id="d6148-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d6148-118">lastActivityDate</span></span>  | <span data-ttu-id="d6148-119">Дата</span><span class="sxs-lookup"><span data-stu-id="d6148-119">Date</span></span>              |
| <span data-ttu-id="d6148-120">postedCount</span><span class="sxs-lookup"><span data-stu-id="d6148-120">postedCount</span></span>       | <span data-ttu-id="d6148-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d6148-121">Int64</span></span>             |
| <span data-ttu-id="d6148-122">readCount</span><span class="sxs-lookup"><span data-stu-id="d6148-122">readCount</span></span>         | <span data-ttu-id="d6148-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d6148-123">Int64</span></span>             |
| <span data-ttu-id="d6148-124">likedCount</span><span class="sxs-lookup"><span data-stu-id="d6148-124">likedCount</span></span>        | <span data-ttu-id="d6148-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d6148-125">Int64</span></span>             |
| <span data-ttu-id="d6148-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="d6148-126">assignedProducts</span></span>  | <span data-ttu-id="d6148-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d6148-127">String collection</span></span> |
| <span data-ttu-id="d6148-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d6148-128">reportPeriod</span></span>      | <span data-ttu-id="d6148-129">String</span><span class="sxs-lookup"><span data-stu-id="d6148-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="d6148-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6148-130">JSON representation</span></span>

<span data-ttu-id="d6148-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6148-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```


