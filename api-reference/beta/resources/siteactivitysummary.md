---
title: Тип ресурса Ситеактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 0e24da683b2abe319a60e5a51144a96f9ec00135
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520550"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="0283a-103">Тип ресурса Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="0283a-103">siteActivitySummary resource type</span></span>

<span data-ttu-id="0283a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0283a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0283a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0283a-105">Properties</span></span>

| <span data-ttu-id="0283a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0283a-106">Property</span></span>          | <span data-ttu-id="0283a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0283a-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="0283a-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="0283a-108">reportRefreshDate</span></span> | <span data-ttu-id="0283a-109">Дата</span><span class="sxs-lookup"><span data-stu-id="0283a-109">Date</span></span>   |
| <span data-ttu-id="0283a-110">виеведоредитед</span><span class="sxs-lookup"><span data-stu-id="0283a-110">viewedOrEdited</span></span>    | <span data-ttu-id="0283a-111">Int64</span><span class="sxs-lookup"><span data-stu-id="0283a-111">Int64</span></span>  |
| <span data-ttu-id="0283a-112">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="0283a-112">synced</span></span>            | <span data-ttu-id="0283a-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0283a-113">Int64</span></span>  |
| <span data-ttu-id="0283a-114">шарединтерналли</span><span class="sxs-lookup"><span data-stu-id="0283a-114">sharedInternally</span></span>  | <span data-ttu-id="0283a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="0283a-115">Int64</span></span>  |
| <span data-ttu-id="0283a-116">шаредекстерналли</span><span class="sxs-lookup"><span data-stu-id="0283a-116">sharedExternally</span></span>  | <span data-ttu-id="0283a-117">Int64</span><span class="sxs-lookup"><span data-stu-id="0283a-117">Int64</span></span>  |
| <span data-ttu-id="0283a-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="0283a-118">reportDate</span></span>        | <span data-ttu-id="0283a-119">Дата</span><span class="sxs-lookup"><span data-stu-id="0283a-119">Date</span></span>   |
| <span data-ttu-id="0283a-120">репортпериод</span><span class="sxs-lookup"><span data-stu-id="0283a-120">reportPeriod</span></span>      | <span data-ttu-id="0283a-121">String</span><span class="sxs-lookup"><span data-stu-id="0283a-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0283a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0283a-122">JSON representation</span></span>

<span data-ttu-id="0283a-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0283a-123">The following is a JSON representation of the resource.</span></span>

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
