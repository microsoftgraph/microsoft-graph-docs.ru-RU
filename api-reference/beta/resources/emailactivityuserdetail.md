---
title: Тип ресурса emailActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 4f74b4af41c44e41b07bae1a8421011bc5188efc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074805"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="e36e6-103">Тип ресурса emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e36e6-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e36e6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e36e6-104">Properties</span></span>

| <span data-ttu-id="e36e6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e36e6-105">Property</span></span>          | <span data-ttu-id="e36e6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e36e6-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="e36e6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e36e6-107">reportRefreshDate</span></span> | <span data-ttu-id="e36e6-108">Date</span><span class="sxs-lookup"><span data-stu-id="e36e6-108">Date</span></span>              |
| <span data-ttu-id="e36e6-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e36e6-109">userPrincipalName</span></span> | <span data-ttu-id="e36e6-110">String</span><span class="sxs-lookup"><span data-stu-id="e36e6-110">String</span></span>            |
| <span data-ttu-id="e36e6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e36e6-111">displayName</span></span>       | <span data-ttu-id="e36e6-112">String</span><span class="sxs-lookup"><span data-stu-id="e36e6-112">String</span></span>            |
| <span data-ttu-id="e36e6-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e36e6-113">isDeleted</span></span>         | <span data-ttu-id="e36e6-114">Логический</span><span class="sxs-lookup"><span data-stu-id="e36e6-114">Boolean</span></span>           |
| <span data-ttu-id="e36e6-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="e36e6-115">deletedDate</span></span>       | <span data-ttu-id="e36e6-116">Date</span><span class="sxs-lookup"><span data-stu-id="e36e6-116">Date</span></span>              |
| <span data-ttu-id="e36e6-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e36e6-117">lastActivityDate</span></span>  | <span data-ttu-id="e36e6-118">Date</span><span class="sxs-lookup"><span data-stu-id="e36e6-118">Date</span></span>              |
| <span data-ttu-id="e36e6-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="e36e6-119">sendCount</span></span>         | <span data-ttu-id="e36e6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e36e6-120">Int64</span></span>             |
| <span data-ttu-id="e36e6-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="e36e6-121">receiveCount</span></span>      | <span data-ttu-id="e36e6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e36e6-122">Int64</span></span>             |
| <span data-ttu-id="e36e6-123">readCount</span><span class="sxs-lookup"><span data-stu-id="e36e6-123">readCount</span></span>         | <span data-ttu-id="e36e6-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e36e6-124">Int64</span></span>             |
| <span data-ttu-id="e36e6-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="e36e6-125">assignedProducts</span></span>  | <span data-ttu-id="e36e6-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e36e6-126">String collection</span></span> |
| <span data-ttu-id="e36e6-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e36e6-127">reportPeriod</span></span>      | <span data-ttu-id="e36e6-128">String</span><span class="sxs-lookup"><span data-stu-id="e36e6-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="e36e6-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e36e6-129">JSON representation</span></span>

<span data-ttu-id="e36e6-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e36e6-130">The following is a JSON representation of the resource.</span></span>

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
