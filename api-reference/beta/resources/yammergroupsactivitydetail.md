---
title: Тип ресурса Яммерграупсактивитидетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551423"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="02f0a-103">Тип ресурса Яммерграупсактивитидетаил</span><span class="sxs-lookup"><span data-stu-id="02f0a-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="02f0a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="02f0a-104">Properties</span></span>

| <span data-ttu-id="02f0a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="02f0a-105">Property</span></span>           | <span data-ttu-id="02f0a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="02f0a-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="02f0a-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="02f0a-107">reportRefreshDate</span></span>  | <span data-ttu-id="02f0a-108">Дата</span><span class="sxs-lookup"><span data-stu-id="02f0a-108">Date</span></span>    |
| <span data-ttu-id="02f0a-109">Граупдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="02f0a-109">groupDisplayName</span></span>   | <span data-ttu-id="02f0a-110">String</span><span class="sxs-lookup"><span data-stu-id="02f0a-110">String</span></span>  |
| <span data-ttu-id="02f0a-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="02f0a-111">isDeleted</span></span>          | <span data-ttu-id="02f0a-112">Логический</span><span class="sxs-lookup"><span data-stu-id="02f0a-112">Boolean</span></span> |
| <span data-ttu-id="02f0a-113">ОвнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="02f0a-113">ownerPrincipalName</span></span> | <span data-ttu-id="02f0a-114">String</span><span class="sxs-lookup"><span data-stu-id="02f0a-114">String</span></span>  |
| <span data-ttu-id="02f0a-115">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="02f0a-115">lastActivityDate</span></span>   | <span data-ttu-id="02f0a-116">Дата</span><span class="sxs-lookup"><span data-stu-id="02f0a-116">Date</span></span>    |
| <span data-ttu-id="02f0a-117">groupType</span><span class="sxs-lookup"><span data-stu-id="02f0a-117">groupType</span></span>          | <span data-ttu-id="02f0a-118">String</span><span class="sxs-lookup"><span data-stu-id="02f0a-118">String</span></span>  |
| <span data-ttu-id="02f0a-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="02f0a-119">office365Connected</span></span> | <span data-ttu-id="02f0a-120">Логический</span><span class="sxs-lookup"><span data-stu-id="02f0a-120">Boolean</span></span> |
| <span data-ttu-id="02f0a-121">Мемберкаунт</span><span class="sxs-lookup"><span data-stu-id="02f0a-121">memberCount</span></span>        | <span data-ttu-id="02f0a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="02f0a-122">Int64</span></span>   |
| <span data-ttu-id="02f0a-123">Постедкаунт</span><span class="sxs-lookup"><span data-stu-id="02f0a-123">postedCount</span></span>        | <span data-ttu-id="02f0a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="02f0a-124">Int64</span></span>   |
| <span data-ttu-id="02f0a-125">Реадкаунт</span><span class="sxs-lookup"><span data-stu-id="02f0a-125">readCount</span></span>          | <span data-ttu-id="02f0a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="02f0a-126">Int64</span></span>   |
| <span data-ttu-id="02f0a-127">Ликедкаунт</span><span class="sxs-lookup"><span data-stu-id="02f0a-127">likedCount</span></span>         | <span data-ttu-id="02f0a-128">Int64</span><span class="sxs-lookup"><span data-stu-id="02f0a-128">Int64</span></span>   |
| <span data-ttu-id="02f0a-129">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="02f0a-129">reportPeriod</span></span>       | <span data-ttu-id="02f0a-130">String</span><span class="sxs-lookup"><span data-stu-id="02f0a-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="02f0a-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="02f0a-131">JSON representation</span></span>

<span data-ttu-id="02f0a-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02f0a-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "office365Connected": true, 
  "memberCount": 1024, 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "reportPeriod": "String"
}
```
