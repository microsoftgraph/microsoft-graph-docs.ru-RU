---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54bd15c4549495ff891d7283c6851e7058ffb887
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780212"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="9834d-103">Тип ресурса Макослобчилдапп</span><span class="sxs-lookup"><span data-stu-id="9834d-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="9834d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9834d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9834d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9834d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9834d-106">Содержит свойства бизнес-приложения MacOS в пакете набора</span><span class="sxs-lookup"><span data-stu-id="9834d-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="9834d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9834d-107">Properties</span></span>
|<span data-ttu-id="9834d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9834d-108">Property</span></span>|<span data-ttu-id="9834d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9834d-109">Type</span></span>|<span data-ttu-id="9834d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9834d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9834d-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="9834d-111">bundleId</span></span>|<span data-ttu-id="9834d-112">String</span><span class="sxs-lookup"><span data-stu-id="9834d-112">String</span></span>|<span data-ttu-id="9834d-113">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9834d-113">The Identity Name.</span></span>|
|<span data-ttu-id="9834d-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9834d-114">buildNumber</span></span>|<span data-ttu-id="9834d-115">String</span><span class="sxs-lookup"><span data-stu-id="9834d-115">String</span></span>|<span data-ttu-id="9834d-116">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="9834d-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9834d-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="9834d-117">versionNumber</span></span>|<span data-ttu-id="9834d-118">String</span><span class="sxs-lookup"><span data-stu-id="9834d-118">String</span></span>|<span data-ttu-id="9834d-119">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="9834d-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9834d-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="9834d-120">Relationships</span></span>
<span data-ttu-id="9834d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="9834d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9834d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9834d-122">JSON Representation</span></span>
<span data-ttu-id="9834d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9834d-123">Here is a JSON representation of the resource.</span></span>
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





