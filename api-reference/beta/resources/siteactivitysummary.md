---
title: Тип ресурса Ситеактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 1258530aea56f7ec26a2f48274935afc809f2fd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965021"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="be3f7-103">Тип ресурса Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="be3f7-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="be3f7-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="be3f7-104">Properties</span></span>

| <span data-ttu-id="be3f7-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="be3f7-105">Property</span></span>          | <span data-ttu-id="be3f7-106">Тип</span><span class="sxs-lookup"><span data-stu-id="be3f7-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="be3f7-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="be3f7-107">reportRefreshDate</span></span> | <span data-ttu-id="be3f7-108">Дата</span><span class="sxs-lookup"><span data-stu-id="be3f7-108">Date</span></span>   |
| <span data-ttu-id="be3f7-109">Виеведоредитед</span><span class="sxs-lookup"><span data-stu-id="be3f7-109">viewedOrEdited</span></span>    | <span data-ttu-id="be3f7-110">Int64</span><span class="sxs-lookup"><span data-stu-id="be3f7-110">Int64</span></span>  |
| <span data-ttu-id="be3f7-111">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="be3f7-111">synced</span></span>            | <span data-ttu-id="be3f7-112">Int64</span><span class="sxs-lookup"><span data-stu-id="be3f7-112">Int64</span></span>  |
| <span data-ttu-id="be3f7-113">Шарединтерналли</span><span class="sxs-lookup"><span data-stu-id="be3f7-113">sharedInternally</span></span>  | <span data-ttu-id="be3f7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="be3f7-114">Int64</span></span>  |
| <span data-ttu-id="be3f7-115">Шаредекстерналли</span><span class="sxs-lookup"><span data-stu-id="be3f7-115">sharedExternally</span></span>  | <span data-ttu-id="be3f7-116">Int64</span><span class="sxs-lookup"><span data-stu-id="be3f7-116">Int64</span></span>  |
| <span data-ttu-id="be3f7-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="be3f7-117">reportDate</span></span>        | <span data-ttu-id="be3f7-118">Дата</span><span class="sxs-lookup"><span data-stu-id="be3f7-118">Date</span></span>   |
| <span data-ttu-id="be3f7-119">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="be3f7-119">reportPeriod</span></span>      | <span data-ttu-id="be3f7-120">String</span><span class="sxs-lookup"><span data-stu-id="be3f7-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="be3f7-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be3f7-121">JSON representation</span></span>

<span data-ttu-id="be3f7-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be3f7-122">The following is a JSON representation of the resource.</span></span>

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
