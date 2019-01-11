---
title: Тип ресурса operatingSystemVersionRange
description: Диапазон версии операционной системы.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56df6b53dc29247d3f718ad185152069a071a0f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875805"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="740ae-103">Тип ресурса operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="740ae-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="740ae-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="740ae-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="740ae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="740ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="740ae-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="740ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="740ae-107">Диапазон версии операционной системы.</span><span class="sxs-lookup"><span data-stu-id="740ae-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="740ae-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="740ae-108">Properties</span></span>
|<span data-ttu-id="740ae-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="740ae-109">Property</span></span>|<span data-ttu-id="740ae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="740ae-110">Type</span></span>|<span data-ttu-id="740ae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="740ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="740ae-112">описание</span><span class="sxs-lookup"><span data-stu-id="740ae-112">description</span></span>|<span data-ttu-id="740ae-113">Строка</span><span class="sxs-lookup"><span data-stu-id="740ae-113">String</span></span>|<span data-ttu-id="740ae-114">Описание этого диапазона (например действительно 1702 сборок)</span><span class="sxs-lookup"><span data-stu-id="740ae-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="740ae-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="740ae-115">lowestVersion</span></span>|<span data-ttu-id="740ae-116">Строка</span><span class="sxs-lookup"><span data-stu-id="740ae-116">String</span></span>|<span data-ttu-id="740ae-117">Низший включительно версия, которая содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="740ae-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="740ae-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="740ae-118">highestVersion</span></span>|<span data-ttu-id="740ae-119">Строка</span><span class="sxs-lookup"><span data-stu-id="740ae-119">String</span></span>|<span data-ttu-id="740ae-120">Наибольший включительно версию, которая содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="740ae-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="740ae-121">Связи</span><span class="sxs-lookup"><span data-stu-id="740ae-121">Relationships</span></span>
<span data-ttu-id="740ae-122">Нет</span><span class="sxs-lookup"><span data-stu-id="740ae-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="740ae-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="740ae-123">JSON Representation</span></span>
<span data-ttu-id="740ae-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="740ae-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





