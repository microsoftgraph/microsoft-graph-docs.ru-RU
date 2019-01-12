---
title: Тип ресурса operatingSystemVersionRange
description: Диапазон версии операционной системы.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c0b81482ad4b48ad5fe59b1ec0109fcd3bf03f83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918548"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="01a7d-103">Тип ресурса operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="01a7d-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="01a7d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01a7d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01a7d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01a7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01a7d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="01a7d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01a7d-107">Диапазон версии операционной системы.</span><span class="sxs-lookup"><span data-stu-id="01a7d-107">Operating System version range.</span></span>
## <a name="properties"></a><span data-ttu-id="01a7d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="01a7d-108">Properties</span></span>
|<span data-ttu-id="01a7d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="01a7d-109">Property</span></span>|<span data-ttu-id="01a7d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="01a7d-110">Type</span></span>|<span data-ttu-id="01a7d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="01a7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01a7d-112">описание</span><span class="sxs-lookup"><span data-stu-id="01a7d-112">description</span></span>|<span data-ttu-id="01a7d-113">Строка</span><span class="sxs-lookup"><span data-stu-id="01a7d-113">String</span></span>|<span data-ttu-id="01a7d-114">Описание этого диапазона (например действительно 1702 сборок)</span><span class="sxs-lookup"><span data-stu-id="01a7d-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="01a7d-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="01a7d-115">lowestVersion</span></span>|<span data-ttu-id="01a7d-116">Строка</span><span class="sxs-lookup"><span data-stu-id="01a7d-116">String</span></span>|<span data-ttu-id="01a7d-117">Низший включительно версия, которая содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="01a7d-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="01a7d-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="01a7d-118">highestVersion</span></span>|<span data-ttu-id="01a7d-119">Строка</span><span class="sxs-lookup"><span data-stu-id="01a7d-119">String</span></span>|<span data-ttu-id="01a7d-120">Наибольший включительно версию, которая содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="01a7d-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01a7d-121">Связи</span><span class="sxs-lookup"><span data-stu-id="01a7d-121">Relationships</span></span>
<span data-ttu-id="01a7d-122">Нет</span><span class="sxs-lookup"><span data-stu-id="01a7d-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="01a7d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01a7d-123">JSON Representation</span></span>
<span data-ttu-id="01a7d-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01a7d-124">Here is a JSON representation of the resource.</span></span>
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





