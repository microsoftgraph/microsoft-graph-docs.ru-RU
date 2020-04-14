---
title: Тип ресурса Маилбоксусажемаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 32a2aba9aab207cede8118baed4435708995192a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473434"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="e5361-103">Тип ресурса Маилбоксусажемаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="e5361-103">mailboxUsageMailboxCounts resource type</span></span>

<span data-ttu-id="e5361-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5361-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e5361-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5361-105">Properties</span></span>

| <span data-ttu-id="e5361-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5361-106">Property</span></span>          | <span data-ttu-id="e5361-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e5361-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e5361-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="e5361-108">reportRefreshDate</span></span> | <span data-ttu-id="e5361-109">Дата</span><span class="sxs-lookup"><span data-stu-id="e5361-109">Date</span></span>   |
| <span data-ttu-id="e5361-110">total</span><span class="sxs-lookup"><span data-stu-id="e5361-110">total</span></span>             | <span data-ttu-id="e5361-111">Int64</span><span class="sxs-lookup"><span data-stu-id="e5361-111">Int64</span></span>  |
| <span data-ttu-id="e5361-112">ASP</span><span class="sxs-lookup"><span data-stu-id="e5361-112">active</span></span>            | <span data-ttu-id="e5361-113">Int64</span><span class="sxs-lookup"><span data-stu-id="e5361-113">Int64</span></span>  |
| <span data-ttu-id="e5361-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="e5361-114">reportDate</span></span>        | <span data-ttu-id="e5361-115">Дата</span><span class="sxs-lookup"><span data-stu-id="e5361-115">Date</span></span>   |
| <span data-ttu-id="e5361-116">репортпериод</span><span class="sxs-lookup"><span data-stu-id="e5361-116">reportPeriod</span></span>      | <span data-ttu-id="e5361-117">String</span><span class="sxs-lookup"><span data-stu-id="e5361-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e5361-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5361-118">JSON representation</span></span>

<span data-ttu-id="e5361-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5361-119">The following is a JSON representation of the resource.</span></span>

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
