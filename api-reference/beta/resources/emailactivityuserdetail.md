---
title: Тип ресурса emailActivityUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 16512c3a8a4dab62d4a71406d6c33d52a5a9bc08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818005"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="5de44-103">Тип ресурса emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="5de44-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5de44-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="5de44-104">Properties</span></span>

| <span data-ttu-id="5de44-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="5de44-105">Property</span></span>          | <span data-ttu-id="5de44-106">Тип</span><span class="sxs-lookup"><span data-stu-id="5de44-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="5de44-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5de44-107">reportRefreshDate</span></span> | <span data-ttu-id="5de44-108">Date</span><span class="sxs-lookup"><span data-stu-id="5de44-108">Date</span></span>              |
| <span data-ttu-id="5de44-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5de44-109">userPrincipalName</span></span> | <span data-ttu-id="5de44-110">Строка</span><span class="sxs-lookup"><span data-stu-id="5de44-110">String</span></span>            |
| <span data-ttu-id="5de44-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5de44-111">displayName</span></span>       | <span data-ttu-id="5de44-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5de44-112">String</span></span>            |
| <span data-ttu-id="5de44-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5de44-113">isDeleted</span></span>         | <span data-ttu-id="5de44-114">Логический</span><span class="sxs-lookup"><span data-stu-id="5de44-114">Boolean</span></span>           |
| <span data-ttu-id="5de44-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="5de44-115">deletedDate</span></span>       | <span data-ttu-id="5de44-116">Date</span><span class="sxs-lookup"><span data-stu-id="5de44-116">Date</span></span>              |
| <span data-ttu-id="5de44-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="5de44-117">lastActivityDate</span></span>  | <span data-ttu-id="5de44-118">Date</span><span class="sxs-lookup"><span data-stu-id="5de44-118">Date</span></span>              |
| <span data-ttu-id="5de44-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="5de44-119">sendCount</span></span>         | <span data-ttu-id="5de44-120">Int64</span><span class="sxs-lookup"><span data-stu-id="5de44-120">Int64</span></span>             |
| <span data-ttu-id="5de44-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="5de44-121">receiveCount</span></span>      | <span data-ttu-id="5de44-122">Int64</span><span class="sxs-lookup"><span data-stu-id="5de44-122">Int64</span></span>             |
| <span data-ttu-id="5de44-123">readCount</span><span class="sxs-lookup"><span data-stu-id="5de44-123">readCount</span></span>         | <span data-ttu-id="5de44-124">Int64</span><span class="sxs-lookup"><span data-stu-id="5de44-124">Int64</span></span>             |
| <span data-ttu-id="5de44-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="5de44-125">assignedProducts</span></span>  | <span data-ttu-id="5de44-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5de44-126">String collection</span></span> |
| <span data-ttu-id="5de44-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5de44-127">reportPeriod</span></span>      | <span data-ttu-id="5de44-128">String</span><span class="sxs-lookup"><span data-stu-id="5de44-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="5de44-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5de44-129">JSON representation</span></span>

<span data-ttu-id="5de44-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5de44-130">The following is a JSON representation of the resource.</span></span>

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
