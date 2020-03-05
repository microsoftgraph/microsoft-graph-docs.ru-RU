---
title: Тип ресурса Емаилактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c664cb4a381cf2ebe3de9bd9ca53719786b94405
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499570"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="f0862-103">Тип ресурса Емаилактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="f0862-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="f0862-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f0862-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f0862-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0862-105">Properties</span></span>

| <span data-ttu-id="f0862-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0862-106">Property</span></span>          | <span data-ttu-id="f0862-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f0862-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="f0862-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="f0862-108">reportRefreshDate</span></span> | <span data-ttu-id="f0862-109">Дата</span><span class="sxs-lookup"><span data-stu-id="f0862-109">Date</span></span>              |
| <span data-ttu-id="f0862-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0862-110">userPrincipalName</span></span> | <span data-ttu-id="f0862-111">String</span><span class="sxs-lookup"><span data-stu-id="f0862-111">String</span></span>            |
| <span data-ttu-id="f0862-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f0862-112">displayName</span></span>       | <span data-ttu-id="f0862-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f0862-113">String</span></span>            |
| <span data-ttu-id="f0862-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f0862-114">isDeleted</span></span>         | <span data-ttu-id="f0862-115">Логический</span><span class="sxs-lookup"><span data-stu-id="f0862-115">Boolean</span></span>           |
| <span data-ttu-id="f0862-116">делетеддате</span><span class="sxs-lookup"><span data-stu-id="f0862-116">deletedDate</span></span>       | <span data-ttu-id="f0862-117">Дата</span><span class="sxs-lookup"><span data-stu-id="f0862-117">Date</span></span>              |
| <span data-ttu-id="f0862-118">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="f0862-118">lastActivityDate</span></span>  | <span data-ttu-id="f0862-119">Дата</span><span class="sxs-lookup"><span data-stu-id="f0862-119">Date</span></span>              |
| <span data-ttu-id="f0862-120">сендкаунт</span><span class="sxs-lookup"><span data-stu-id="f0862-120">sendCount</span></span>         | <span data-ttu-id="f0862-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f0862-121">Int64</span></span>             |
| <span data-ttu-id="f0862-122">рецеивекаунт</span><span class="sxs-lookup"><span data-stu-id="f0862-122">receiveCount</span></span>      | <span data-ttu-id="f0862-123">Int64</span><span class="sxs-lookup"><span data-stu-id="f0862-123">Int64</span></span>             |
| <span data-ttu-id="f0862-124">реадкаунт</span><span class="sxs-lookup"><span data-stu-id="f0862-124">readCount</span></span>         | <span data-ttu-id="f0862-125">Int64</span><span class="sxs-lookup"><span data-stu-id="f0862-125">Int64</span></span>             |
| <span data-ttu-id="f0862-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="f0862-126">assignedProducts</span></span>  | <span data-ttu-id="f0862-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f0862-127">String collection</span></span> |
| <span data-ttu-id="f0862-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="f0862-128">reportPeriod</span></span>      | <span data-ttu-id="f0862-129">String</span><span class="sxs-lookup"><span data-stu-id="f0862-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="f0862-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0862-130">JSON representation</span></span>

<span data-ttu-id="f0862-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0862-131">The following is a JSON representation of the resource.</span></span>

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
