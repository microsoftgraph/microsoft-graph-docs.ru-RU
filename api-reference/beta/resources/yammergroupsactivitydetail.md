---
title: Тип ресурса Яммерграупсактивитидетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: f16eda3f28556a18c47c68d532ace4244edfad19
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963754"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="8cb71-103">Тип ресурса Яммерграупсактивитидетаил</span><span class="sxs-lookup"><span data-stu-id="8cb71-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8cb71-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cb71-104">Properties</span></span>

| <span data-ttu-id="8cb71-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cb71-105">Property</span></span>           | <span data-ttu-id="8cb71-106">Тип</span><span class="sxs-lookup"><span data-stu-id="8cb71-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="8cb71-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="8cb71-107">reportRefreshDate</span></span>  | <span data-ttu-id="8cb71-108">Дата</span><span class="sxs-lookup"><span data-stu-id="8cb71-108">Date</span></span>    |
| <span data-ttu-id="8cb71-109">Граупдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="8cb71-109">groupDisplayName</span></span>   | <span data-ttu-id="8cb71-110">String</span><span class="sxs-lookup"><span data-stu-id="8cb71-110">String</span></span>  |
| <span data-ttu-id="8cb71-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8cb71-111">isDeleted</span></span>          | <span data-ttu-id="8cb71-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cb71-112">Boolean</span></span> |
| <span data-ttu-id="8cb71-113">ОвнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="8cb71-113">ownerPrincipalName</span></span> | <span data-ttu-id="8cb71-114">String</span><span class="sxs-lookup"><span data-stu-id="8cb71-114">String</span></span>  |
| <span data-ttu-id="8cb71-115">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="8cb71-115">lastActivityDate</span></span>   | <span data-ttu-id="8cb71-116">Дата</span><span class="sxs-lookup"><span data-stu-id="8cb71-116">Date</span></span>    |
| <span data-ttu-id="8cb71-117">groupType</span><span class="sxs-lookup"><span data-stu-id="8cb71-117">groupType</span></span>          | <span data-ttu-id="8cb71-118">String</span><span class="sxs-lookup"><span data-stu-id="8cb71-118">String</span></span>  |
| <span data-ttu-id="8cb71-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="8cb71-119">office365Connected</span></span> | <span data-ttu-id="8cb71-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cb71-120">Boolean</span></span> |
| <span data-ttu-id="8cb71-121">Мемберкаунт</span><span class="sxs-lookup"><span data-stu-id="8cb71-121">memberCount</span></span>        | <span data-ttu-id="8cb71-122">Int64</span><span class="sxs-lookup"><span data-stu-id="8cb71-122">Int64</span></span>   |
| <span data-ttu-id="8cb71-123">Постедкаунт</span><span class="sxs-lookup"><span data-stu-id="8cb71-123">postedCount</span></span>        | <span data-ttu-id="8cb71-124">Int64</span><span class="sxs-lookup"><span data-stu-id="8cb71-124">Int64</span></span>   |
| <span data-ttu-id="8cb71-125">Реадкаунт</span><span class="sxs-lookup"><span data-stu-id="8cb71-125">readCount</span></span>          | <span data-ttu-id="8cb71-126">Int64</span><span class="sxs-lookup"><span data-stu-id="8cb71-126">Int64</span></span>   |
| <span data-ttu-id="8cb71-127">Ликедкаунт</span><span class="sxs-lookup"><span data-stu-id="8cb71-127">likedCount</span></span>         | <span data-ttu-id="8cb71-128">Int64</span><span class="sxs-lookup"><span data-stu-id="8cb71-128">Int64</span></span>   |
| <span data-ttu-id="8cb71-129">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="8cb71-129">reportPeriod</span></span>       | <span data-ttu-id="8cb71-130">String</span><span class="sxs-lookup"><span data-stu-id="8cb71-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8cb71-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cb71-131">JSON representation</span></span>

<span data-ttu-id="8cb71-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cb71-132">The following is a JSON representation of the resource.</span></span>

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
