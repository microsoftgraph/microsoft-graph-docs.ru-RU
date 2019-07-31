---
title: Тип ресурса Скипефорбусинесспиртопирактивитюсеркаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: baafa0ba3ddf59efdfe049c324b21f1294b155f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964797"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="4b88f-103">Тип ресурса Скипефорбусинесспиртопирактивитюсеркаунтс</span><span class="sxs-lookup"><span data-stu-id="4b88f-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4b88f-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b88f-104">Properties</span></span>

| <span data-ttu-id="4b88f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b88f-105">Property</span></span>          | <span data-ttu-id="4b88f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4b88f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4b88f-107">im</span><span class="sxs-lookup"><span data-stu-id="4b88f-107">im</span></span>                | <span data-ttu-id="4b88f-108">Int64</span><span class="sxs-lookup"><span data-stu-id="4b88f-108">Int64</span></span>  |
| <span data-ttu-id="4b88f-109">audio</span><span class="sxs-lookup"><span data-stu-id="4b88f-109">audio</span></span>             | <span data-ttu-id="4b88f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4b88f-110">Int64</span></span>  |
| <span data-ttu-id="4b88f-111">video</span><span class="sxs-lookup"><span data-stu-id="4b88f-111">video</span></span>             | <span data-ttu-id="4b88f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4b88f-112">Int64</span></span>  |
| <span data-ttu-id="4b88f-113">Аппшаринг</span><span class="sxs-lookup"><span data-stu-id="4b88f-113">appSharing</span></span>        | <span data-ttu-id="4b88f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4b88f-114">Int64</span></span>  |
| <span data-ttu-id="4b88f-115">Филетрансфер</span><span class="sxs-lookup"><span data-stu-id="4b88f-115">fileTransfer</span></span>      | <span data-ttu-id="4b88f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4b88f-116">Int64</span></span>  |
| <span data-ttu-id="4b88f-117">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="4b88f-117">reportRefreshDate</span></span> | <span data-ttu-id="4b88f-118">Дата</span><span class="sxs-lookup"><span data-stu-id="4b88f-118">Date</span></span>   |
| <span data-ttu-id="4b88f-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="4b88f-119">reportDate</span></span>        | <span data-ttu-id="4b88f-120">Дата</span><span class="sxs-lookup"><span data-stu-id="4b88f-120">Date</span></span>   |
| <span data-ttu-id="4b88f-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="4b88f-121">reportPeriod</span></span>      | <span data-ttu-id="4b88f-122">String</span><span class="sxs-lookup"><span data-stu-id="4b88f-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4b88f-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b88f-123">JSON representation</span></span>

<span data-ttu-id="4b88f-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b88f-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
