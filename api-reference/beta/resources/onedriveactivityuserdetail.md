---
title: Тип ресурса Онедривеактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 4021d1bdfb9322dbef75264ab88bb8b3a71c20e7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812150"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="76eaa-103">Тип ресурса Онедривеактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="76eaa-103">oneDriveActivityUserDetail resource type</span></span>

<span data-ttu-id="76eaa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76eaa-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="76eaa-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="76eaa-105">Properties</span></span>

| <span data-ttu-id="76eaa-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="76eaa-106">Property</span></span>                  | <span data-ttu-id="76eaa-107">Тип</span><span class="sxs-lookup"><span data-stu-id="76eaa-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="76eaa-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="76eaa-108">reportRefreshDate</span></span>         | <span data-ttu-id="76eaa-109">Дата</span><span class="sxs-lookup"><span data-stu-id="76eaa-109">Date</span></span>              |
| <span data-ttu-id="76eaa-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="76eaa-110">userPrincipalName</span></span>         | <span data-ttu-id="76eaa-111">String</span><span class="sxs-lookup"><span data-stu-id="76eaa-111">String</span></span>            |
| <span data-ttu-id="76eaa-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="76eaa-112">isDeleted</span></span>                 | <span data-ttu-id="76eaa-113">Логический</span><span class="sxs-lookup"><span data-stu-id="76eaa-113">Boolean</span></span>           |
| <span data-ttu-id="76eaa-114">делетеддате</span><span class="sxs-lookup"><span data-stu-id="76eaa-114">deletedDate</span></span>               | <span data-ttu-id="76eaa-115">Дата</span><span class="sxs-lookup"><span data-stu-id="76eaa-115">Date</span></span>              |
| <span data-ttu-id="76eaa-116">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="76eaa-116">lastActivityDate</span></span>          | <span data-ttu-id="76eaa-117">Дата</span><span class="sxs-lookup"><span data-stu-id="76eaa-117">Date</span></span>              |
| <span data-ttu-id="76eaa-118">виеведоредитедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="76eaa-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="76eaa-119">Int64</span><span class="sxs-lookup"><span data-stu-id="76eaa-119">Int64</span></span>             |
| <span data-ttu-id="76eaa-120">синцедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="76eaa-120">syncedFileCount</span></span>           | <span data-ttu-id="76eaa-121">Int64</span><span class="sxs-lookup"><span data-stu-id="76eaa-121">Int64</span></span>             |
| <span data-ttu-id="76eaa-122">шарединтерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="76eaa-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="76eaa-123">Int64</span><span class="sxs-lookup"><span data-stu-id="76eaa-123">Int64</span></span>             |
| <span data-ttu-id="76eaa-124">шаредекстерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="76eaa-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="76eaa-125">Int64</span><span class="sxs-lookup"><span data-stu-id="76eaa-125">Int64</span></span>             |
| <span data-ttu-id="76eaa-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="76eaa-126">assignedProducts</span></span>          | <span data-ttu-id="76eaa-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="76eaa-127">String collection</span></span> |
| <span data-ttu-id="76eaa-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="76eaa-128">reportPeriod</span></span>              | <span data-ttu-id="76eaa-129">String</span><span class="sxs-lookup"><span data-stu-id="76eaa-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="76eaa-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="76eaa-130">JSON representation</span></span>

<span data-ttu-id="76eaa-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76eaa-131">The following is a JSON representation of the resource.</span></span>

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
