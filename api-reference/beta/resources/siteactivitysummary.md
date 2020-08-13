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
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="c53c3-103">Тип ресурса Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="c53c3-103">siteActivitySummary resource type</span></span>

<span data-ttu-id="c53c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c53c3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c53c3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c53c3-105">Properties</span></span>

| <span data-ttu-id="c53c3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c53c3-106">Property</span></span>          | <span data-ttu-id="c53c3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c53c3-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c53c3-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="c53c3-108">reportRefreshDate</span></span> | <span data-ttu-id="c53c3-109">Дата</span><span class="sxs-lookup"><span data-stu-id="c53c3-109">Date</span></span>   |
| <span data-ttu-id="c53c3-110">виеведоредитед</span><span class="sxs-lookup"><span data-stu-id="c53c3-110">viewedOrEdited</span></span>    | <span data-ttu-id="c53c3-111">Int64</span><span class="sxs-lookup"><span data-stu-id="c53c3-111">Int64</span></span>  |
| <span data-ttu-id="c53c3-112">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="c53c3-112">synced</span></span>            | <span data-ttu-id="c53c3-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c53c3-113">Int64</span></span>  |
| <span data-ttu-id="c53c3-114">шарединтерналли</span><span class="sxs-lookup"><span data-stu-id="c53c3-114">sharedInternally</span></span>  | <span data-ttu-id="c53c3-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c53c3-115">Int64</span></span>  |
| <span data-ttu-id="c53c3-116">шаредекстерналли</span><span class="sxs-lookup"><span data-stu-id="c53c3-116">sharedExternally</span></span>  | <span data-ttu-id="c53c3-117">Int64</span><span class="sxs-lookup"><span data-stu-id="c53c3-117">Int64</span></span>  |
| <span data-ttu-id="c53c3-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="c53c3-118">reportDate</span></span>        | <span data-ttu-id="c53c3-119">Дата</span><span class="sxs-lookup"><span data-stu-id="c53c3-119">Date</span></span>   |
| <span data-ttu-id="c53c3-120">репортпериод</span><span class="sxs-lookup"><span data-stu-id="c53c3-120">reportPeriod</span></span>      | <span data-ttu-id="c53c3-121">Строка</span><span class="sxs-lookup"><span data-stu-id="c53c3-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c53c3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c53c3-122">JSON representation</span></span>

<span data-ttu-id="c53c3-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c53c3-123">The following is a JSON representation of the resource.</span></span>

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
