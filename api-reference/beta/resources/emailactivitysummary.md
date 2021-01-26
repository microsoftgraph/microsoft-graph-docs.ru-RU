---
title: Тип ресурса emailActivitySummary
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9b3bb1d05c57874497d536de332f85b462335b5d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981874"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="d8181-103">Тип ресурса emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="d8181-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="d8181-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8181-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d8181-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8181-105">Properties</span></span>

| <span data-ttu-id="d8181-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8181-106">Property</span></span>          | <span data-ttu-id="d8181-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d8181-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d8181-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d8181-108">reportRefreshDate</span></span> | <span data-ttu-id="d8181-109">Дата</span><span class="sxs-lookup"><span data-stu-id="d8181-109">Date</span></span>   |
| <span data-ttu-id="d8181-110">Отправить</span><span class="sxs-lookup"><span data-stu-id="d8181-110">send</span></span>              | <span data-ttu-id="d8181-111">Int64</span><span class="sxs-lookup"><span data-stu-id="d8181-111">Int64</span></span>  |
| <span data-ttu-id="d8181-112">receive</span><span class="sxs-lookup"><span data-stu-id="d8181-112">receive</span></span>           | <span data-ttu-id="d8181-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d8181-113">Int64</span></span>  |
| <span data-ttu-id="d8181-114">read</span><span class="sxs-lookup"><span data-stu-id="d8181-114">read</span></span>              | <span data-ttu-id="d8181-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d8181-115">Int64</span></span>  |
| <span data-ttu-id="d8181-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="d8181-116">reportDate</span></span>        | <span data-ttu-id="d8181-117">Дата</span><span class="sxs-lookup"><span data-stu-id="d8181-117">Date</span></span>   |
| <span data-ttu-id="d8181-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d8181-118">reportPeriod</span></span>      | <span data-ttu-id="d8181-119">String</span><span class="sxs-lookup"><span data-stu-id="d8181-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8181-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8181-120">JSON representation</span></span>

<span data-ttu-id="d8181-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8181-121">The following is a JSON representation of the resource.</span></span>

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


