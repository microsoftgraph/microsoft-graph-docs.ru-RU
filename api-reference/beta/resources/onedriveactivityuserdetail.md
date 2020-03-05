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
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="b085c-103">Тип ресурса Онедривеактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="b085c-103">oneDriveActivityUserDetail resource type</span></span>

<span data-ttu-id="b085c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b085c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b085c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b085c-105">Properties</span></span>

| <span data-ttu-id="b085c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b085c-106">Property</span></span>                  | <span data-ttu-id="b085c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b085c-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="b085c-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="b085c-108">reportRefreshDate</span></span>         | <span data-ttu-id="b085c-109">Дата</span><span class="sxs-lookup"><span data-stu-id="b085c-109">Date</span></span>              |
| <span data-ttu-id="b085c-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b085c-110">userPrincipalName</span></span>         | <span data-ttu-id="b085c-111">String</span><span class="sxs-lookup"><span data-stu-id="b085c-111">String</span></span>            |
| <span data-ttu-id="b085c-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b085c-112">isDeleted</span></span>                 | <span data-ttu-id="b085c-113">Логический</span><span class="sxs-lookup"><span data-stu-id="b085c-113">Boolean</span></span>           |
| <span data-ttu-id="b085c-114">делетеддате</span><span class="sxs-lookup"><span data-stu-id="b085c-114">deletedDate</span></span>               | <span data-ttu-id="b085c-115">Дата</span><span class="sxs-lookup"><span data-stu-id="b085c-115">Date</span></span>              |
| <span data-ttu-id="b085c-116">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="b085c-116">lastActivityDate</span></span>          | <span data-ttu-id="b085c-117">Дата</span><span class="sxs-lookup"><span data-stu-id="b085c-117">Date</span></span>              |
| <span data-ttu-id="b085c-118">виеведоредитедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="b085c-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="b085c-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b085c-119">Int64</span></span>             |
| <span data-ttu-id="b085c-120">синцедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="b085c-120">syncedFileCount</span></span>           | <span data-ttu-id="b085c-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b085c-121">Int64</span></span>             |
| <span data-ttu-id="b085c-122">шарединтерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="b085c-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="b085c-123">Int64</span><span class="sxs-lookup"><span data-stu-id="b085c-123">Int64</span></span>             |
| <span data-ttu-id="b085c-124">шаредекстерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="b085c-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="b085c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="b085c-125">Int64</span></span>             |
| <span data-ttu-id="b085c-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="b085c-126">assignedProducts</span></span>          | <span data-ttu-id="b085c-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b085c-127">String collection</span></span> |
| <span data-ttu-id="b085c-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="b085c-128">reportPeriod</span></span>              | <span data-ttu-id="b085c-129">String</span><span class="sxs-lookup"><span data-stu-id="b085c-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="b085c-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b085c-130">JSON representation</span></span>

<span data-ttu-id="b085c-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b085c-131">The following is a JSON representation of the resource.</span></span>

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
