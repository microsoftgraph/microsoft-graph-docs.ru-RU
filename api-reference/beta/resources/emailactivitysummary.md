---
title: Тип ресурса Емаилактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 84958874af09b31aafed694c1a62d080a5c798ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506673"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="fde63-103">Тип ресурса Емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="fde63-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fde63-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="fde63-104">Properties</span></span>

| <span data-ttu-id="fde63-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="fde63-105">Property</span></span>          | <span data-ttu-id="fde63-106">Тип</span><span class="sxs-lookup"><span data-stu-id="fde63-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fde63-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="fde63-107">reportRefreshDate</span></span> | <span data-ttu-id="fde63-108">Дата</span><span class="sxs-lookup"><span data-stu-id="fde63-108">Date</span></span>   |
| <span data-ttu-id="fde63-109">Отправить</span><span class="sxs-lookup"><span data-stu-id="fde63-109">send</span></span>              | <span data-ttu-id="fde63-110">Int64</span><span class="sxs-lookup"><span data-stu-id="fde63-110">Int64</span></span>  |
| <span data-ttu-id="fde63-111">получил</span><span class="sxs-lookup"><span data-stu-id="fde63-111">receive</span></span>           | <span data-ttu-id="fde63-112">Int64</span><span class="sxs-lookup"><span data-stu-id="fde63-112">Int64</span></span>  |
| <span data-ttu-id="fde63-113">прочитан</span><span class="sxs-lookup"><span data-stu-id="fde63-113">read</span></span>              | <span data-ttu-id="fde63-114">Int64</span><span class="sxs-lookup"><span data-stu-id="fde63-114">Int64</span></span>  |
| <span data-ttu-id="fde63-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="fde63-115">reportDate</span></span>        | <span data-ttu-id="fde63-116">Дата</span><span class="sxs-lookup"><span data-stu-id="fde63-116">Date</span></span>   |
| <span data-ttu-id="fde63-117">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="fde63-117">reportPeriod</span></span>      | <span data-ttu-id="fde63-118">String</span><span class="sxs-lookup"><span data-stu-id="fde63-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fde63-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fde63-119">JSON representation</span></span>

<span data-ttu-id="fde63-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fde63-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
