---
title: Тип ресурса Скипефорбусинессдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 582c3483d4292f634385461508bf579834dfd12e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520410"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="f5540-103">Тип ресурса Скипефорбусинессдевицеусажеусердетаил</span><span class="sxs-lookup"><span data-stu-id="f5540-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="f5540-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5540-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f5540-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5540-105">Properties</span></span>

| <span data-ttu-id="f5540-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5540-106">Property</span></span>          | <span data-ttu-id="f5540-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f5540-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="f5540-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="f5540-108">reportRefreshDate</span></span> | <span data-ttu-id="f5540-109">Дата</span><span class="sxs-lookup"><span data-stu-id="f5540-109">Date</span></span>    |
| <span data-ttu-id="f5540-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f5540-110">userPrincipalName</span></span> | <span data-ttu-id="f5540-111">String</span><span class="sxs-lookup"><span data-stu-id="f5540-111">String</span></span>  |
| <span data-ttu-id="f5540-112">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="f5540-112">lastActivityDate</span></span>  | <span data-ttu-id="f5540-113">Дата</span><span class="sxs-lookup"><span data-stu-id="f5540-113">Date</span></span>    |
| <span data-ttu-id="f5540-114">уседвиндовс</span><span class="sxs-lookup"><span data-stu-id="f5540-114">usedWindows</span></span>       | <span data-ttu-id="f5540-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5540-115">Boolean</span></span> |
| <span data-ttu-id="f5540-116">уседвиндовсфоне</span><span class="sxs-lookup"><span data-stu-id="f5540-116">usedWindowsPhone</span></span>  | <span data-ttu-id="f5540-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5540-117">Boolean</span></span> |
| <span data-ttu-id="f5540-118">уседандроидфоне</span><span class="sxs-lookup"><span data-stu-id="f5540-118">usedAndroidPhone</span></span>  | <span data-ttu-id="f5540-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5540-119">Boolean</span></span> |
| <span data-ttu-id="f5540-120">уседифоне</span><span class="sxs-lookup"><span data-stu-id="f5540-120">usediPhone</span></span>        | <span data-ttu-id="f5540-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5540-121">Boolean</span></span> |
| <span data-ttu-id="f5540-122">уседипад</span><span class="sxs-lookup"><span data-stu-id="f5540-122">usediPad</span></span>          | <span data-ttu-id="f5540-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5540-123">Boolean</span></span> |
| <span data-ttu-id="f5540-124">репортпериод</span><span class="sxs-lookup"><span data-stu-id="f5540-124">reportPeriod</span></span>      | <span data-ttu-id="f5540-125">String</span><span class="sxs-lookup"><span data-stu-id="f5540-125">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f5540-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5540-126">JSON representation</span></span>

<span data-ttu-id="f5540-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5540-127">The following is a JSON representation of the resource.</span></span>

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
