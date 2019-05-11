---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7fe455bc0e934e08b858a084009ac5c8364a673
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950965"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="2c971-103">Тип ресурса Оператингсистемверсионранже</span><span class="sxs-lookup"><span data-stu-id="2c971-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="2c971-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c971-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c971-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c971-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c971-106">Диапазон версий операционной системы.</span><span class="sxs-lookup"><span data-stu-id="2c971-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="2c971-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c971-107">Properties</span></span>
|<span data-ttu-id="2c971-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c971-108">Property</span></span>|<span data-ttu-id="2c971-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2c971-109">Type</span></span>|<span data-ttu-id="2c971-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2c971-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c971-111">description</span><span class="sxs-lookup"><span data-stu-id="2c971-111">description</span></span>|<span data-ttu-id="2c971-112">String</span><span class="sxs-lookup"><span data-stu-id="2c971-112">String</span></span>|<span data-ttu-id="2c971-113">Описание этого диапазона (например, "допустимые сборки 1702")</span><span class="sxs-lookup"><span data-stu-id="2c971-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="2c971-114">Ловестверсион</span><span class="sxs-lookup"><span data-stu-id="2c971-114">lowestVersion</span></span>|<span data-ttu-id="2c971-115">Строка</span><span class="sxs-lookup"><span data-stu-id="2c971-115">String</span></span>|<span data-ttu-id="2c971-116">Наименьшая включающая версия, содержащаяся в этом диапазоне.</span><span class="sxs-lookup"><span data-stu-id="2c971-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="2c971-117">Хигхестверсион</span><span class="sxs-lookup"><span data-stu-id="2c971-117">highestVersion</span></span>|<span data-ttu-id="2c971-118">Строка</span><span class="sxs-lookup"><span data-stu-id="2c971-118">String</span></span>|<span data-ttu-id="2c971-119">Максимальная включающая версия, которую содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="2c971-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c971-120">Связи</span><span class="sxs-lookup"><span data-stu-id="2c971-120">Relationships</span></span>
<span data-ttu-id="2c971-121">Нет</span><span class="sxs-lookup"><span data-stu-id="2c971-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c971-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c971-122">JSON Representation</span></span>
<span data-ttu-id="2c971-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c971-123">Here is a JSON representation of the resource.</span></span>
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




