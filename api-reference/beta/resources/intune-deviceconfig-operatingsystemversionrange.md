---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80b0afb706a71ef8e0e3d4877fa7d0df822fe1d6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788123"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="6ea93-103">Тип ресурса Оператингсистемверсионранже</span><span class="sxs-lookup"><span data-stu-id="6ea93-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="6ea93-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ea93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ea93-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ea93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ea93-106">Диапазон версий операционной системы.</span><span class="sxs-lookup"><span data-stu-id="6ea93-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="6ea93-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ea93-107">Properties</span></span>
|<span data-ttu-id="6ea93-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ea93-108">Property</span></span>|<span data-ttu-id="6ea93-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6ea93-109">Type</span></span>|<span data-ttu-id="6ea93-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ea93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ea93-111">description</span><span class="sxs-lookup"><span data-stu-id="6ea93-111">description</span></span>|<span data-ttu-id="6ea93-112">String</span><span class="sxs-lookup"><span data-stu-id="6ea93-112">String</span></span>|<span data-ttu-id="6ea93-113">Описание этого диапазона (например, "допустимые сборки 1702")</span><span class="sxs-lookup"><span data-stu-id="6ea93-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="6ea93-114">Ловестверсион</span><span class="sxs-lookup"><span data-stu-id="6ea93-114">lowestVersion</span></span>|<span data-ttu-id="6ea93-115">String</span><span class="sxs-lookup"><span data-stu-id="6ea93-115">String</span></span>|<span data-ttu-id="6ea93-116">Наименьшая включающая версия, содержащаяся в этом диапазоне.</span><span class="sxs-lookup"><span data-stu-id="6ea93-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="6ea93-117">Хигхестверсион</span><span class="sxs-lookup"><span data-stu-id="6ea93-117">highestVersion</span></span>|<span data-ttu-id="6ea93-118">String</span><span class="sxs-lookup"><span data-stu-id="6ea93-118">String</span></span>|<span data-ttu-id="6ea93-119">Максимальная включающая версия, которую содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="6ea93-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ea93-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="6ea93-120">Relationships</span></span>
<span data-ttu-id="6ea93-121">Нет</span><span class="sxs-lookup"><span data-stu-id="6ea93-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ea93-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ea93-122">JSON Representation</span></span>
<span data-ttu-id="6ea93-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ea93-123">Here is a JSON representation of the resource.</span></span>
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





