---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1de8618d20151d079e3f2fdcbadf3658db2b73ef
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788424"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="2c757-103">Тип ресурса Оператингсистемверсионранже</span><span class="sxs-lookup"><span data-stu-id="2c757-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="2c757-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c757-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c757-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c757-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c757-106">Диапазон версий операционной системы.</span><span class="sxs-lookup"><span data-stu-id="2c757-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="2c757-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c757-107">Properties</span></span>
|<span data-ttu-id="2c757-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c757-108">Property</span></span>|<span data-ttu-id="2c757-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2c757-109">Type</span></span>|<span data-ttu-id="2c757-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2c757-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c757-111">description</span><span class="sxs-lookup"><span data-stu-id="2c757-111">description</span></span>|<span data-ttu-id="2c757-112">String</span><span class="sxs-lookup"><span data-stu-id="2c757-112">String</span></span>|<span data-ttu-id="2c757-113">Описание этого диапазона (например, "допустимые сборки 1702")</span><span class="sxs-lookup"><span data-stu-id="2c757-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="2c757-114">ловестверсион</span><span class="sxs-lookup"><span data-stu-id="2c757-114">lowestVersion</span></span>|<span data-ttu-id="2c757-115">String</span><span class="sxs-lookup"><span data-stu-id="2c757-115">String</span></span>|<span data-ttu-id="2c757-116">Наименьшая включающая версия, содержащаяся в этом диапазоне.</span><span class="sxs-lookup"><span data-stu-id="2c757-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="2c757-117">хигхестверсион</span><span class="sxs-lookup"><span data-stu-id="2c757-117">highestVersion</span></span>|<span data-ttu-id="2c757-118">String</span><span class="sxs-lookup"><span data-stu-id="2c757-118">String</span></span>|<span data-ttu-id="2c757-119">Максимальная включающая версия, которую содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="2c757-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c757-120">Связи</span><span class="sxs-lookup"><span data-stu-id="2c757-120">Relationships</span></span>
<span data-ttu-id="2c757-121">Нет</span><span class="sxs-lookup"><span data-stu-id="2c757-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c757-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c757-122">JSON Representation</span></span>
<span data-ttu-id="2c757-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c757-123">Here is a JSON representation of the resource.</span></span>
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



