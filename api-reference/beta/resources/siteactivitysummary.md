---
title: Тип ресурса Ситеактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: f629d8b60179e83515af1e9fa5d86e55e7681f17
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807908"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="f1e7d-103">Тип ресурса Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="f1e7d-103">siteActivitySummary resource type</span></span>

<span data-ttu-id="f1e7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1e7d-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f1e7d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1e7d-105">Properties</span></span>

| <span data-ttu-id="f1e7d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1e7d-106">Property</span></span>          | <span data-ttu-id="f1e7d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f1e7d-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f1e7d-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="f1e7d-108">reportRefreshDate</span></span> | <span data-ttu-id="f1e7d-109">Дата</span><span class="sxs-lookup"><span data-stu-id="f1e7d-109">Date</span></span>   |
| <span data-ttu-id="f1e7d-110">виеведоредитед</span><span class="sxs-lookup"><span data-stu-id="f1e7d-110">viewedOrEdited</span></span>    | <span data-ttu-id="f1e7d-111">Int64</span><span class="sxs-lookup"><span data-stu-id="f1e7d-111">Int64</span></span>  |
| <span data-ttu-id="f1e7d-112">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="f1e7d-112">synced</span></span>            | <span data-ttu-id="f1e7d-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f1e7d-113">Int64</span></span>  |
| <span data-ttu-id="f1e7d-114">шарединтерналли</span><span class="sxs-lookup"><span data-stu-id="f1e7d-114">sharedInternally</span></span>  | <span data-ttu-id="f1e7d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f1e7d-115">Int64</span></span>  |
| <span data-ttu-id="f1e7d-116">шаредекстерналли</span><span class="sxs-lookup"><span data-stu-id="f1e7d-116">sharedExternally</span></span>  | <span data-ttu-id="f1e7d-117">Int64</span><span class="sxs-lookup"><span data-stu-id="f1e7d-117">Int64</span></span>  |
| <span data-ttu-id="f1e7d-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="f1e7d-118">reportDate</span></span>        | <span data-ttu-id="f1e7d-119">Дата</span><span class="sxs-lookup"><span data-stu-id="f1e7d-119">Date</span></span>   |
| <span data-ttu-id="f1e7d-120">репортпериод</span><span class="sxs-lookup"><span data-stu-id="f1e7d-120">reportPeriod</span></span>      | <span data-ttu-id="f1e7d-121">String</span><span class="sxs-lookup"><span data-stu-id="f1e7d-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1e7d-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f1e7d-122">JSON representation</span></span>

<span data-ttu-id="f1e7d-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1e7d-123">The following is a JSON representation of the resource.</span></span>

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
