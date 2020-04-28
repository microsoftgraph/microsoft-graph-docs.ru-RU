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
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="ada99-103">Тип ресурса Яммерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="ada99-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="ada99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ada99-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="ada99-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ada99-105">Properties</span></span>

| <span data-ttu-id="ada99-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ada99-106">Property</span></span>          | <span data-ttu-id="ada99-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ada99-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="ada99-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="ada99-108">reportRefreshDate</span></span> | <span data-ttu-id="ada99-109">Дата</span><span class="sxs-lookup"><span data-stu-id="ada99-109">Date</span></span>              |
| <span data-ttu-id="ada99-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ada99-110">userPrincipalName</span></span> | <span data-ttu-id="ada99-111">String</span><span class="sxs-lookup"><span data-stu-id="ada99-111">String</span></span>            |
| <span data-ttu-id="ada99-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ada99-112">displayName</span></span>       | <span data-ttu-id="ada99-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ada99-113">String</span></span>            |
| <span data-ttu-id="ada99-114">userState</span><span class="sxs-lookup"><span data-stu-id="ada99-114">userState</span></span>         | <span data-ttu-id="ada99-115">String</span><span class="sxs-lookup"><span data-stu-id="ada99-115">String</span></span>            |
| <span data-ttu-id="ada99-116">статечанжедате</span><span class="sxs-lookup"><span data-stu-id="ada99-116">stateChangeDate</span></span>   | <span data-ttu-id="ada99-117">Дата</span><span class="sxs-lookup"><span data-stu-id="ada99-117">Date</span></span>              |
| <span data-ttu-id="ada99-118">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="ada99-118">lastActivityDate</span></span>  | <span data-ttu-id="ada99-119">Дата</span><span class="sxs-lookup"><span data-stu-id="ada99-119">Date</span></span>              |
| <span data-ttu-id="ada99-120">постедкаунт</span><span class="sxs-lookup"><span data-stu-id="ada99-120">postedCount</span></span>       | <span data-ttu-id="ada99-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ada99-121">Int64</span></span>             |
| <span data-ttu-id="ada99-122">реадкаунт</span><span class="sxs-lookup"><span data-stu-id="ada99-122">readCount</span></span>         | <span data-ttu-id="ada99-123">Int64</span><span class="sxs-lookup"><span data-stu-id="ada99-123">Int64</span></span>             |
| <span data-ttu-id="ada99-124">ликедкаунт</span><span class="sxs-lookup"><span data-stu-id="ada99-124">likedCount</span></span>        | <span data-ttu-id="ada99-125">Int64</span><span class="sxs-lookup"><span data-stu-id="ada99-125">Int64</span></span>             |
| <span data-ttu-id="ada99-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="ada99-126">assignedProducts</span></span>  | <span data-ttu-id="ada99-127">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ada99-127">String collection</span></span> |
| <span data-ttu-id="ada99-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="ada99-128">reportPeriod</span></span>      | <span data-ttu-id="ada99-129">String</span><span class="sxs-lookup"><span data-stu-id="ada99-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="ada99-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ada99-130">JSON representation</span></span>

<span data-ttu-id="ada99-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ada99-131">The following is a JSON representation of the resource.</span></span>

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
