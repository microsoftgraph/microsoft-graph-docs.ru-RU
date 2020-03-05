---
title: Тип ресурса Емаилактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: dd30bb496cb6591b3bde11d1c0c38b4099175891
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499591"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="831f7-103">Тип ресурса Емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="831f7-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="831f7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="831f7-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="831f7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="831f7-105">Properties</span></span>

| <span data-ttu-id="831f7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="831f7-106">Property</span></span>          | <span data-ttu-id="831f7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="831f7-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="831f7-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="831f7-108">reportRefreshDate</span></span> | <span data-ttu-id="831f7-109">Дата</span><span class="sxs-lookup"><span data-stu-id="831f7-109">Date</span></span>   |
| <span data-ttu-id="831f7-110">Отправить</span><span class="sxs-lookup"><span data-stu-id="831f7-110">send</span></span>              | <span data-ttu-id="831f7-111">Int64</span><span class="sxs-lookup"><span data-stu-id="831f7-111">Int64</span></span>  |
| <span data-ttu-id="831f7-112">получил</span><span class="sxs-lookup"><span data-stu-id="831f7-112">receive</span></span>           | <span data-ttu-id="831f7-113">Int64</span><span class="sxs-lookup"><span data-stu-id="831f7-113">Int64</span></span>  |
| <span data-ttu-id="831f7-114">прочитан</span><span class="sxs-lookup"><span data-stu-id="831f7-114">read</span></span>              | <span data-ttu-id="831f7-115">Int64</span><span class="sxs-lookup"><span data-stu-id="831f7-115">Int64</span></span>  |
| <span data-ttu-id="831f7-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="831f7-116">reportDate</span></span>        | <span data-ttu-id="831f7-117">Дата</span><span class="sxs-lookup"><span data-stu-id="831f7-117">Date</span></span>   |
| <span data-ttu-id="831f7-118">репортпериод</span><span class="sxs-lookup"><span data-stu-id="831f7-118">reportPeriod</span></span>      | <span data-ttu-id="831f7-119">String</span><span class="sxs-lookup"><span data-stu-id="831f7-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="831f7-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="831f7-120">JSON representation</span></span>

<span data-ttu-id="831f7-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="831f7-121">The following is a JSON representation of the resource.</span></span>

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
