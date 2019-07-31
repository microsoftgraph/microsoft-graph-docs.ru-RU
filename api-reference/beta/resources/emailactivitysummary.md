---
title: Тип ресурса Емаилактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 64c9468d79a93b6f82fff0f04206a0fb6e95e4fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972224"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="6252c-103">Тип ресурса Емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="6252c-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6252c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6252c-104">Properties</span></span>

| <span data-ttu-id="6252c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6252c-105">Property</span></span>          | <span data-ttu-id="6252c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6252c-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6252c-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="6252c-107">reportRefreshDate</span></span> | <span data-ttu-id="6252c-108">Дата</span><span class="sxs-lookup"><span data-stu-id="6252c-108">Date</span></span>   |
| <span data-ttu-id="6252c-109">Отправить</span><span class="sxs-lookup"><span data-stu-id="6252c-109">send</span></span>              | <span data-ttu-id="6252c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6252c-110">Int64</span></span>  |
| <span data-ttu-id="6252c-111">получил</span><span class="sxs-lookup"><span data-stu-id="6252c-111">receive</span></span>           | <span data-ttu-id="6252c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6252c-112">Int64</span></span>  |
| <span data-ttu-id="6252c-113">прочитан</span><span class="sxs-lookup"><span data-stu-id="6252c-113">read</span></span>              | <span data-ttu-id="6252c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6252c-114">Int64</span></span>  |
| <span data-ttu-id="6252c-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="6252c-115">reportDate</span></span>        | <span data-ttu-id="6252c-116">Дата</span><span class="sxs-lookup"><span data-stu-id="6252c-116">Date</span></span>   |
| <span data-ttu-id="6252c-117">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="6252c-117">reportPeriod</span></span>      | <span data-ttu-id="6252c-118">String</span><span class="sxs-lookup"><span data-stu-id="6252c-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6252c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6252c-119">JSON representation</span></span>

<span data-ttu-id="6252c-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6252c-120">The following is a JSON representation of the resource.</span></span>

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
