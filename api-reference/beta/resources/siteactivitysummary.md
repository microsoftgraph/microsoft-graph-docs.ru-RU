---
title: Тип ресурса Ситеактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: ce2d4806dd8c2e8367bf5a9c075fab84e3c17900
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985694"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="17305-103">Тип ресурса Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="17305-103">siteActivitySummary resource type</span></span>

<span data-ttu-id="17305-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17305-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="17305-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="17305-105">Properties</span></span>

| <span data-ttu-id="17305-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="17305-106">Property</span></span>          | <span data-ttu-id="17305-107">Тип</span><span class="sxs-lookup"><span data-stu-id="17305-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="17305-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="17305-108">reportRefreshDate</span></span> | <span data-ttu-id="17305-109">Дата</span><span class="sxs-lookup"><span data-stu-id="17305-109">Date</span></span>   |
| <span data-ttu-id="17305-110">виеведоредитед</span><span class="sxs-lookup"><span data-stu-id="17305-110">viewedOrEdited</span></span>    | <span data-ttu-id="17305-111">Int64</span><span class="sxs-lookup"><span data-stu-id="17305-111">Int64</span></span>  |
| <span data-ttu-id="17305-112">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="17305-112">synced</span></span>            | <span data-ttu-id="17305-113">Int64</span><span class="sxs-lookup"><span data-stu-id="17305-113">Int64</span></span>  |
| <span data-ttu-id="17305-114">шарединтерналли</span><span class="sxs-lookup"><span data-stu-id="17305-114">sharedInternally</span></span>  | <span data-ttu-id="17305-115">Int64</span><span class="sxs-lookup"><span data-stu-id="17305-115">Int64</span></span>  |
| <span data-ttu-id="17305-116">шаредекстерналли</span><span class="sxs-lookup"><span data-stu-id="17305-116">sharedExternally</span></span>  | <span data-ttu-id="17305-117">Int64</span><span class="sxs-lookup"><span data-stu-id="17305-117">Int64</span></span>  |
| <span data-ttu-id="17305-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="17305-118">reportDate</span></span>        | <span data-ttu-id="17305-119">Дата</span><span class="sxs-lookup"><span data-stu-id="17305-119">Date</span></span>   |
| <span data-ttu-id="17305-120">репортпериод</span><span class="sxs-lookup"><span data-stu-id="17305-120">reportPeriod</span></span>      | <span data-ttu-id="17305-121">String</span><span class="sxs-lookup"><span data-stu-id="17305-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="17305-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17305-122">JSON representation</span></span>

<span data-ttu-id="17305-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17305-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date",
  "viewedOrEdited": 1024,
  "synced": 1024,
  "sharedInternally": 1024,
  "sharedExternally": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


