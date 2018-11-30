---
title: Тип ресурса emailActivitySummary
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 039592a33cd004b9a5dc7800c0dbd4ece91bd48c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080218"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="76dde-103">Тип ресурса emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="76dde-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="76dde-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="76dde-104">Properties</span></span>

| <span data-ttu-id="76dde-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="76dde-105">Property</span></span>          | <span data-ttu-id="76dde-106">Тип</span><span class="sxs-lookup"><span data-stu-id="76dde-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="76dde-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="76dde-107">reportRefreshDate</span></span> | <span data-ttu-id="76dde-108">Date</span><span class="sxs-lookup"><span data-stu-id="76dde-108">Date</span></span>   |
| <span data-ttu-id="76dde-109">отправить</span><span class="sxs-lookup"><span data-stu-id="76dde-109">send</span></span>              | <span data-ttu-id="76dde-110">Int64</span><span class="sxs-lookup"><span data-stu-id="76dde-110">Int64</span></span>  |
| <span data-ttu-id="76dde-111">Получение</span><span class="sxs-lookup"><span data-stu-id="76dde-111">receive</span></span>           | <span data-ttu-id="76dde-112">Int64</span><span class="sxs-lookup"><span data-stu-id="76dde-112">Int64</span></span>  |
| <span data-ttu-id="76dde-113">чтение</span><span class="sxs-lookup"><span data-stu-id="76dde-113">read</span></span>              | <span data-ttu-id="76dde-114">Int64</span><span class="sxs-lookup"><span data-stu-id="76dde-114">Int64</span></span>  |
| <span data-ttu-id="76dde-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="76dde-115">reportDate</span></span>        | <span data-ttu-id="76dde-116">Date</span><span class="sxs-lookup"><span data-stu-id="76dde-116">Date</span></span>   |
| <span data-ttu-id="76dde-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="76dde-117">reportPeriod</span></span>      | <span data-ttu-id="76dde-118">String</span><span class="sxs-lookup"><span data-stu-id="76dde-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76dde-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76dde-119">JSON representation</span></span>

<span data-ttu-id="76dde-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76dde-120">The following is a JSON representation of the resource.</span></span>

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
