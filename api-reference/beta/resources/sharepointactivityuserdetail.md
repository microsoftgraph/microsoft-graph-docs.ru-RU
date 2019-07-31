---
title: Тип ресурса Шарепоинтактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 3d1c1f1b2bcf919769009bbb65a917c4b9cb84f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008434"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="c77aa-103">Тип ресурса Шарепоинтактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="c77aa-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c77aa-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c77aa-104">Properties</span></span>

| <span data-ttu-id="c77aa-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c77aa-105">Property</span></span>                  | <span data-ttu-id="c77aa-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c77aa-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="c77aa-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="c77aa-107">reportRefreshDate</span></span>         | <span data-ttu-id="c77aa-108">Дата</span><span class="sxs-lookup"><span data-stu-id="c77aa-108">Date</span></span>              |
| <span data-ttu-id="c77aa-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c77aa-109">userPrincipalName</span></span>         | <span data-ttu-id="c77aa-110">String</span><span class="sxs-lookup"><span data-stu-id="c77aa-110">String</span></span>            |
| <span data-ttu-id="c77aa-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c77aa-111">isDeleted</span></span>                 | <span data-ttu-id="c77aa-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c77aa-112">Boolean</span></span>           |
| <span data-ttu-id="c77aa-113">Делетеддате</span><span class="sxs-lookup"><span data-stu-id="c77aa-113">deletedDate</span></span>               | <span data-ttu-id="c77aa-114">Дата</span><span class="sxs-lookup"><span data-stu-id="c77aa-114">Date</span></span>              |
| <span data-ttu-id="c77aa-115">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="c77aa-115">lastActivityDate</span></span>          | <span data-ttu-id="c77aa-116">Дата</span><span class="sxs-lookup"><span data-stu-id="c77aa-116">Date</span></span>              |
| <span data-ttu-id="c77aa-117">Виеведоредитедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="c77aa-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="c77aa-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c77aa-118">Int64</span></span>             |
| <span data-ttu-id="c77aa-119">Синцедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="c77aa-119">syncedFileCount</span></span>           | <span data-ttu-id="c77aa-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c77aa-120">Int64</span></span>             |
| <span data-ttu-id="c77aa-121">Шарединтерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="c77aa-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="c77aa-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c77aa-122">Int64</span></span>             |
| <span data-ttu-id="c77aa-123">Шаредекстерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="c77aa-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="c77aa-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c77aa-124">Int64</span></span>             |
| <span data-ttu-id="c77aa-125">Виситедпажекаунт</span><span class="sxs-lookup"><span data-stu-id="c77aa-125">visitedPageCount</span></span>          | <span data-ttu-id="c77aa-126">Int64</span><span class="sxs-lookup"><span data-stu-id="c77aa-126">Int64</span></span>             |
| <span data-ttu-id="c77aa-127">Ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="c77aa-127">assignedProducts</span></span>          | <span data-ttu-id="c77aa-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c77aa-128">String collection</span></span> |
| <span data-ttu-id="c77aa-129">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="c77aa-129">reportPeriod</span></span>              | <span data-ttu-id="c77aa-130">String</span><span class="sxs-lookup"><span data-stu-id="c77aa-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="c77aa-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c77aa-131">JSON representation</span></span>

<span data-ttu-id="c77aa-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c77aa-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "viewedOrEditedFileCount": 1024, 
  "syncedFileCount": 1024, 
  "sharedInternallyFileCount": 1024, 
  "sharedExternallyFileCount": 1024, 
  "visitedPageCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
