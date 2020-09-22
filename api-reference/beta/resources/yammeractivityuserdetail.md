---
title: Тип ресурса Яммерактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: eb17035f0d062d55a3607dd30f31459b79b8400c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971372"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="d217e-103">Тип ресурса Яммерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="d217e-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="d217e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d217e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d217e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d217e-105">Properties</span></span>

| <span data-ttu-id="d217e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d217e-106">Property</span></span>          | <span data-ttu-id="d217e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d217e-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="d217e-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="d217e-108">reportRefreshDate</span></span> | <span data-ttu-id="d217e-109">Дата</span><span class="sxs-lookup"><span data-stu-id="d217e-109">Date</span></span>              |
| <span data-ttu-id="d217e-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d217e-110">userPrincipalName</span></span> | <span data-ttu-id="d217e-111">String</span><span class="sxs-lookup"><span data-stu-id="d217e-111">String</span></span>            |
| <span data-ttu-id="d217e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d217e-112">displayName</span></span>       | <span data-ttu-id="d217e-113">String</span><span class="sxs-lookup"><span data-stu-id="d217e-113">String</span></span>            |
| <span data-ttu-id="d217e-114">userState</span><span class="sxs-lookup"><span data-stu-id="d217e-114">userState</span></span>         | <span data-ttu-id="d217e-115">String</span><span class="sxs-lookup"><span data-stu-id="d217e-115">String</span></span>            |
| <span data-ttu-id="d217e-116">статечанжедате</span><span class="sxs-lookup"><span data-stu-id="d217e-116">stateChangeDate</span></span>   | <span data-ttu-id="d217e-117">Дата</span><span class="sxs-lookup"><span data-stu-id="d217e-117">Date</span></span>              |
| <span data-ttu-id="d217e-118">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="d217e-118">lastActivityDate</span></span>  | <span data-ttu-id="d217e-119">Дата</span><span class="sxs-lookup"><span data-stu-id="d217e-119">Date</span></span>              |
| <span data-ttu-id="d217e-120">постедкаунт</span><span class="sxs-lookup"><span data-stu-id="d217e-120">postedCount</span></span>       | <span data-ttu-id="d217e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d217e-121">Int64</span></span>             |
| <span data-ttu-id="d217e-122">реадкаунт</span><span class="sxs-lookup"><span data-stu-id="d217e-122">readCount</span></span>         | <span data-ttu-id="d217e-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d217e-123">Int64</span></span>             |
| <span data-ttu-id="d217e-124">ликедкаунт</span><span class="sxs-lookup"><span data-stu-id="d217e-124">likedCount</span></span>        | <span data-ttu-id="d217e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d217e-125">Int64</span></span>             |
| <span data-ttu-id="d217e-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="d217e-126">assignedProducts</span></span>  | <span data-ttu-id="d217e-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d217e-127">String collection</span></span> |
| <span data-ttu-id="d217e-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="d217e-128">reportPeriod</span></span>      | <span data-ttu-id="d217e-129">String</span><span class="sxs-lookup"><span data-stu-id="d217e-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="d217e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d217e-130">JSON representation</span></span>

<span data-ttu-id="d217e-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d217e-131">The following is a JSON representation of the resource.</span></span>

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


