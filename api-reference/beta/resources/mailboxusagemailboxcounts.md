---
title: Тип ресурса Маилбоксусажемаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e9da6a72c3c2d79323041e683702a7af2e4699c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463273"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="4085b-103">Тип ресурса Маилбоксусажемаилбокскаунтс</span><span class="sxs-lookup"><span data-stu-id="4085b-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4085b-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4085b-104">Properties</span></span>

| <span data-ttu-id="4085b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4085b-105">Property</span></span>          | <span data-ttu-id="4085b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4085b-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4085b-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="4085b-107">reportRefreshDate</span></span> | <span data-ttu-id="4085b-108">Дата</span><span class="sxs-lookup"><span data-stu-id="4085b-108">Date</span></span>   |
| <span data-ttu-id="4085b-109">total</span><span class="sxs-lookup"><span data-stu-id="4085b-109">total</span></span>             | <span data-ttu-id="4085b-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4085b-110">Int64</span></span>  |
| <span data-ttu-id="4085b-111">ASP</span><span class="sxs-lookup"><span data-stu-id="4085b-111">active</span></span>            | <span data-ttu-id="4085b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4085b-112">Int64</span></span>  |
| <span data-ttu-id="4085b-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="4085b-113">reportDate</span></span>        | <span data-ttu-id="4085b-114">Дата</span><span class="sxs-lookup"><span data-stu-id="4085b-114">Date</span></span>   |
| <span data-ttu-id="4085b-115">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="4085b-115">reportPeriod</span></span>      | <span data-ttu-id="4085b-116">String</span><span class="sxs-lookup"><span data-stu-id="4085b-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4085b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4085b-117">JSON representation</span></span>

<span data-ttu-id="4085b-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4085b-118">The following is a JSON representation of the resource.</span></span>

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
