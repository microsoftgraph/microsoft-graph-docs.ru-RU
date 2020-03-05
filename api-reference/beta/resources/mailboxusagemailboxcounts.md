---
title: Тип ресурса Маилбоксусажемаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 41bb58fa74deb9f8296a8f109d83b7cdeb73012e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522850"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="530d3-103">Тип ресурса Маилбоксусажемаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="530d3-103">mailboxUsageMailboxCounts resource type</span></span>

<span data-ttu-id="530d3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="530d3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="530d3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="530d3-105">Properties</span></span>

| <span data-ttu-id="530d3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="530d3-106">Property</span></span>          | <span data-ttu-id="530d3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="530d3-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="530d3-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="530d3-108">reportRefreshDate</span></span> | <span data-ttu-id="530d3-109">Дата</span><span class="sxs-lookup"><span data-stu-id="530d3-109">Date</span></span>   |
| <span data-ttu-id="530d3-110">total</span><span class="sxs-lookup"><span data-stu-id="530d3-110">total</span></span>             | <span data-ttu-id="530d3-111">Int64</span><span class="sxs-lookup"><span data-stu-id="530d3-111">Int64</span></span>  |
| <span data-ttu-id="530d3-112">ASP</span><span class="sxs-lookup"><span data-stu-id="530d3-112">active</span></span>            | <span data-ttu-id="530d3-113">Int64</span><span class="sxs-lookup"><span data-stu-id="530d3-113">Int64</span></span>  |
| <span data-ttu-id="530d3-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="530d3-114">reportDate</span></span>        | <span data-ttu-id="530d3-115">Дата</span><span class="sxs-lookup"><span data-stu-id="530d3-115">Date</span></span>   |
| <span data-ttu-id="530d3-116">репортпериод</span><span class="sxs-lookup"><span data-stu-id="530d3-116">reportPeriod</span></span>      | <span data-ttu-id="530d3-117">String</span><span class="sxs-lookup"><span data-stu-id="530d3-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="530d3-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="530d3-118">JSON representation</span></span>

<span data-ttu-id="530d3-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="530d3-119">The following is a JSON representation of the resource.</span></span>

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
