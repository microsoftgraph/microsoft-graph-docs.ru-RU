---
title: Тип ресурса operatingSystemVersionRange
description: Диапазон версии операционной системы.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aaac008b013a8bf2cfd1a88d1fab06a523abb949
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398529"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="ded2e-103">Тип ресурса operatingSystemVersionRange</span><span class="sxs-lookup"><span data-stu-id="ded2e-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="ded2e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ded2e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ded2e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ded2e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ded2e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ded2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ded2e-107">Диапазон версии операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ded2e-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="ded2e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ded2e-108">Properties</span></span>
|<span data-ttu-id="ded2e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ded2e-109">Property</span></span>|<span data-ttu-id="ded2e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ded2e-110">Type</span></span>|<span data-ttu-id="ded2e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ded2e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ded2e-112">description</span><span class="sxs-lookup"><span data-stu-id="ded2e-112">description</span></span>|<span data-ttu-id="ded2e-113">String</span><span class="sxs-lookup"><span data-stu-id="ded2e-113">String</span></span>|<span data-ttu-id="ded2e-114">Описание этого диапазона (например действительно 1702 сборок)</span><span class="sxs-lookup"><span data-stu-id="ded2e-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="ded2e-115">lowestVersion</span><span class="sxs-lookup"><span data-stu-id="ded2e-115">lowestVersion</span></span>|<span data-ttu-id="ded2e-116">String</span><span class="sxs-lookup"><span data-stu-id="ded2e-116">String</span></span>|<span data-ttu-id="ded2e-117">Низший включительно версия, которая содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="ded2e-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="ded2e-118">highestVersion</span><span class="sxs-lookup"><span data-stu-id="ded2e-118">highestVersion</span></span>|<span data-ttu-id="ded2e-119">String</span><span class="sxs-lookup"><span data-stu-id="ded2e-119">String</span></span>|<span data-ttu-id="ded2e-120">Наибольший включительно версию, которая содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="ded2e-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ded2e-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="ded2e-121">Relationships</span></span>
<span data-ttu-id="ded2e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ded2e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ded2e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ded2e-123">JSON Representation</span></span>
<span data-ttu-id="ded2e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ded2e-124">Here is a JSON representation of the resource.</span></span>
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




