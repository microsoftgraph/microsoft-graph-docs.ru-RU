---
title: Тип ресурса Яммерактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 960945d72db1cc347228983b9567968dfcfc52d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963789"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="aa315-103">Тип ресурса Яммерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="aa315-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="aa315-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa315-104">Properties</span></span>

| <span data-ttu-id="aa315-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa315-105">Property</span></span>          | <span data-ttu-id="aa315-106">Тип</span><span class="sxs-lookup"><span data-stu-id="aa315-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="aa315-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="aa315-107">reportRefreshDate</span></span> | <span data-ttu-id="aa315-108">Дата</span><span class="sxs-lookup"><span data-stu-id="aa315-108">Date</span></span>              |
| <span data-ttu-id="aa315-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aa315-109">userPrincipalName</span></span> | <span data-ttu-id="aa315-110">String</span><span class="sxs-lookup"><span data-stu-id="aa315-110">String</span></span>            |
| <span data-ttu-id="aa315-111">displayName</span><span class="sxs-lookup"><span data-stu-id="aa315-111">displayName</span></span>       | <span data-ttu-id="aa315-112">Строка</span><span class="sxs-lookup"><span data-stu-id="aa315-112">String</span></span>            |
| <span data-ttu-id="aa315-113">userState</span><span class="sxs-lookup"><span data-stu-id="aa315-113">userState</span></span>         | <span data-ttu-id="aa315-114">String</span><span class="sxs-lookup"><span data-stu-id="aa315-114">String</span></span>            |
| <span data-ttu-id="aa315-115">Статечанжедате</span><span class="sxs-lookup"><span data-stu-id="aa315-115">stateChangeDate</span></span>   | <span data-ttu-id="aa315-116">Дата</span><span class="sxs-lookup"><span data-stu-id="aa315-116">Date</span></span>              |
| <span data-ttu-id="aa315-117">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="aa315-117">lastActivityDate</span></span>  | <span data-ttu-id="aa315-118">Дата</span><span class="sxs-lookup"><span data-stu-id="aa315-118">Date</span></span>              |
| <span data-ttu-id="aa315-119">Постедкаунт</span><span class="sxs-lookup"><span data-stu-id="aa315-119">postedCount</span></span>       | <span data-ttu-id="aa315-120">Int64</span><span class="sxs-lookup"><span data-stu-id="aa315-120">Int64</span></span>             |
| <span data-ttu-id="aa315-121">Реадкаунт</span><span class="sxs-lookup"><span data-stu-id="aa315-121">readCount</span></span>         | <span data-ttu-id="aa315-122">Int64</span><span class="sxs-lookup"><span data-stu-id="aa315-122">Int64</span></span>             |
| <span data-ttu-id="aa315-123">Ликедкаунт</span><span class="sxs-lookup"><span data-stu-id="aa315-123">likedCount</span></span>        | <span data-ttu-id="aa315-124">Int64</span><span class="sxs-lookup"><span data-stu-id="aa315-124">Int64</span></span>             |
| <span data-ttu-id="aa315-125">Ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="aa315-125">assignedProducts</span></span>  | <span data-ttu-id="aa315-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="aa315-126">String collection</span></span> |
| <span data-ttu-id="aa315-127">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="aa315-127">reportPeriod</span></span>      | <span data-ttu-id="aa315-128">String</span><span class="sxs-lookup"><span data-stu-id="aa315-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="aa315-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa315-129">JSON representation</span></span>

<span data-ttu-id="aa315-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa315-130">The following is a JSON representation of the resource.</span></span>

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
