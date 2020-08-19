---
title: Тип ресурса Онедривеусажеаккаунткаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 8ab079eb15fd2dfe2d66a07d5734b6aa9430055e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812115"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="c7420-103">Тип ресурса Онедривеусажеаккаунткаунтс</span><span class="sxs-lookup"><span data-stu-id="c7420-103">oneDriveUsageAccountCounts resource type</span></span>

<span data-ttu-id="c7420-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7420-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c7420-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7420-105">Properties</span></span>

| <span data-ttu-id="c7420-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7420-106">Property</span></span>          | <span data-ttu-id="c7420-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c7420-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c7420-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="c7420-108">reportRefreshDate</span></span> | <span data-ttu-id="c7420-109">Дата</span><span class="sxs-lookup"><span data-stu-id="c7420-109">Date</span></span>   |
| <span data-ttu-id="c7420-110">ситетипе</span><span class="sxs-lookup"><span data-stu-id="c7420-110">siteType</span></span>          | <span data-ttu-id="c7420-111">String</span><span class="sxs-lookup"><span data-stu-id="c7420-111">String</span></span> |
| <span data-ttu-id="c7420-112">total</span><span class="sxs-lookup"><span data-stu-id="c7420-112">total</span></span>             | <span data-ttu-id="c7420-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c7420-113">Int64</span></span>  |
| <span data-ttu-id="c7420-114">ASP</span><span class="sxs-lookup"><span data-stu-id="c7420-114">active</span></span>            | <span data-ttu-id="c7420-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c7420-115">Int64</span></span>  |
| <span data-ttu-id="c7420-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="c7420-116">reportDate</span></span>        | <span data-ttu-id="c7420-117">Дата</span><span class="sxs-lookup"><span data-stu-id="c7420-117">Date</span></span>   |
| <span data-ttu-id="c7420-118">репортпериод</span><span class="sxs-lookup"><span data-stu-id="c7420-118">reportPeriod</span></span>      | <span data-ttu-id="c7420-119">String</span><span class="sxs-lookup"><span data-stu-id="c7420-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7420-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c7420-120">JSON representation</span></span>

<span data-ttu-id="c7420-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7420-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteType": "String",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
