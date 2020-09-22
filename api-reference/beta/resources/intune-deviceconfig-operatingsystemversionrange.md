---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4ce1fffd5170ea55b524c7a8828efc9ce71fc64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989243"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="d2bc7-103">Тип ресурса Оператингсистемверсионранже</span><span class="sxs-lookup"><span data-stu-id="d2bc7-103">operatingSystemVersionRange resource type</span></span>

<span data-ttu-id="d2bc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2bc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2bc7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2bc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2bc7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2bc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2bc7-107">Диапазон версий операционной системы.</span><span class="sxs-lookup"><span data-stu-id="d2bc7-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="d2bc7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2bc7-108">Properties</span></span>
|<span data-ttu-id="d2bc7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2bc7-109">Property</span></span>|<span data-ttu-id="d2bc7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d2bc7-110">Type</span></span>|<span data-ttu-id="d2bc7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d2bc7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2bc7-112">description</span><span class="sxs-lookup"><span data-stu-id="d2bc7-112">description</span></span>|<span data-ttu-id="d2bc7-113">String</span><span class="sxs-lookup"><span data-stu-id="d2bc7-113">String</span></span>|<span data-ttu-id="d2bc7-114">Описание этого диапазона (например, "допустимые сборки 1702")</span><span class="sxs-lookup"><span data-stu-id="d2bc7-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="d2bc7-115">ловестверсион</span><span class="sxs-lookup"><span data-stu-id="d2bc7-115">lowestVersion</span></span>|<span data-ttu-id="d2bc7-116">String</span><span class="sxs-lookup"><span data-stu-id="d2bc7-116">String</span></span>|<span data-ttu-id="d2bc7-117">Наименьшая включающая версия, содержащаяся в этом диапазоне.</span><span class="sxs-lookup"><span data-stu-id="d2bc7-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="d2bc7-118">хигхестверсион</span><span class="sxs-lookup"><span data-stu-id="d2bc7-118">highestVersion</span></span>|<span data-ttu-id="d2bc7-119">String</span><span class="sxs-lookup"><span data-stu-id="d2bc7-119">String</span></span>|<span data-ttu-id="d2bc7-120">Максимальная включающая версия, которую содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="d2bc7-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2bc7-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d2bc7-121">Relationships</span></span>
<span data-ttu-id="d2bc7-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d2bc7-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2bc7-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2bc7-123">JSON Representation</span></span>
<span data-ttu-id="d2bc7-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2bc7-124">Here is a JSON representation of the resource.</span></span>
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






