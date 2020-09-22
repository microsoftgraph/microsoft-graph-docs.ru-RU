---
title: Тип ресурса Онедривеусажеаккаунтдетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 6e355e1f71d493b30ffb2fe41816208dfe4816e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039288"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="3f901-103">Тип ресурса Онедривеусажеаккаунтдетаил</span><span class="sxs-lookup"><span data-stu-id="3f901-103">oneDriveUsageAccountDetail resource type</span></span>

<span data-ttu-id="3f901-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f901-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3f901-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f901-105">Properties</span></span>

| <span data-ttu-id="3f901-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f901-106">Property</span></span>                | <span data-ttu-id="3f901-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3f901-107">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="3f901-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="3f901-108">reportRefreshDate</span></span>       | <span data-ttu-id="3f901-109">Дата</span><span class="sxs-lookup"><span data-stu-id="3f901-109">Date</span></span>    |
| <span data-ttu-id="3f901-110">siteUrl</span><span class="sxs-lookup"><span data-stu-id="3f901-110">siteUrl</span></span>                 | <span data-ttu-id="3f901-111">String</span><span class="sxs-lookup"><span data-stu-id="3f901-111">String</span></span>  |
| <span data-ttu-id="3f901-112">овнердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="3f901-112">ownerDisplayName</span></span>        | <span data-ttu-id="3f901-113">String</span><span class="sxs-lookup"><span data-stu-id="3f901-113">String</span></span>  |
| <span data-ttu-id="3f901-114">овнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="3f901-114">ownerPrincipalName</span></span>      | <span data-ttu-id="3f901-115">String</span><span class="sxs-lookup"><span data-stu-id="3f901-115">String</span></span>  |
| <span data-ttu-id="3f901-116">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3f901-116">isDeleted</span></span>               | <span data-ttu-id="3f901-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f901-117">Boolean</span></span> |
| <span data-ttu-id="3f901-118">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="3f901-118">lastActivityDate</span></span>        | <span data-ttu-id="3f901-119">Дата</span><span class="sxs-lookup"><span data-stu-id="3f901-119">Date</span></span>    |
| <span data-ttu-id="3f901-120">филекаунт</span><span class="sxs-lookup"><span data-stu-id="3f901-120">fileCount</span></span>               | <span data-ttu-id="3f901-121">Int64</span><span class="sxs-lookup"><span data-stu-id="3f901-121">Int64</span></span>   |
| <span data-ttu-id="3f901-122">активефилекаунт</span><span class="sxs-lookup"><span data-stu-id="3f901-122">activeFileCount</span></span>         | <span data-ttu-id="3f901-123">Int64</span><span class="sxs-lookup"><span data-stu-id="3f901-123">Int64</span></span>   |
| <span data-ttu-id="3f901-124">сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="3f901-124">storageUsedInBytes</span></span>      | <span data-ttu-id="3f901-125">Int64</span><span class="sxs-lookup"><span data-stu-id="3f901-125">Int64</span></span>   |
| <span data-ttu-id="3f901-126">сторажеаллокатединбитес</span><span class="sxs-lookup"><span data-stu-id="3f901-126">storageAllocatedInBytes</span></span> | <span data-ttu-id="3f901-127">Int64</span><span class="sxs-lookup"><span data-stu-id="3f901-127">Int64</span></span>   |
| <span data-ttu-id="3f901-128">репортпериод</span><span class="sxs-lookup"><span data-stu-id="3f901-128">reportPeriod</span></span>            | <span data-ttu-id="3f901-129">String</span><span class="sxs-lookup"><span data-stu-id="3f901-129">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="3f901-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f901-130">JSON representation</span></span>

<span data-ttu-id="3f901-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f901-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteUrl": "String",
  "ownerDisplayName": "String",
  "ownerPrincipalName": "String",
  "isDeleted": true,
  "lastActivityDate": "Date",
  "fileCount": 1024,
  "activeFileCount": 1024,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "reportPeriod": "String"
}
```


