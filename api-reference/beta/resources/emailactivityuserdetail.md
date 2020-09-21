---
title: Тип ресурса Емаилактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 76ec180ceb239f79c420f26b48521e9bc7e81787
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979485"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="2e4ec-103">Тип ресурса Емаилактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="2e4ec-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="2e4ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e4ec-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2e4ec-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e4ec-105">Properties</span></span>

| <span data-ttu-id="2e4ec-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e4ec-106">Property</span></span>          | <span data-ttu-id="2e4ec-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2e4ec-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="2e4ec-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="2e4ec-108">reportRefreshDate</span></span> | <span data-ttu-id="2e4ec-109">Дата</span><span class="sxs-lookup"><span data-stu-id="2e4ec-109">Date</span></span>              |
| <span data-ttu-id="2e4ec-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2e4ec-110">userPrincipalName</span></span> | <span data-ttu-id="2e4ec-111">String</span><span class="sxs-lookup"><span data-stu-id="2e4ec-111">String</span></span>            |
| <span data-ttu-id="2e4ec-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2e4ec-112">displayName</span></span>       | <span data-ttu-id="2e4ec-113">String</span><span class="sxs-lookup"><span data-stu-id="2e4ec-113">String</span></span>            |
| <span data-ttu-id="2e4ec-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="2e4ec-114">isDeleted</span></span>         | <span data-ttu-id="2e4ec-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e4ec-115">Boolean</span></span>           |
| <span data-ttu-id="2e4ec-116">делетеддате</span><span class="sxs-lookup"><span data-stu-id="2e4ec-116">deletedDate</span></span>       | <span data-ttu-id="2e4ec-117">Дата</span><span class="sxs-lookup"><span data-stu-id="2e4ec-117">Date</span></span>              |
| <span data-ttu-id="2e4ec-118">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="2e4ec-118">lastActivityDate</span></span>  | <span data-ttu-id="2e4ec-119">Дата</span><span class="sxs-lookup"><span data-stu-id="2e4ec-119">Date</span></span>              |
| <span data-ttu-id="2e4ec-120">сендкаунт</span><span class="sxs-lookup"><span data-stu-id="2e4ec-120">sendCount</span></span>         | <span data-ttu-id="2e4ec-121">Int64</span><span class="sxs-lookup"><span data-stu-id="2e4ec-121">Int64</span></span>             |
| <span data-ttu-id="2e4ec-122">рецеивекаунт</span><span class="sxs-lookup"><span data-stu-id="2e4ec-122">receiveCount</span></span>      | <span data-ttu-id="2e4ec-123">Int64</span><span class="sxs-lookup"><span data-stu-id="2e4ec-123">Int64</span></span>             |
| <span data-ttu-id="2e4ec-124">реадкаунт</span><span class="sxs-lookup"><span data-stu-id="2e4ec-124">readCount</span></span>         | <span data-ttu-id="2e4ec-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2e4ec-125">Int64</span></span>             |
| <span data-ttu-id="2e4ec-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="2e4ec-126">assignedProducts</span></span>  | <span data-ttu-id="2e4ec-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2e4ec-127">String collection</span></span> |
| <span data-ttu-id="2e4ec-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="2e4ec-128">reportPeriod</span></span>      | <span data-ttu-id="2e4ec-129">String</span><span class="sxs-lookup"><span data-stu-id="2e4ec-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="2e4ec-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e4ec-130">JSON representation</span></span>

<span data-ttu-id="2e4ec-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e4ec-131">The following is a JSON representation of the resource.</span></span>

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


