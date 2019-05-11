---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c4ee0802b6e6029d6c49672736e77a89f5346a0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950286"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="f0eae-103">Тип ресурса Макослобчилдапп</span><span class="sxs-lookup"><span data-stu-id="f0eae-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="f0eae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0eae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0eae-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0eae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0eae-106">Содержит свойства бизнес-приложения MacOS в пакете набора</span><span class="sxs-lookup"><span data-stu-id="f0eae-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="f0eae-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0eae-107">Properties</span></span>
|<span data-ttu-id="f0eae-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0eae-108">Property</span></span>|<span data-ttu-id="f0eae-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f0eae-109">Type</span></span>|<span data-ttu-id="f0eae-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f0eae-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0eae-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="f0eae-111">bundleId</span></span>|<span data-ttu-id="f0eae-112">String</span><span class="sxs-lookup"><span data-stu-id="f0eae-112">String</span></span>|<span data-ttu-id="f0eae-113">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f0eae-113">The Identity Name.</span></span>|
|<span data-ttu-id="f0eae-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="f0eae-114">buildNumber</span></span>|<span data-ttu-id="f0eae-115">String</span><span class="sxs-lookup"><span data-stu-id="f0eae-115">String</span></span>|<span data-ttu-id="f0eae-116">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="f0eae-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f0eae-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="f0eae-117">versionNumber</span></span>|<span data-ttu-id="f0eae-118">Строка</span><span class="sxs-lookup"><span data-stu-id="f0eae-118">String</span></span>|<span data-ttu-id="f0eae-119">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="f0eae-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0eae-120">Связи</span><span class="sxs-lookup"><span data-stu-id="f0eae-120">Relationships</span></span>
<span data-ttu-id="f0eae-121">Нет</span><span class="sxs-lookup"><span data-stu-id="f0eae-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0eae-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0eae-122">JSON Representation</span></span>
<span data-ttu-id="f0eae-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0eae-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```




