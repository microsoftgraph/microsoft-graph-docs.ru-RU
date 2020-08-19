---
title: Тип ресурса Скипефорбусинессдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 50f37fdfd3441c256241b76ebcc6b144eb1486d7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811055"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="327e7-103">Тип ресурса Скипефорбусинессдевицеусажеусердетаил</span><span class="sxs-lookup"><span data-stu-id="327e7-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="327e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="327e7-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="327e7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="327e7-105">Properties</span></span>

| <span data-ttu-id="327e7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="327e7-106">Property</span></span>          | <span data-ttu-id="327e7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="327e7-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="327e7-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="327e7-108">reportRefreshDate</span></span> | <span data-ttu-id="327e7-109">Дата</span><span class="sxs-lookup"><span data-stu-id="327e7-109">Date</span></span>    |
| <span data-ttu-id="327e7-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="327e7-110">userPrincipalName</span></span> | <span data-ttu-id="327e7-111">String</span><span class="sxs-lookup"><span data-stu-id="327e7-111">String</span></span>  |
| <span data-ttu-id="327e7-112">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="327e7-112">lastActivityDate</span></span>  | <span data-ttu-id="327e7-113">Дата</span><span class="sxs-lookup"><span data-stu-id="327e7-113">Date</span></span>    |
| <span data-ttu-id="327e7-114">уседвиндовс</span><span class="sxs-lookup"><span data-stu-id="327e7-114">usedWindows</span></span>       | <span data-ttu-id="327e7-115">Логический</span><span class="sxs-lookup"><span data-stu-id="327e7-115">Boolean</span></span> |
| <span data-ttu-id="327e7-116">уседвиндовсфоне</span><span class="sxs-lookup"><span data-stu-id="327e7-116">usedWindowsPhone</span></span>  | <span data-ttu-id="327e7-117">Логический</span><span class="sxs-lookup"><span data-stu-id="327e7-117">Boolean</span></span> |
| <span data-ttu-id="327e7-118">уседандроидфоне</span><span class="sxs-lookup"><span data-stu-id="327e7-118">usedAndroidPhone</span></span>  | <span data-ttu-id="327e7-119">Логический</span><span class="sxs-lookup"><span data-stu-id="327e7-119">Boolean</span></span> |
| <span data-ttu-id="327e7-120">уседифоне</span><span class="sxs-lookup"><span data-stu-id="327e7-120">usediPhone</span></span>        | <span data-ttu-id="327e7-121">Логический</span><span class="sxs-lookup"><span data-stu-id="327e7-121">Boolean</span></span> |
| <span data-ttu-id="327e7-122">уседипад</span><span class="sxs-lookup"><span data-stu-id="327e7-122">usediPad</span></span>          | <span data-ttu-id="327e7-123">Логический</span><span class="sxs-lookup"><span data-stu-id="327e7-123">Boolean</span></span> |
| <span data-ttu-id="327e7-124">репортпериод</span><span class="sxs-lookup"><span data-stu-id="327e7-124">reportPeriod</span></span>      | <span data-ttu-id="327e7-125">String</span><span class="sxs-lookup"><span data-stu-id="327e7-125">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="327e7-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="327e7-126">JSON representation</span></span>

<span data-ttu-id="327e7-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="327e7-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "lastActivityDate": "Date",
  "usedWindows": true,
  "usedWindowsPhone": true,
  "usedAndroidPhone": true,
  "usediPhone": true,
  "usediPad": true,
  "reportPeriod": "String"
}
```
