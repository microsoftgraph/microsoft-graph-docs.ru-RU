---
title: Тип ресурса Шарепоинтактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 20b99e3c6431d945200db868cc02302600e0e76c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807117"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="865ae-103">Тип ресурса Шарепоинтактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="865ae-103">sharePointActivityUserDetail resource type</span></span>

<span data-ttu-id="865ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="865ae-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="865ae-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="865ae-105">Properties</span></span>

| <span data-ttu-id="865ae-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="865ae-106">Property</span></span>                  | <span data-ttu-id="865ae-107">Тип</span><span class="sxs-lookup"><span data-stu-id="865ae-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="865ae-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="865ae-108">reportRefreshDate</span></span>         | <span data-ttu-id="865ae-109">Дата</span><span class="sxs-lookup"><span data-stu-id="865ae-109">Date</span></span>              |
| <span data-ttu-id="865ae-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="865ae-110">userPrincipalName</span></span>         | <span data-ttu-id="865ae-111">String</span><span class="sxs-lookup"><span data-stu-id="865ae-111">String</span></span>            |
| <span data-ttu-id="865ae-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="865ae-112">isDeleted</span></span>                 | <span data-ttu-id="865ae-113">Логический</span><span class="sxs-lookup"><span data-stu-id="865ae-113">Boolean</span></span>           |
| <span data-ttu-id="865ae-114">делетеддате</span><span class="sxs-lookup"><span data-stu-id="865ae-114">deletedDate</span></span>               | <span data-ttu-id="865ae-115">Дата</span><span class="sxs-lookup"><span data-stu-id="865ae-115">Date</span></span>              |
| <span data-ttu-id="865ae-116">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="865ae-116">lastActivityDate</span></span>          | <span data-ttu-id="865ae-117">Дата</span><span class="sxs-lookup"><span data-stu-id="865ae-117">Date</span></span>              |
| <span data-ttu-id="865ae-118">виеведоредитедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="865ae-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="865ae-119">Int64</span><span class="sxs-lookup"><span data-stu-id="865ae-119">Int64</span></span>             |
| <span data-ttu-id="865ae-120">синцедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="865ae-120">syncedFileCount</span></span>           | <span data-ttu-id="865ae-121">Int64</span><span class="sxs-lookup"><span data-stu-id="865ae-121">Int64</span></span>             |
| <span data-ttu-id="865ae-122">шарединтерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="865ae-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="865ae-123">Int64</span><span class="sxs-lookup"><span data-stu-id="865ae-123">Int64</span></span>             |
| <span data-ttu-id="865ae-124">шаредекстерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="865ae-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="865ae-125">Int64</span><span class="sxs-lookup"><span data-stu-id="865ae-125">Int64</span></span>             |
| <span data-ttu-id="865ae-126">виситедпажекаунт</span><span class="sxs-lookup"><span data-stu-id="865ae-126">visitedPageCount</span></span>          | <span data-ttu-id="865ae-127">Int64</span><span class="sxs-lookup"><span data-stu-id="865ae-127">Int64</span></span>             |
| <span data-ttu-id="865ae-128">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="865ae-128">assignedProducts</span></span>          | <span data-ttu-id="865ae-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="865ae-129">String collection</span></span> |
| <span data-ttu-id="865ae-130">репортпериод</span><span class="sxs-lookup"><span data-stu-id="865ae-130">reportPeriod</span></span>              | <span data-ttu-id="865ae-131">String</span><span class="sxs-lookup"><span data-stu-id="865ae-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="865ae-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="865ae-132">JSON representation</span></span>

<span data-ttu-id="865ae-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="865ae-133">The following is a JSON representation of the resource.</span></span>

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
