---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20a52b813de13b51fcf94a93fa440337e7123f02
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525959"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="67930-103">Тип ресурса Оператингсистемверсионранже</span><span class="sxs-lookup"><span data-stu-id="67930-103">operatingSystemVersionRange resource type</span></span>

<span data-ttu-id="67930-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="67930-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67930-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67930-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67930-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67930-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67930-107">Диапазон версий операционной системы.</span><span class="sxs-lookup"><span data-stu-id="67930-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="67930-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="67930-108">Properties</span></span>
|<span data-ttu-id="67930-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="67930-109">Property</span></span>|<span data-ttu-id="67930-110">Тип</span><span class="sxs-lookup"><span data-stu-id="67930-110">Type</span></span>|<span data-ttu-id="67930-111">Описание</span><span class="sxs-lookup"><span data-stu-id="67930-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67930-112">description</span><span class="sxs-lookup"><span data-stu-id="67930-112">description</span></span>|<span data-ttu-id="67930-113">String</span><span class="sxs-lookup"><span data-stu-id="67930-113">String</span></span>|<span data-ttu-id="67930-114">Описание этого диапазона (например, "допустимые сборки 1702")</span><span class="sxs-lookup"><span data-stu-id="67930-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="67930-115">ловестверсион</span><span class="sxs-lookup"><span data-stu-id="67930-115">lowestVersion</span></span>|<span data-ttu-id="67930-116">String</span><span class="sxs-lookup"><span data-stu-id="67930-116">String</span></span>|<span data-ttu-id="67930-117">Наименьшая включающая версия, содержащаяся в этом диапазоне.</span><span class="sxs-lookup"><span data-stu-id="67930-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="67930-118">хигхестверсион</span><span class="sxs-lookup"><span data-stu-id="67930-118">highestVersion</span></span>|<span data-ttu-id="67930-119">String</span><span class="sxs-lookup"><span data-stu-id="67930-119">String</span></span>|<span data-ttu-id="67930-120">Максимальная включающая версия, которую содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="67930-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67930-121">Связи</span><span class="sxs-lookup"><span data-stu-id="67930-121">Relationships</span></span>
<span data-ttu-id="67930-122">Нет</span><span class="sxs-lookup"><span data-stu-id="67930-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67930-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67930-123">JSON Representation</span></span>
<span data-ttu-id="67930-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67930-124">Here is a JSON representation of the resource.</span></span>
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



