---
title: Тип ресурса Яммерактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541187"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="0c4af-103">Тип ресурса Яммерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="0c4af-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0c4af-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c4af-104">Properties</span></span>

| <span data-ttu-id="0c4af-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c4af-105">Property</span></span>          | <span data-ttu-id="0c4af-106">Тип</span><span class="sxs-lookup"><span data-stu-id="0c4af-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="0c4af-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="0c4af-107">reportRefreshDate</span></span> | <span data-ttu-id="0c4af-108">Дата</span><span class="sxs-lookup"><span data-stu-id="0c4af-108">Date</span></span>              |
| <span data-ttu-id="0c4af-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0c4af-109">userPrincipalName</span></span> | <span data-ttu-id="0c4af-110">String</span><span class="sxs-lookup"><span data-stu-id="0c4af-110">String</span></span>            |
| <span data-ttu-id="0c4af-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0c4af-111">displayName</span></span>       | <span data-ttu-id="0c4af-112">String</span><span class="sxs-lookup"><span data-stu-id="0c4af-112">String</span></span>            |
| <span data-ttu-id="0c4af-113">userState</span><span class="sxs-lookup"><span data-stu-id="0c4af-113">userState</span></span>         | <span data-ttu-id="0c4af-114">String</span><span class="sxs-lookup"><span data-stu-id="0c4af-114">String</span></span>            |
| <span data-ttu-id="0c4af-115">Статечанжедате</span><span class="sxs-lookup"><span data-stu-id="0c4af-115">stateChangeDate</span></span>   | <span data-ttu-id="0c4af-116">Дата</span><span class="sxs-lookup"><span data-stu-id="0c4af-116">Date</span></span>              |
| <span data-ttu-id="0c4af-117">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="0c4af-117">lastActivityDate</span></span>  | <span data-ttu-id="0c4af-118">Дата</span><span class="sxs-lookup"><span data-stu-id="0c4af-118">Date</span></span>              |
| <span data-ttu-id="0c4af-119">Постедкаунт</span><span class="sxs-lookup"><span data-stu-id="0c4af-119">postedCount</span></span>       | <span data-ttu-id="0c4af-120">Int64</span><span class="sxs-lookup"><span data-stu-id="0c4af-120">Int64</span></span>             |
| <span data-ttu-id="0c4af-121">Реадкаунт</span><span class="sxs-lookup"><span data-stu-id="0c4af-121">readCount</span></span>         | <span data-ttu-id="0c4af-122">Int64</span><span class="sxs-lookup"><span data-stu-id="0c4af-122">Int64</span></span>             |
| <span data-ttu-id="0c4af-123">Ликедкаунт</span><span class="sxs-lookup"><span data-stu-id="0c4af-123">likedCount</span></span>        | <span data-ttu-id="0c4af-124">Int64</span><span class="sxs-lookup"><span data-stu-id="0c4af-124">Int64</span></span>             |
| <span data-ttu-id="0c4af-125">Ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="0c4af-125">assignedProducts</span></span>  | <span data-ttu-id="0c4af-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0c4af-126">String collection</span></span> |
| <span data-ttu-id="0c4af-127">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="0c4af-127">reportPeriod</span></span>      | <span data-ttu-id="0c4af-128">String</span><span class="sxs-lookup"><span data-stu-id="0c4af-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="0c4af-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0c4af-129">JSON representation</span></span>

<span data-ttu-id="0c4af-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c4af-130">The following is a JSON representation of the resource.</span></span>

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
