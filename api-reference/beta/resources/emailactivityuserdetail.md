---
title: Тип ресурса Емаилактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542834"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="7a105-103">Тип ресурса Емаилактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="7a105-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7a105-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a105-104">Properties</span></span>

| <span data-ttu-id="7a105-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a105-105">Property</span></span>          | <span data-ttu-id="7a105-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7a105-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="7a105-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="7a105-107">reportRefreshDate</span></span> | <span data-ttu-id="7a105-108">Дата</span><span class="sxs-lookup"><span data-stu-id="7a105-108">Date</span></span>              |
| <span data-ttu-id="7a105-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7a105-109">userPrincipalName</span></span> | <span data-ttu-id="7a105-110">String</span><span class="sxs-lookup"><span data-stu-id="7a105-110">String</span></span>            |
| <span data-ttu-id="7a105-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7a105-111">displayName</span></span>       | <span data-ttu-id="7a105-112">String</span><span class="sxs-lookup"><span data-stu-id="7a105-112">String</span></span>            |
| <span data-ttu-id="7a105-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="7a105-113">isDeleted</span></span>         | <span data-ttu-id="7a105-114">Логический</span><span class="sxs-lookup"><span data-stu-id="7a105-114">Boolean</span></span>           |
| <span data-ttu-id="7a105-115">Делетеддате</span><span class="sxs-lookup"><span data-stu-id="7a105-115">deletedDate</span></span>       | <span data-ttu-id="7a105-116">Дата</span><span class="sxs-lookup"><span data-stu-id="7a105-116">Date</span></span>              |
| <span data-ttu-id="7a105-117">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="7a105-117">lastActivityDate</span></span>  | <span data-ttu-id="7a105-118">Дата</span><span class="sxs-lookup"><span data-stu-id="7a105-118">Date</span></span>              |
| <span data-ttu-id="7a105-119">Сендкаунт</span><span class="sxs-lookup"><span data-stu-id="7a105-119">sendCount</span></span>         | <span data-ttu-id="7a105-120">Int64</span><span class="sxs-lookup"><span data-stu-id="7a105-120">Int64</span></span>             |
| <span data-ttu-id="7a105-121">Рецеивекаунт</span><span class="sxs-lookup"><span data-stu-id="7a105-121">receiveCount</span></span>      | <span data-ttu-id="7a105-122">Int64</span><span class="sxs-lookup"><span data-stu-id="7a105-122">Int64</span></span>             |
| <span data-ttu-id="7a105-123">Реадкаунт</span><span class="sxs-lookup"><span data-stu-id="7a105-123">readCount</span></span>         | <span data-ttu-id="7a105-124">Int64</span><span class="sxs-lookup"><span data-stu-id="7a105-124">Int64</span></span>             |
| <span data-ttu-id="7a105-125">Ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="7a105-125">assignedProducts</span></span>  | <span data-ttu-id="7a105-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7a105-126">String collection</span></span> |
| <span data-ttu-id="7a105-127">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="7a105-127">reportPeriod</span></span>      | <span data-ttu-id="7a105-128">String</span><span class="sxs-lookup"><span data-stu-id="7a105-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="7a105-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7a105-129">JSON representation</span></span>

<span data-ttu-id="7a105-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a105-130">The following is a JSON representation of the resource.</span></span>

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
