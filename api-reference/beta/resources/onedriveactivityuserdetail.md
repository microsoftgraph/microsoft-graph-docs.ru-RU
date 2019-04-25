---
title: Тип ресурса Онедривеактивитюсердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582250"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="42562-103">Тип ресурса Онедривеактивитюсердетаил</span><span class="sxs-lookup"><span data-stu-id="42562-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="42562-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="42562-104">Properties</span></span>

| <span data-ttu-id="42562-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="42562-105">Property</span></span>                  | <span data-ttu-id="42562-106">Тип</span><span class="sxs-lookup"><span data-stu-id="42562-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="42562-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="42562-107">reportRefreshDate</span></span>         | <span data-ttu-id="42562-108">Дата</span><span class="sxs-lookup"><span data-stu-id="42562-108">Date</span></span>              |
| <span data-ttu-id="42562-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="42562-109">userPrincipalName</span></span>         | <span data-ttu-id="42562-110">String</span><span class="sxs-lookup"><span data-stu-id="42562-110">String</span></span>            |
| <span data-ttu-id="42562-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="42562-111">isDeleted</span></span>                 | <span data-ttu-id="42562-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="42562-112">Boolean</span></span>           |
| <span data-ttu-id="42562-113">Делетеддате</span><span class="sxs-lookup"><span data-stu-id="42562-113">deletedDate</span></span>               | <span data-ttu-id="42562-114">Дата</span><span class="sxs-lookup"><span data-stu-id="42562-114">Date</span></span>              |
| <span data-ttu-id="42562-115">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="42562-115">lastActivityDate</span></span>          | <span data-ttu-id="42562-116">Дата</span><span class="sxs-lookup"><span data-stu-id="42562-116">Date</span></span>              |
| <span data-ttu-id="42562-117">Виеведоредитедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="42562-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="42562-118">Int64</span><span class="sxs-lookup"><span data-stu-id="42562-118">Int64</span></span>             |
| <span data-ttu-id="42562-119">Синцедфилекаунт</span><span class="sxs-lookup"><span data-stu-id="42562-119">syncedFileCount</span></span>           | <span data-ttu-id="42562-120">Int64</span><span class="sxs-lookup"><span data-stu-id="42562-120">Int64</span></span>             |
| <span data-ttu-id="42562-121">Шарединтерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="42562-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="42562-122">Int64</span><span class="sxs-lookup"><span data-stu-id="42562-122">Int64</span></span>             |
| <span data-ttu-id="42562-123">Шаредекстерналлифилекаунт</span><span class="sxs-lookup"><span data-stu-id="42562-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="42562-124">Int64</span><span class="sxs-lookup"><span data-stu-id="42562-124">Int64</span></span>             |
| <span data-ttu-id="42562-125">Ассигнедпродуктс</span><span class="sxs-lookup"><span data-stu-id="42562-125">assignedProducts</span></span>          | <span data-ttu-id="42562-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="42562-126">String collection</span></span> |
| <span data-ttu-id="42562-127">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="42562-127">reportPeriod</span></span>              | <span data-ttu-id="42562-128">String</span><span class="sxs-lookup"><span data-stu-id="42562-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="42562-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42562-129">JSON representation</span></span>

<span data-ttu-id="42562-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42562-130">The following is a JSON representation of the resource.</span></span>

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
