---
title: Тип ресурса Маилбоксусажемаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e8282422f9724cbffff8f3e9573f0a7cb0a94920
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971820"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="64b73-103">Тип ресурса Маилбоксусажемаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="64b73-103">mailboxUsageMailboxCounts resource type</span></span>

<span data-ttu-id="64b73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64b73-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="64b73-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="64b73-105">Properties</span></span>

| <span data-ttu-id="64b73-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="64b73-106">Property</span></span>          | <span data-ttu-id="64b73-107">Тип</span><span class="sxs-lookup"><span data-stu-id="64b73-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="64b73-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="64b73-108">reportRefreshDate</span></span> | <span data-ttu-id="64b73-109">Дата</span><span class="sxs-lookup"><span data-stu-id="64b73-109">Date</span></span>   |
| <span data-ttu-id="64b73-110">total</span><span class="sxs-lookup"><span data-stu-id="64b73-110">total</span></span>             | <span data-ttu-id="64b73-111">Int64</span><span class="sxs-lookup"><span data-stu-id="64b73-111">Int64</span></span>  |
| <span data-ttu-id="64b73-112">ASP</span><span class="sxs-lookup"><span data-stu-id="64b73-112">active</span></span>            | <span data-ttu-id="64b73-113">Int64</span><span class="sxs-lookup"><span data-stu-id="64b73-113">Int64</span></span>  |
| <span data-ttu-id="64b73-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="64b73-114">reportDate</span></span>        | <span data-ttu-id="64b73-115">Дата</span><span class="sxs-lookup"><span data-stu-id="64b73-115">Date</span></span>   |
| <span data-ttu-id="64b73-116">репортпериод</span><span class="sxs-lookup"><span data-stu-id="64b73-116">reportPeriod</span></span>      | <span data-ttu-id="64b73-117">String</span><span class="sxs-lookup"><span data-stu-id="64b73-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64b73-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64b73-118">JSON representation</span></span>

<span data-ttu-id="64b73-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64b73-119">The following is a JSON representation of the resource.</span></span>

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


