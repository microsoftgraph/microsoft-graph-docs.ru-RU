---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a74d40582806fb4f574cb80beaff2db0abac0caa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798044"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="76641-103">Тип ресурса Макослобчилдапп</span><span class="sxs-lookup"><span data-stu-id="76641-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="76641-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76641-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76641-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76641-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76641-106">Содержит свойства бизнес-приложения MacOS в пакете набора</span><span class="sxs-lookup"><span data-stu-id="76641-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="76641-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="76641-107">Properties</span></span>
|<span data-ttu-id="76641-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="76641-108">Property</span></span>|<span data-ttu-id="76641-109">Тип</span><span class="sxs-lookup"><span data-stu-id="76641-109">Type</span></span>|<span data-ttu-id="76641-110">Описание</span><span class="sxs-lookup"><span data-stu-id="76641-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76641-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="76641-111">bundleId</span></span>|<span data-ttu-id="76641-112">String</span><span class="sxs-lookup"><span data-stu-id="76641-112">String</span></span>|<span data-ttu-id="76641-113">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="76641-113">The Identity Name.</span></span>|
|<span data-ttu-id="76641-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="76641-114">buildNumber</span></span>|<span data-ttu-id="76641-115">String</span><span class="sxs-lookup"><span data-stu-id="76641-115">String</span></span>|<span data-ttu-id="76641-116">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="76641-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="76641-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="76641-117">versionNumber</span></span>|<span data-ttu-id="76641-118">String</span><span class="sxs-lookup"><span data-stu-id="76641-118">String</span></span>|<span data-ttu-id="76641-119">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="76641-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76641-120">Связи</span><span class="sxs-lookup"><span data-stu-id="76641-120">Relationships</span></span>
<span data-ttu-id="76641-121">Нет</span><span class="sxs-lookup"><span data-stu-id="76641-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76641-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76641-122">JSON Representation</span></span>
<span data-ttu-id="76641-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76641-123">Here is a JSON representation of the resource.</span></span>
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



