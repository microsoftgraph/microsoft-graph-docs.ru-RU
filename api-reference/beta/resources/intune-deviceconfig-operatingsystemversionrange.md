---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4a1658cb75d88da6f0739b175646d5fa1de60b66
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722931"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="e7189-103">Тип ресурса Оператингсистемверсионранже</span><span class="sxs-lookup"><span data-stu-id="e7189-103">operatingSystemVersionRange resource type</span></span>

<span data-ttu-id="e7189-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7189-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7189-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7189-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7189-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7189-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7189-107">Диапазон версий операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e7189-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="e7189-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7189-108">Properties</span></span>
|<span data-ttu-id="e7189-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7189-109">Property</span></span>|<span data-ttu-id="e7189-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e7189-110">Type</span></span>|<span data-ttu-id="e7189-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e7189-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7189-112">description</span><span class="sxs-lookup"><span data-stu-id="e7189-112">description</span></span>|<span data-ttu-id="e7189-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e7189-113">String</span></span>|<span data-ttu-id="e7189-114">Описание этого диапазона (например, "допустимые сборки 1702")</span><span class="sxs-lookup"><span data-stu-id="e7189-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="e7189-115">ловестверсион</span><span class="sxs-lookup"><span data-stu-id="e7189-115">lowestVersion</span></span>|<span data-ttu-id="e7189-116">Строка</span><span class="sxs-lookup"><span data-stu-id="e7189-116">String</span></span>|<span data-ttu-id="e7189-117">Наименьшая включающая версия, содержащаяся в этом диапазоне.</span><span class="sxs-lookup"><span data-stu-id="e7189-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="e7189-118">хигхестверсион</span><span class="sxs-lookup"><span data-stu-id="e7189-118">highestVersion</span></span>|<span data-ttu-id="e7189-119">Строка</span><span class="sxs-lookup"><span data-stu-id="e7189-119">String</span></span>|<span data-ttu-id="e7189-120">Максимальная включающая версия, которую содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="e7189-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7189-121">Связи</span><span class="sxs-lookup"><span data-stu-id="e7189-121">Relationships</span></span>
<span data-ttu-id="e7189-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e7189-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7189-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7189-123">JSON Representation</span></span>
<span data-ttu-id="e7189-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7189-124">Here is a JSON representation of the resource.</span></span>
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





