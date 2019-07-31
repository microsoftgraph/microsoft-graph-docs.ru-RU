---
title: Тип ресурса Теамсусерактивитюсердетаил
description: Ниже приведен пример JSON репресентаион для ресурса.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cbe6297388907f28f8841e0a1dcb2ec3ae788844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964356"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="a5287-103">Тип ресурса Теамсусерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="a5287-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a5287-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5287-104">Properties</span></span>

| <span data-ttu-id="a5287-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5287-105">Property</span></span>                | <span data-ttu-id="a5287-106">Тип</span><span class="sxs-lookup"><span data-stu-id="a5287-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="a5287-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="a5287-107">reportRefreshDate</span></span>       | <span data-ttu-id="a5287-108">Дата</span><span class="sxs-lookup"><span data-stu-id="a5287-108">Date</span></span>              |
| <span data-ttu-id="a5287-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a5287-109">userPrincipalName</span></span>       | <span data-ttu-id="a5287-110">String</span><span class="sxs-lookup"><span data-stu-id="a5287-110">String</span></span>            |
| <span data-ttu-id="a5287-111">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="a5287-111">lastActivityDate</span></span>        | <span data-ttu-id="a5287-112">Дата</span><span class="sxs-lookup"><span data-stu-id="a5287-112">Date</span></span>              |
| <span data-ttu-id="a5287-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a5287-113">isDeleted</span></span>               | <span data-ttu-id="a5287-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5287-114">Boolean</span></span>           |
| <span data-ttu-id="a5287-115">Делетеддате</span><span class="sxs-lookup"><span data-stu-id="a5287-115">deletedDate</span></span>             | <span data-ttu-id="a5287-116">Дата</span><span class="sxs-lookup"><span data-stu-id="a5287-116">Date</span></span>              |
| <span data-ttu-id="a5287-117">Ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="a5287-117">assignedProducts</span></span>        | <span data-ttu-id="a5287-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a5287-118">String collection</span></span> |
| <span data-ttu-id="a5287-119">Теамчатмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="a5287-119">teamChatMessageCount</span></span>    | <span data-ttu-id="a5287-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a5287-120">Int64</span></span>             |
| <span data-ttu-id="a5287-121">Приватечатмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="a5287-121">privateChatMessageCount</span></span> | <span data-ttu-id="a5287-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a5287-122">Int64</span></span>             |
| <span data-ttu-id="a5287-123">Каллкаунт</span><span class="sxs-lookup"><span data-stu-id="a5287-123">callCount</span></span>               | <span data-ttu-id="a5287-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a5287-124">Int64</span></span>             |
| <span data-ttu-id="a5287-125">Митингкаунт</span><span class="sxs-lookup"><span data-stu-id="a5287-125">meetingCount</span></span>            | <span data-ttu-id="a5287-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a5287-126">Int64</span></span>             |
| <span data-ttu-id="a5287-127">Хасосерактион</span><span class="sxs-lookup"><span data-stu-id="a5287-127">hasOtherAction</span></span>          | <span data-ttu-id="a5287-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5287-128">Boolean</span></span>           |
| <span data-ttu-id="a5287-129">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="a5287-129">reportPeriod</span></span>            | <span data-ttu-id="a5287-130">String</span><span class="sxs-lookup"><span data-stu-id="a5287-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="a5287-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5287-131">JSON representation</span></span>

<span data-ttu-id="a5287-132">Ниже приведен пример JSON репресентаион для ресурса.</span><span class="sxs-lookup"><span data-stu-id="a5287-132">The following is a JSON representaion of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
