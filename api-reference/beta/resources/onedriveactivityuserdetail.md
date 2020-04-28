---
title: Тип ресурса Онедривеактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 22702a392a76a21951c24667da0e8a1e61c8b36c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522395"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="4251e-103">Тип ресурса Онедривеактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="4251e-103">oneDriveActivityUserDetail resource type</span></span>

<span data-ttu-id="4251e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4251e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="4251e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4251e-105">Properties</span></span>

| <span data-ttu-id="4251e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4251e-106">Property</span></span>                  | <span data-ttu-id="4251e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4251e-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="4251e-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="4251e-108">reportRefreshDate</span></span>         | <span data-ttu-id="4251e-109">Дата</span><span class="sxs-lookup"><span data-stu-id="4251e-109">Date</span></span>              |
| <span data-ttu-id="4251e-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4251e-110">userPrincipalName</span></span>         | <span data-ttu-id="4251e-111">String</span><span class="sxs-lookup"><span data-stu-id="4251e-111">String</span></span>            |
| <span data-ttu-id="4251e-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4251e-112">isDeleted</span></span>                 | <span data-ttu-id="4251e-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="4251e-113">Boolean</span></span>           |
| <span data-ttu-id="4251e-114">делетеддате</span><span class="sxs-lookup"><span data-stu-id="4251e-114">deletedDate</span></span>               | <span data-ttu-id="4251e-115">Дата</span><span class="sxs-lookup"><span data-stu-id="4251e-115">Date</span></span>              |
| <span data-ttu-id="4251e-116">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="4251e-116">lastActivityDate</span></span>          | <span data-ttu-id="4251e-117">Дата</span><span class="sxs-lookup"><span data-stu-id="4251e-117">Date</span></span>              |
| <span data-ttu-id="4251e-118">виеведоредитедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="4251e-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="4251e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="4251e-119">Int64</span></span>             |
| <span data-ttu-id="4251e-120">синцедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="4251e-120">syncedFileCount</span></span>           | <span data-ttu-id="4251e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="4251e-121">Int64</span></span>             |
| <span data-ttu-id="4251e-122">шарединтерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="4251e-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="4251e-123">Int64</span><span class="sxs-lookup"><span data-stu-id="4251e-123">Int64</span></span>             |
| <span data-ttu-id="4251e-124">шаредекстерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="4251e-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="4251e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="4251e-125">Int64</span></span>             |
| <span data-ttu-id="4251e-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="4251e-126">assignedProducts</span></span>          | <span data-ttu-id="4251e-127">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4251e-127">String collection</span></span> |
| <span data-ttu-id="4251e-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="4251e-128">reportPeriod</span></span>              | <span data-ttu-id="4251e-129">String</span><span class="sxs-lookup"><span data-stu-id="4251e-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="4251e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4251e-130">JSON representation</span></span>

<span data-ttu-id="4251e-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4251e-131">The following is a JSON representation of the resource.</span></span>

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
