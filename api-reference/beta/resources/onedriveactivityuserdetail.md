---
title: Тип ресурса Онедривеактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: c61db94678ed50e6cc93f123a506ce262616a1ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966484"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="4aed8-103">Тип ресурса Онедривеактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="4aed8-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4aed8-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4aed8-104">Properties</span></span>

| <span data-ttu-id="4aed8-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4aed8-105">Property</span></span>                  | <span data-ttu-id="4aed8-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4aed8-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="4aed8-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="4aed8-107">reportRefreshDate</span></span>         | <span data-ttu-id="4aed8-108">Дата</span><span class="sxs-lookup"><span data-stu-id="4aed8-108">Date</span></span>              |
| <span data-ttu-id="4aed8-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4aed8-109">userPrincipalName</span></span>         | <span data-ttu-id="4aed8-110">String</span><span class="sxs-lookup"><span data-stu-id="4aed8-110">String</span></span>            |
| <span data-ttu-id="4aed8-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4aed8-111">isDeleted</span></span>                 | <span data-ttu-id="4aed8-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aed8-112">Boolean</span></span>           |
| <span data-ttu-id="4aed8-113">Делетеддате</span><span class="sxs-lookup"><span data-stu-id="4aed8-113">deletedDate</span></span>               | <span data-ttu-id="4aed8-114">Дата</span><span class="sxs-lookup"><span data-stu-id="4aed8-114">Date</span></span>              |
| <span data-ttu-id="4aed8-115">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="4aed8-115">lastActivityDate</span></span>          | <span data-ttu-id="4aed8-116">Дата</span><span class="sxs-lookup"><span data-stu-id="4aed8-116">Date</span></span>              |
| <span data-ttu-id="4aed8-117">Виеведоредитедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="4aed8-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="4aed8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4aed8-118">Int64</span></span>             |
| <span data-ttu-id="4aed8-119">Синцедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="4aed8-119">syncedFileCount</span></span>           | <span data-ttu-id="4aed8-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4aed8-120">Int64</span></span>             |
| <span data-ttu-id="4aed8-121">Шарединтерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="4aed8-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="4aed8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4aed8-122">Int64</span></span>             |
| <span data-ttu-id="4aed8-123">Шаредекстерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="4aed8-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="4aed8-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4aed8-124">Int64</span></span>             |
| <span data-ttu-id="4aed8-125">Ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="4aed8-125">assignedProducts</span></span>          | <span data-ttu-id="4aed8-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4aed8-126">String collection</span></span> |
| <span data-ttu-id="4aed8-127">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="4aed8-127">reportPeriod</span></span>              | <span data-ttu-id="4aed8-128">String</span><span class="sxs-lookup"><span data-stu-id="4aed8-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="4aed8-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4aed8-129">JSON representation</span></span>

<span data-ttu-id="4aed8-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4aed8-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
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
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
