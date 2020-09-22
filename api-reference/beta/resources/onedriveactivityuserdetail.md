---
title: Тип ресурса Онедривеактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 24f6b9da0fb4e4a141872bd00b423b799b880aa6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048865"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="70312-103">Тип ресурса Онедривеактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="70312-103">oneDriveActivityUserDetail resource type</span></span>

<span data-ttu-id="70312-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70312-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="70312-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="70312-105">Properties</span></span>

| <span data-ttu-id="70312-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="70312-106">Property</span></span>                  | <span data-ttu-id="70312-107">Тип</span><span class="sxs-lookup"><span data-stu-id="70312-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="70312-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="70312-108">reportRefreshDate</span></span>         | <span data-ttu-id="70312-109">Дата</span><span class="sxs-lookup"><span data-stu-id="70312-109">Date</span></span>              |
| <span data-ttu-id="70312-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70312-110">userPrincipalName</span></span>         | <span data-ttu-id="70312-111">String</span><span class="sxs-lookup"><span data-stu-id="70312-111">String</span></span>            |
| <span data-ttu-id="70312-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="70312-112">isDeleted</span></span>                 | <span data-ttu-id="70312-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="70312-113">Boolean</span></span>           |
| <span data-ttu-id="70312-114">делетеддате</span><span class="sxs-lookup"><span data-stu-id="70312-114">deletedDate</span></span>               | <span data-ttu-id="70312-115">Дата</span><span class="sxs-lookup"><span data-stu-id="70312-115">Date</span></span>              |
| <span data-ttu-id="70312-116">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="70312-116">lastActivityDate</span></span>          | <span data-ttu-id="70312-117">Дата</span><span class="sxs-lookup"><span data-stu-id="70312-117">Date</span></span>              |
| <span data-ttu-id="70312-118">виеведоредитедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="70312-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="70312-119">Int64</span><span class="sxs-lookup"><span data-stu-id="70312-119">Int64</span></span>             |
| <span data-ttu-id="70312-120">синцедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="70312-120">syncedFileCount</span></span>           | <span data-ttu-id="70312-121">Int64</span><span class="sxs-lookup"><span data-stu-id="70312-121">Int64</span></span>             |
| <span data-ttu-id="70312-122">шарединтерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="70312-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="70312-123">Int64</span><span class="sxs-lookup"><span data-stu-id="70312-123">Int64</span></span>             |
| <span data-ttu-id="70312-124">шаредекстерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="70312-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="70312-125">Int64</span><span class="sxs-lookup"><span data-stu-id="70312-125">Int64</span></span>             |
| <span data-ttu-id="70312-126">ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="70312-126">assignedProducts</span></span>          | <span data-ttu-id="70312-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="70312-127">String collection</span></span> |
| <span data-ttu-id="70312-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="70312-128">reportPeriod</span></span>              | <span data-ttu-id="70312-129">Строка</span><span class="sxs-lookup"><span data-stu-id="70312-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="70312-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70312-130">JSON representation</span></span>

<span data-ttu-id="70312-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70312-131">The following is a JSON representation of the resource.</span></span>

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


