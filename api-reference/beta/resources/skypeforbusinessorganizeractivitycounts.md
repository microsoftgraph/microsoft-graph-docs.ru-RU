---
title: Тип ресурса Скипефорбусинессорганизерактивитикаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 9f6c77e86f76ac2e34fb87cf8ca5b6bded35a2a2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461161"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a><span data-ttu-id="52073-103">Тип ресурса Скипефорбусинессорганизерактивитикаунтс</span><span class="sxs-lookup"><span data-stu-id="52073-103">skypeForBusinessOrganizerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="52073-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="52073-104">Properties</span></span>

| <span data-ttu-id="52073-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="52073-105">Property</span></span>           | <span data-ttu-id="52073-106">Тип</span><span class="sxs-lookup"><span data-stu-id="52073-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="52073-107">im</span><span class="sxs-lookup"><span data-stu-id="52073-107">im</span></span>                 | <span data-ttu-id="52073-108">Int64</span><span class="sxs-lookup"><span data-stu-id="52073-108">Int64</span></span>  |
| <span data-ttu-id="52073-109">Audiovideohttp</span><span class="sxs-lookup"><span data-stu-id="52073-109">audioVideo</span></span>         | <span data-ttu-id="52073-110">Int64</span><span class="sxs-lookup"><span data-stu-id="52073-110">Int64</span></span>  |
| <span data-ttu-id="52073-111">Аппшаринг</span><span class="sxs-lookup"><span data-stu-id="52073-111">appSharing</span></span>         | <span data-ttu-id="52073-112">Int64</span><span class="sxs-lookup"><span data-stu-id="52073-112">Int64</span></span>  |
| <span data-ttu-id="52073-113">web</span><span class="sxs-lookup"><span data-stu-id="52073-113">web</span></span>                | <span data-ttu-id="52073-114">Int64</span><span class="sxs-lookup"><span data-stu-id="52073-114">Int64</span></span>  |
| <span data-ttu-id="52073-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="52073-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="52073-116">Int64</span><span class="sxs-lookup"><span data-stu-id="52073-116">Int64</span></span>  |
| <span data-ttu-id="52073-117">Диалинаутмикрософт</span><span class="sxs-lookup"><span data-stu-id="52073-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="52073-118">Int64</span><span class="sxs-lookup"><span data-stu-id="52073-118">Int64</span></span>  |
| <span data-ttu-id="52073-119">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="52073-119">reportRefreshDate</span></span>  | <span data-ttu-id="52073-120">Дата</span><span class="sxs-lookup"><span data-stu-id="52073-120">Date</span></span>   |
| <span data-ttu-id="52073-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="52073-121">reportDate</span></span>         | <span data-ttu-id="52073-122">Дата</span><span class="sxs-lookup"><span data-stu-id="52073-122">Date</span></span>   |
| <span data-ttu-id="52073-123">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="52073-123">reportPeriod</span></span>       | <span data-ttu-id="52073-124">String</span><span class="sxs-lookup"><span data-stu-id="52073-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52073-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52073-125">JSON representation</span></span>

<span data-ttu-id="52073-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52073-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
