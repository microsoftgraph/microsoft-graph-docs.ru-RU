---
title: Тип ресурса Скипефорбусинессдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b84cf9c7654354446fb7c6a5005befe3d17a0fa4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964916"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="05971-103">Тип ресурса Скипефорбусинессдевицеусажеусердетаил</span><span class="sxs-lookup"><span data-stu-id="05971-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="05971-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="05971-104">Properties</span></span>

| <span data-ttu-id="05971-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="05971-105">Property</span></span>          | <span data-ttu-id="05971-106">Тип</span><span class="sxs-lookup"><span data-stu-id="05971-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="05971-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="05971-107">reportRefreshDate</span></span> | <span data-ttu-id="05971-108">Дата</span><span class="sxs-lookup"><span data-stu-id="05971-108">Date</span></span>    |
| <span data-ttu-id="05971-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="05971-109">userPrincipalName</span></span> | <span data-ttu-id="05971-110">String</span><span class="sxs-lookup"><span data-stu-id="05971-110">String</span></span>  |
| <span data-ttu-id="05971-111">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="05971-111">lastActivityDate</span></span>  | <span data-ttu-id="05971-112">Дата</span><span class="sxs-lookup"><span data-stu-id="05971-112">Date</span></span>    |
| <span data-ttu-id="05971-113">Уседвиндовс</span><span class="sxs-lookup"><span data-stu-id="05971-113">usedWindows</span></span>       | <span data-ttu-id="05971-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="05971-114">Boolean</span></span> |
| <span data-ttu-id="05971-115">Уседвиндовсфоне</span><span class="sxs-lookup"><span data-stu-id="05971-115">usedWindowsPhone</span></span>  | <span data-ttu-id="05971-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="05971-116">Boolean</span></span> |
| <span data-ttu-id="05971-117">Уседандроидфоне</span><span class="sxs-lookup"><span data-stu-id="05971-117">usedAndroidPhone</span></span>  | <span data-ttu-id="05971-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="05971-118">Boolean</span></span> |
| <span data-ttu-id="05971-119">Уседифоне</span><span class="sxs-lookup"><span data-stu-id="05971-119">usediPhone</span></span>        | <span data-ttu-id="05971-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="05971-120">Boolean</span></span> |
| <span data-ttu-id="05971-121">Уседипад</span><span class="sxs-lookup"><span data-stu-id="05971-121">usediPad</span></span>          | <span data-ttu-id="05971-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="05971-122">Boolean</span></span> |
| <span data-ttu-id="05971-123">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="05971-123">reportPeriod</span></span>      | <span data-ttu-id="05971-124">String</span><span class="sxs-lookup"><span data-stu-id="05971-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="05971-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05971-125">JSON representation</span></span>

<span data-ttu-id="05971-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05971-126">The following is a JSON representation of the resource.</span></span>

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
