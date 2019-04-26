---
title: Тип ресурса Яммерактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c220ce211c9c6b61d41aa5773e3bcc01697f4e31
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555117"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="e37db-103">Тип ресурса Яммерактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="e37db-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e37db-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e37db-104">Properties</span></span>

| <span data-ttu-id="e37db-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e37db-105">Property</span></span>          | <span data-ttu-id="e37db-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e37db-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e37db-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="e37db-107">reportRefreshDate</span></span> | <span data-ttu-id="e37db-108">Дата</span><span class="sxs-lookup"><span data-stu-id="e37db-108">Date</span></span>   |
| <span data-ttu-id="e37db-109">метк</span><span class="sxs-lookup"><span data-stu-id="e37db-109">liked</span></span>             | <span data-ttu-id="e37db-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e37db-110">Int64</span></span>  |
| <span data-ttu-id="e37db-111">размещен</span><span class="sxs-lookup"><span data-stu-id="e37db-111">posted</span></span>            | <span data-ttu-id="e37db-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e37db-112">Int64</span></span>  |
| <span data-ttu-id="e37db-113">прочитан</span><span class="sxs-lookup"><span data-stu-id="e37db-113">read</span></span>              | <span data-ttu-id="e37db-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e37db-114">Int64</span></span>  |
| <span data-ttu-id="e37db-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="e37db-115">reportDate</span></span>        | <span data-ttu-id="e37db-116">Дата</span><span class="sxs-lookup"><span data-stu-id="e37db-116">Date</span></span>   |
| <span data-ttu-id="e37db-117">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="e37db-117">reportPeriod</span></span>      | <span data-ttu-id="e37db-118">String</span><span class="sxs-lookup"><span data-stu-id="e37db-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e37db-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e37db-119">JSON representation</span></span>

<span data-ttu-id="e37db-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e37db-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
