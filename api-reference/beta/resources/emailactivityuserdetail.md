---
title: Тип ресурса Емаилактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 54efe4d3a24a0409e8daa2ebde6d4aff4b729118
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440571"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="f3702-103">Тип ресурса Емаилактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="f3702-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="f3702-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3702-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f3702-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3702-105">Properties</span></span>

| <span data-ttu-id="f3702-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3702-106">Property</span></span>          | <span data-ttu-id="f3702-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f3702-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="f3702-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="f3702-108">reportRefreshDate</span></span> | <span data-ttu-id="f3702-109">Дата</span><span class="sxs-lookup"><span data-stu-id="f3702-109">Date</span></span>              |
| <span data-ttu-id="f3702-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f3702-110">userPrincipalName</span></span> | <span data-ttu-id="f3702-111">String</span><span class="sxs-lookup"><span data-stu-id="f3702-111">String</span></span>            |
| <span data-ttu-id="f3702-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f3702-112">displayName</span></span>       | <span data-ttu-id="f3702-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f3702-113">String</span></span>            |
| <span data-ttu-id="f3702-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f3702-114">isDeleted</span></span>         | <span data-ttu-id="f3702-115">Логическое</span><span class="sxs-lookup"><span data-stu-id="f3702-115">Boolean</span></span>           |
| <span data-ttu-id="f3702-116">делетеддате</span><span class="sxs-lookup"><span data-stu-id="f3702-116">deletedDate</span></span>       | <span data-ttu-id="f3702-117">Дата</span><span class="sxs-lookup"><span data-stu-id="f3702-117">Date</span></span>              |
| <span data-ttu-id="f3702-118">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="f3702-118">lastActivityDate</span></span>  | <span data-ttu-id="f3702-119">Дата</span><span class="sxs-lookup"><span data-stu-id="f3702-119">Date</span></span>              |
| <span data-ttu-id="f3702-120">сендкаунт</span><span class="sxs-lookup"><span data-stu-id="f3702-120">sendCount</span></span>         | <span data-ttu-id="f3702-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f3702-121">Int64</span></span>             |
| <span data-ttu-id="f3702-122">рецеивекаунт</span><span class="sxs-lookup"><span data-stu-id="f3702-122">receiveCount</span></span>      | <span data-ttu-id="f3702-123">Int64</span><span class="sxs-lookup"><span data-stu-id="f3702-123">Int64</span></span>             |
| <span data-ttu-id="f3702-124">реадкаунт</span><span class="sxs-lookup"><span data-stu-id="f3702-124">readCount</span></span>         | <span data-ttu-id="f3702-125">Int64</span><span class="sxs-lookup"><span data-stu-id="f3702-125">Int64</span></span>             |
| <span data-ttu-id="f3702-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="f3702-126">assignedProducts</span></span>  | <span data-ttu-id="f3702-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f3702-127">String collection</span></span> |
| <span data-ttu-id="f3702-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="f3702-128">reportPeriod</span></span>      | <span data-ttu-id="f3702-129">String</span><span class="sxs-lookup"><span data-stu-id="f3702-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="f3702-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3702-130">JSON representation</span></span>

<span data-ttu-id="f3702-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3702-131">The following is a JSON representation of the resource.</span></span>

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
