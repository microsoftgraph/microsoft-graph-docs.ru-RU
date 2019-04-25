---
title: Тип ресурса Скипефорбусинесспиртопирактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 4baf218ed9398a8f208c4d1d44a28579773dea6f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523457"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="5593a-103">Тип ресурса Скипефорбусинесспиртопирактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="5593a-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5593a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="5593a-104">Properties</span></span>

| <span data-ttu-id="5593a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="5593a-105">Property</span></span>          | <span data-ttu-id="5593a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="5593a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5593a-107">im</span><span class="sxs-lookup"><span data-stu-id="5593a-107">im</span></span>                | <span data-ttu-id="5593a-108">Int64</span><span class="sxs-lookup"><span data-stu-id="5593a-108">Int64</span></span>  |
| <span data-ttu-id="5593a-109">audio</span><span class="sxs-lookup"><span data-stu-id="5593a-109">audio</span></span>             | <span data-ttu-id="5593a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5593a-110">Int64</span></span>  |
| <span data-ttu-id="5593a-111">video</span><span class="sxs-lookup"><span data-stu-id="5593a-111">video</span></span>             | <span data-ttu-id="5593a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5593a-112">Int64</span></span>  |
| <span data-ttu-id="5593a-113">Аппшаринг</span><span class="sxs-lookup"><span data-stu-id="5593a-113">appSharing</span></span>        | <span data-ttu-id="5593a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5593a-114">Int64</span></span>  |
| <span data-ttu-id="5593a-115">Филетрансфер</span><span class="sxs-lookup"><span data-stu-id="5593a-115">fileTransfer</span></span>      | <span data-ttu-id="5593a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5593a-116">Int64</span></span>  |
| <span data-ttu-id="5593a-117">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="5593a-117">reportRefreshDate</span></span> | <span data-ttu-id="5593a-118">Дата</span><span class="sxs-lookup"><span data-stu-id="5593a-118">Date</span></span>   |
| <span data-ttu-id="5593a-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="5593a-119">reportDate</span></span>        | <span data-ttu-id="5593a-120">Дата</span><span class="sxs-lookup"><span data-stu-id="5593a-120">Date</span></span>   |
| <span data-ttu-id="5593a-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="5593a-121">reportPeriod</span></span>      | <span data-ttu-id="5593a-122">String</span><span class="sxs-lookup"><span data-stu-id="5593a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5593a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5593a-123">JSON representation</span></span>

<span data-ttu-id="5593a-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5593a-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
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
