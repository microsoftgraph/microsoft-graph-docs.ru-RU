---
title: Тип ресурса Яммерактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 922ebf14f59d60a988fe77ee36ce04d9c76befec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519031"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="e9ad9-103">Тип ресурса Яммерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="e9ad9-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="e9ad9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e9ad9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e9ad9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9ad9-105">Properties</span></span>

| <span data-ttu-id="e9ad9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9ad9-106">Property</span></span>          | <span data-ttu-id="e9ad9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e9ad9-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="e9ad9-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="e9ad9-108">reportRefreshDate</span></span> | <span data-ttu-id="e9ad9-109">Дата</span><span class="sxs-lookup"><span data-stu-id="e9ad9-109">Date</span></span>              |
| <span data-ttu-id="e9ad9-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e9ad9-110">userPrincipalName</span></span> | <span data-ttu-id="e9ad9-111">String</span><span class="sxs-lookup"><span data-stu-id="e9ad9-111">String</span></span>            |
| <span data-ttu-id="e9ad9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e9ad9-112">displayName</span></span>       | <span data-ttu-id="e9ad9-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e9ad9-113">String</span></span>            |
| <span data-ttu-id="e9ad9-114">userState</span><span class="sxs-lookup"><span data-stu-id="e9ad9-114">userState</span></span>         | <span data-ttu-id="e9ad9-115">String</span><span class="sxs-lookup"><span data-stu-id="e9ad9-115">String</span></span>            |
| <span data-ttu-id="e9ad9-116">статечанжедате</span><span class="sxs-lookup"><span data-stu-id="e9ad9-116">stateChangeDate</span></span>   | <span data-ttu-id="e9ad9-117">Дата</span><span class="sxs-lookup"><span data-stu-id="e9ad9-117">Date</span></span>              |
| <span data-ttu-id="e9ad9-118">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="e9ad9-118">lastActivityDate</span></span>  | <span data-ttu-id="e9ad9-119">Дата</span><span class="sxs-lookup"><span data-stu-id="e9ad9-119">Date</span></span>              |
| <span data-ttu-id="e9ad9-120">постедкаунт</span><span class="sxs-lookup"><span data-stu-id="e9ad9-120">postedCount</span></span>       | <span data-ttu-id="e9ad9-121">Int64</span><span class="sxs-lookup"><span data-stu-id="e9ad9-121">Int64</span></span>             |
| <span data-ttu-id="e9ad9-122">реадкаунт</span><span class="sxs-lookup"><span data-stu-id="e9ad9-122">readCount</span></span>         | <span data-ttu-id="e9ad9-123">Int64</span><span class="sxs-lookup"><span data-stu-id="e9ad9-123">Int64</span></span>             |
| <span data-ttu-id="e9ad9-124">ликедкаунт</span><span class="sxs-lookup"><span data-stu-id="e9ad9-124">likedCount</span></span>        | <span data-ttu-id="e9ad9-125">Int64</span><span class="sxs-lookup"><span data-stu-id="e9ad9-125">Int64</span></span>             |
| <span data-ttu-id="e9ad9-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="e9ad9-126">assignedProducts</span></span>  | <span data-ttu-id="e9ad9-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e9ad9-127">String collection</span></span> |
| <span data-ttu-id="e9ad9-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="e9ad9-128">reportPeriod</span></span>      | <span data-ttu-id="e9ad9-129">String</span><span class="sxs-lookup"><span data-stu-id="e9ad9-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="e9ad9-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9ad9-130">JSON representation</span></span>

<span data-ttu-id="e9ad9-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9ad9-131">The following is a JSON representation of the resource.</span></span>

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
