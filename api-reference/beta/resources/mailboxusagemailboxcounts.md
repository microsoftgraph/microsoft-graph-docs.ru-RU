---
title: Тип ресурса Маилбоксусажемаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b9f336e3d23cd84f79af7092463383a030336e13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009862"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="e61bf-103">Тип ресурса Маилбоксусажемаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="e61bf-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e61bf-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e61bf-104">Properties</span></span>

| <span data-ttu-id="e61bf-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e61bf-105">Property</span></span>          | <span data-ttu-id="e61bf-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e61bf-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e61bf-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="e61bf-107">reportRefreshDate</span></span> | <span data-ttu-id="e61bf-108">Дата</span><span class="sxs-lookup"><span data-stu-id="e61bf-108">Date</span></span>   |
| <span data-ttu-id="e61bf-109">total</span><span class="sxs-lookup"><span data-stu-id="e61bf-109">total</span></span>             | <span data-ttu-id="e61bf-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e61bf-110">Int64</span></span>  |
| <span data-ttu-id="e61bf-111">ASP</span><span class="sxs-lookup"><span data-stu-id="e61bf-111">active</span></span>            | <span data-ttu-id="e61bf-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e61bf-112">Int64</span></span>  |
| <span data-ttu-id="e61bf-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="e61bf-113">reportDate</span></span>        | <span data-ttu-id="e61bf-114">Дата</span><span class="sxs-lookup"><span data-stu-id="e61bf-114">Date</span></span>   |
| <span data-ttu-id="e61bf-115">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="e61bf-115">reportPeriod</span></span>      | <span data-ttu-id="e61bf-116">String</span><span class="sxs-lookup"><span data-stu-id="e61bf-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e61bf-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e61bf-117">JSON representation</span></span>

<span data-ttu-id="e61bf-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e61bf-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
