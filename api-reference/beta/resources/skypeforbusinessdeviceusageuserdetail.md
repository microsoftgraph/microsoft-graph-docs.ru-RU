---
title: Тип ресурса Скипефорбусинессдевицеусажеусердетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555936"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="62652-103">Тип ресурса Скипефорбусинессдевицеусажеусердетаил</span><span class="sxs-lookup"><span data-stu-id="62652-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="62652-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="62652-104">Properties</span></span>

| <span data-ttu-id="62652-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="62652-105">Property</span></span>          | <span data-ttu-id="62652-106">Тип</span><span class="sxs-lookup"><span data-stu-id="62652-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="62652-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="62652-107">reportRefreshDate</span></span> | <span data-ttu-id="62652-108">Дата</span><span class="sxs-lookup"><span data-stu-id="62652-108">Date</span></span>    |
| <span data-ttu-id="62652-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="62652-109">userPrincipalName</span></span> | <span data-ttu-id="62652-110">String</span><span class="sxs-lookup"><span data-stu-id="62652-110">String</span></span>  |
| <span data-ttu-id="62652-111">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="62652-111">lastActivityDate</span></span>  | <span data-ttu-id="62652-112">Дата</span><span class="sxs-lookup"><span data-stu-id="62652-112">Date</span></span>    |
| <span data-ttu-id="62652-113">Уседвиндовс</span><span class="sxs-lookup"><span data-stu-id="62652-113">usedWindows</span></span>       | <span data-ttu-id="62652-114">Логический</span><span class="sxs-lookup"><span data-stu-id="62652-114">Boolean</span></span> |
| <span data-ttu-id="62652-115">Уседвиндовсфоне</span><span class="sxs-lookup"><span data-stu-id="62652-115">usedWindowsPhone</span></span>  | <span data-ttu-id="62652-116">Логический</span><span class="sxs-lookup"><span data-stu-id="62652-116">Boolean</span></span> |
| <span data-ttu-id="62652-117">Уседандроидфоне</span><span class="sxs-lookup"><span data-stu-id="62652-117">usedAndroidPhone</span></span>  | <span data-ttu-id="62652-118">Логический</span><span class="sxs-lookup"><span data-stu-id="62652-118">Boolean</span></span> |
| <span data-ttu-id="62652-119">Уседифоне</span><span class="sxs-lookup"><span data-stu-id="62652-119">usediPhone</span></span>        | <span data-ttu-id="62652-120">Логический</span><span class="sxs-lookup"><span data-stu-id="62652-120">Boolean</span></span> |
| <span data-ttu-id="62652-121">Уседипад</span><span class="sxs-lookup"><span data-stu-id="62652-121">usediPad</span></span>          | <span data-ttu-id="62652-122">Логический</span><span class="sxs-lookup"><span data-stu-id="62652-122">Boolean</span></span> |
| <span data-ttu-id="62652-123">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="62652-123">reportPeriod</span></span>      | <span data-ttu-id="62652-124">String</span><span class="sxs-lookup"><span data-stu-id="62652-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="62652-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="62652-125">JSON representation</span></span>

<span data-ttu-id="62652-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62652-126">The following is a JSON representation of the resource.</span></span>

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
