---
title: Тип ресурса Теамсусерактивитюсердетаил
description: Ниже приведен пример JSON репресентаион для ресурса.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 237cfc933cbabd628320131866f7bf24ba0195c7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519815"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="56240-103">Тип ресурса Теамсусерактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="56240-103">teamsUserActivityUserDetail resource type</span></span>

<span data-ttu-id="56240-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="56240-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="56240-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="56240-105">Properties</span></span>

| <span data-ttu-id="56240-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="56240-106">Property</span></span>                | <span data-ttu-id="56240-107">Тип</span><span class="sxs-lookup"><span data-stu-id="56240-107">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="56240-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="56240-108">reportRefreshDate</span></span>       | <span data-ttu-id="56240-109">Дата</span><span class="sxs-lookup"><span data-stu-id="56240-109">Date</span></span>              |
| <span data-ttu-id="56240-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="56240-110">userPrincipalName</span></span>       | <span data-ttu-id="56240-111">String</span><span class="sxs-lookup"><span data-stu-id="56240-111">String</span></span>            |
| <span data-ttu-id="56240-112">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="56240-112">lastActivityDate</span></span>        | <span data-ttu-id="56240-113">Дата</span><span class="sxs-lookup"><span data-stu-id="56240-113">Date</span></span>              |
| <span data-ttu-id="56240-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="56240-114">isDeleted</span></span>               | <span data-ttu-id="56240-115">Логический</span><span class="sxs-lookup"><span data-stu-id="56240-115">Boolean</span></span>           |
| <span data-ttu-id="56240-116">делетеддате</span><span class="sxs-lookup"><span data-stu-id="56240-116">deletedDate</span></span>             | <span data-ttu-id="56240-117">Дата</span><span class="sxs-lookup"><span data-stu-id="56240-117">Date</span></span>              |
| <span data-ttu-id="56240-118">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="56240-118">assignedProducts</span></span>        | <span data-ttu-id="56240-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="56240-119">String collection</span></span> |
| <span data-ttu-id="56240-120">теамчатмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="56240-120">teamChatMessageCount</span></span>    | <span data-ttu-id="56240-121">Int64</span><span class="sxs-lookup"><span data-stu-id="56240-121">Int64</span></span>             |
| <span data-ttu-id="56240-122">приватечатмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="56240-122">privateChatMessageCount</span></span> | <span data-ttu-id="56240-123">Int64</span><span class="sxs-lookup"><span data-stu-id="56240-123">Int64</span></span>             |
| <span data-ttu-id="56240-124">каллкаунт</span><span class="sxs-lookup"><span data-stu-id="56240-124">callCount</span></span>               | <span data-ttu-id="56240-125">Int64</span><span class="sxs-lookup"><span data-stu-id="56240-125">Int64</span></span>             |
| <span data-ttu-id="56240-126">митингкаунт</span><span class="sxs-lookup"><span data-stu-id="56240-126">meetingCount</span></span>            | <span data-ttu-id="56240-127">Int64</span><span class="sxs-lookup"><span data-stu-id="56240-127">Int64</span></span>             |
| <span data-ttu-id="56240-128">хасосерактион</span><span class="sxs-lookup"><span data-stu-id="56240-128">hasOtherAction</span></span>          | <span data-ttu-id="56240-129">Логический</span><span class="sxs-lookup"><span data-stu-id="56240-129">Boolean</span></span>           |
| <span data-ttu-id="56240-130">репортпериод</span><span class="sxs-lookup"><span data-stu-id="56240-130">reportPeriod</span></span>            | <span data-ttu-id="56240-131">String</span><span class="sxs-lookup"><span data-stu-id="56240-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="56240-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56240-132">JSON representation</span></span>

<span data-ttu-id="56240-133">Ниже приведен пример JSON репресентаион для ресурса.</span><span class="sxs-lookup"><span data-stu-id="56240-133">The following is a JSON representaion of the resource.</span></span>

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
