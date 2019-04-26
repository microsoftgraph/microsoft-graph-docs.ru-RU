---
title: Тип ресурса Скипефорбусинессактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: e59bd33b1709780bac9726ee716ef9d81ef33c1f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568161"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a><span data-ttu-id="426ad-103">Тип ресурса Скипефорбусинессактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="426ad-103">skypeForBusinessActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="426ad-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="426ad-104">Properties</span></span>

| <span data-ttu-id="426ad-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="426ad-105">Property</span></span>          | <span data-ttu-id="426ad-106">Тип</span><span class="sxs-lookup"><span data-stu-id="426ad-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="426ad-107">Пиртопир</span><span class="sxs-lookup"><span data-stu-id="426ad-107">peerToPeer</span></span>        | <span data-ttu-id="426ad-108">Int64</span><span class="sxs-lookup"><span data-stu-id="426ad-108">Int64</span></span>  |
| <span data-ttu-id="426ad-109">распределяют</span><span class="sxs-lookup"><span data-stu-id="426ad-109">organized</span></span>         | <span data-ttu-id="426ad-110">Int64</span><span class="sxs-lookup"><span data-stu-id="426ad-110">Int64</span></span>  |
| <span data-ttu-id="426ad-111">участвовал</span><span class="sxs-lookup"><span data-stu-id="426ad-111">participated</span></span>      | <span data-ttu-id="426ad-112">Int64</span><span class="sxs-lookup"><span data-stu-id="426ad-112">Int64</span></span>  |
| <span data-ttu-id="426ad-113">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="426ad-113">reportRefreshDate</span></span> | <span data-ttu-id="426ad-114">Дата</span><span class="sxs-lookup"><span data-stu-id="426ad-114">Date</span></span>   |
| <span data-ttu-id="426ad-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="426ad-115">reportDate</span></span>        | <span data-ttu-id="426ad-116">Дата</span><span class="sxs-lookup"><span data-stu-id="426ad-116">Date</span></span>   |
| <span data-ttu-id="426ad-117">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="426ad-117">reportPeriod</span></span>      | <span data-ttu-id="426ad-118">String</span><span class="sxs-lookup"><span data-stu-id="426ad-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="426ad-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="426ad-119">JSON representation</span></span>

<span data-ttu-id="426ad-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="426ad-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
