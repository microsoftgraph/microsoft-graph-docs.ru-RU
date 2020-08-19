---
title: Тип ресурса Скипефорбусинесспиртопирактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 6bdcd96a8c6eb3dff29304bf8dc1dd8956d9063d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811044"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="0f47d-103">Тип ресурса Скипефорбусинесспиртопирактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="0f47d-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

<span data-ttu-id="0f47d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f47d-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0f47d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f47d-105">Properties</span></span>

| <span data-ttu-id="0f47d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f47d-106">Property</span></span>          | <span data-ttu-id="0f47d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0f47d-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="0f47d-108">im</span><span class="sxs-lookup"><span data-stu-id="0f47d-108">im</span></span>                | <span data-ttu-id="0f47d-109">Int64</span><span class="sxs-lookup"><span data-stu-id="0f47d-109">Int64</span></span>  |
| <span data-ttu-id="0f47d-110">audio</span><span class="sxs-lookup"><span data-stu-id="0f47d-110">audio</span></span>             | <span data-ttu-id="0f47d-111">Int64</span><span class="sxs-lookup"><span data-stu-id="0f47d-111">Int64</span></span>  |
| <span data-ttu-id="0f47d-112">video</span><span class="sxs-lookup"><span data-stu-id="0f47d-112">video</span></span>             | <span data-ttu-id="0f47d-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0f47d-113">Int64</span></span>  |
| <span data-ttu-id="0f47d-114">аппшаринг</span><span class="sxs-lookup"><span data-stu-id="0f47d-114">appSharing</span></span>        | <span data-ttu-id="0f47d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="0f47d-115">Int64</span></span>  |
| <span data-ttu-id="0f47d-116">филетрансфер</span><span class="sxs-lookup"><span data-stu-id="0f47d-116">fileTransfer</span></span>      | <span data-ttu-id="0f47d-117">Int64</span><span class="sxs-lookup"><span data-stu-id="0f47d-117">Int64</span></span>  |
| <span data-ttu-id="0f47d-118">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="0f47d-118">reportRefreshDate</span></span> | <span data-ttu-id="0f47d-119">Дата</span><span class="sxs-lookup"><span data-stu-id="0f47d-119">Date</span></span>   |
| <span data-ttu-id="0f47d-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="0f47d-120">reportDate</span></span>        | <span data-ttu-id="0f47d-121">Дата</span><span class="sxs-lookup"><span data-stu-id="0f47d-121">Date</span></span>   |
| <span data-ttu-id="0f47d-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="0f47d-122">reportPeriod</span></span>      | <span data-ttu-id="0f47d-123">String</span><span class="sxs-lookup"><span data-stu-id="0f47d-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0f47d-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0f47d-124">JSON representation</span></span>

<span data-ttu-id="0f47d-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f47d-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```json
{
  "im": 1024,
  "audio": 1024,
  "video": 1024,
  "appSharing": 1024,
  "fileTransfer": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
