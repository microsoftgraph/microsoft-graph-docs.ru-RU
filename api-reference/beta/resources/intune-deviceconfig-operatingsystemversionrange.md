---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d94d120fcedd6ef086002895f7364f78f5ef3579
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969914"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="618b1-103">Тип ресурса Оператингсистемверсионранже</span><span class="sxs-lookup"><span data-stu-id="618b1-103">operatingSystemVersionRange resource type</span></span>

> <span data-ttu-id="618b1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="618b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="618b1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="618b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="618b1-106">Диапазон версий операционной системы.</span><span class="sxs-lookup"><span data-stu-id="618b1-106">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="618b1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="618b1-107">Properties</span></span>
|<span data-ttu-id="618b1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="618b1-108">Property</span></span>|<span data-ttu-id="618b1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="618b1-109">Type</span></span>|<span data-ttu-id="618b1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="618b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="618b1-111">description</span><span class="sxs-lookup"><span data-stu-id="618b1-111">description</span></span>|<span data-ttu-id="618b1-112">String</span><span class="sxs-lookup"><span data-stu-id="618b1-112">String</span></span>|<span data-ttu-id="618b1-113">Описание этого диапазона (например, "допустимые сборки 1702")</span><span class="sxs-lookup"><span data-stu-id="618b1-113">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="618b1-114">Ловестверсион</span><span class="sxs-lookup"><span data-stu-id="618b1-114">lowestVersion</span></span>|<span data-ttu-id="618b1-115">String</span><span class="sxs-lookup"><span data-stu-id="618b1-115">String</span></span>|<span data-ttu-id="618b1-116">Наименьшая включающая версия, содержащаяся в этом диапазоне.</span><span class="sxs-lookup"><span data-stu-id="618b1-116">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="618b1-117">Хигхестверсион</span><span class="sxs-lookup"><span data-stu-id="618b1-117">highestVersion</span></span>|<span data-ttu-id="618b1-118">String</span><span class="sxs-lookup"><span data-stu-id="618b1-118">String</span></span>|<span data-ttu-id="618b1-119">Максимальная включающая версия, которую содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="618b1-119">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="618b1-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="618b1-120">Relationships</span></span>
<span data-ttu-id="618b1-121">Нет</span><span class="sxs-lookup"><span data-stu-id="618b1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="618b1-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="618b1-122">JSON Representation</span></span>
<span data-ttu-id="618b1-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="618b1-123">Here is a JSON representation of the resource.</span></span>
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





