---
title: Тип ресурса Оператингсистемверсионранже
description: Диапазон версий операционной системы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9019150efed2f52f884746d7c62f1d7e5a35e83
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293957"
---
# <a name="operatingsystemversionrange-resource-type"></a><span data-ttu-id="63884-103">Тип ресурса Оператингсистемверсионранже</span><span class="sxs-lookup"><span data-stu-id="63884-103">operatingSystemVersionRange resource type</span></span>

<span data-ttu-id="63884-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63884-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63884-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63884-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63884-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63884-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63884-107">Диапазон версий операционной системы.</span><span class="sxs-lookup"><span data-stu-id="63884-107">Operating System version range.</span></span>

## <a name="properties"></a><span data-ttu-id="63884-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="63884-108">Properties</span></span>
|<span data-ttu-id="63884-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="63884-109">Property</span></span>|<span data-ttu-id="63884-110">Тип</span><span class="sxs-lookup"><span data-stu-id="63884-110">Type</span></span>|<span data-ttu-id="63884-111">Описание</span><span class="sxs-lookup"><span data-stu-id="63884-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63884-112">description</span><span class="sxs-lookup"><span data-stu-id="63884-112">description</span></span>|<span data-ttu-id="63884-113">String</span><span class="sxs-lookup"><span data-stu-id="63884-113">String</span></span>|<span data-ttu-id="63884-114">Описание этого диапазона (например, "допустимые сборки 1702")</span><span class="sxs-lookup"><span data-stu-id="63884-114">The description of this range (e.g. Valid 1702 builds)</span></span>|
|<span data-ttu-id="63884-115">ловестверсион</span><span class="sxs-lookup"><span data-stu-id="63884-115">lowestVersion</span></span>|<span data-ttu-id="63884-116">String</span><span class="sxs-lookup"><span data-stu-id="63884-116">String</span></span>|<span data-ttu-id="63884-117">Наименьшая включающая версия, содержащаяся в этом диапазоне.</span><span class="sxs-lookup"><span data-stu-id="63884-117">The lowest inclusive version that this range contains.</span></span>|
|<span data-ttu-id="63884-118">хигхестверсион</span><span class="sxs-lookup"><span data-stu-id="63884-118">highestVersion</span></span>|<span data-ttu-id="63884-119">String</span><span class="sxs-lookup"><span data-stu-id="63884-119">String</span></span>|<span data-ttu-id="63884-120">Максимальная включающая версия, которую содержит этот диапазон.</span><span class="sxs-lookup"><span data-stu-id="63884-120">The highest inclusive version that this range contains.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63884-121">Связи</span><span class="sxs-lookup"><span data-stu-id="63884-121">Relationships</span></span>
<span data-ttu-id="63884-122">Нет</span><span class="sxs-lookup"><span data-stu-id="63884-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63884-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63884-123">JSON Representation</span></span>
<span data-ttu-id="63884-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63884-124">Here is a JSON representation of the resource.</span></span>
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




