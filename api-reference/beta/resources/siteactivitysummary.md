---
title: Тип ресурса Ситеактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a49b8e47ca2a6efcc5c5c87702fdea0122b208e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583601"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="bc2ca-103">Тип ресурса Ситеактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="bc2ca-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bc2ca-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc2ca-104">Properties</span></span>

| <span data-ttu-id="bc2ca-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc2ca-105">Property</span></span>          | <span data-ttu-id="bc2ca-106">Тип</span><span class="sxs-lookup"><span data-stu-id="bc2ca-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="bc2ca-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="bc2ca-107">reportRefreshDate</span></span> | <span data-ttu-id="bc2ca-108">Дата</span><span class="sxs-lookup"><span data-stu-id="bc2ca-108">Date</span></span>   |
| <span data-ttu-id="bc2ca-109">Виеведоредитед</span><span class="sxs-lookup"><span data-stu-id="bc2ca-109">viewedOrEdited</span></span>    | <span data-ttu-id="bc2ca-110">Int64</span><span class="sxs-lookup"><span data-stu-id="bc2ca-110">Int64</span></span>  |
| <span data-ttu-id="bc2ca-111">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="bc2ca-111">synced</span></span>            | <span data-ttu-id="bc2ca-112">Int64</span><span class="sxs-lookup"><span data-stu-id="bc2ca-112">Int64</span></span>  |
| <span data-ttu-id="bc2ca-113">Шарединтерналли</span><span class="sxs-lookup"><span data-stu-id="bc2ca-113">sharedInternally</span></span>  | <span data-ttu-id="bc2ca-114">Int64</span><span class="sxs-lookup"><span data-stu-id="bc2ca-114">Int64</span></span>  |
| <span data-ttu-id="bc2ca-115">Шаредекстерналли</span><span class="sxs-lookup"><span data-stu-id="bc2ca-115">sharedExternally</span></span>  | <span data-ttu-id="bc2ca-116">Int64</span><span class="sxs-lookup"><span data-stu-id="bc2ca-116">Int64</span></span>  |
| <span data-ttu-id="bc2ca-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="bc2ca-117">reportDate</span></span>        | <span data-ttu-id="bc2ca-118">Дата</span><span class="sxs-lookup"><span data-stu-id="bc2ca-118">Date</span></span>   |
| <span data-ttu-id="bc2ca-119">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="bc2ca-119">reportPeriod</span></span>      | <span data-ttu-id="bc2ca-120">String</span><span class="sxs-lookup"><span data-stu-id="bc2ca-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bc2ca-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc2ca-121">JSON representation</span></span>

<span data-ttu-id="bc2ca-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc2ca-122">The following is a JSON representation of the resource.</span></span>

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
