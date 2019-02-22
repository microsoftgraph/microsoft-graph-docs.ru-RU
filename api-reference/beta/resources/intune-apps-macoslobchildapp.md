---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4bf8a8715bb681d1737a2fb1b39e5bac61fb9d7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147000"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="11276-103">Тип ресурса Макослобчилдапп</span><span class="sxs-lookup"><span data-stu-id="11276-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="11276-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11276-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11276-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11276-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11276-106">Содержит свойства бизнес-приложения MacOS в пакете набора</span><span class="sxs-lookup"><span data-stu-id="11276-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="11276-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="11276-107">Properties</span></span>
|<span data-ttu-id="11276-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="11276-108">Property</span></span>|<span data-ttu-id="11276-109">Тип</span><span class="sxs-lookup"><span data-stu-id="11276-109">Type</span></span>|<span data-ttu-id="11276-110">Описание</span><span class="sxs-lookup"><span data-stu-id="11276-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11276-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="11276-111">bundleId</span></span>|<span data-ttu-id="11276-112">String</span><span class="sxs-lookup"><span data-stu-id="11276-112">String</span></span>|<span data-ttu-id="11276-113">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="11276-113">The Identity Name.</span></span>|
|<span data-ttu-id="11276-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="11276-114">buildNumber</span></span>|<span data-ttu-id="11276-115">String</span><span class="sxs-lookup"><span data-stu-id="11276-115">String</span></span>|<span data-ttu-id="11276-116">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="11276-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="11276-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="11276-117">versionNumber</span></span>|<span data-ttu-id="11276-118">String</span><span class="sxs-lookup"><span data-stu-id="11276-118">String</span></span>|<span data-ttu-id="11276-119">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="11276-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11276-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="11276-120">Relationships</span></span>
<span data-ttu-id="11276-121">Нет</span><span class="sxs-lookup"><span data-stu-id="11276-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11276-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11276-122">JSON Representation</span></span>
<span data-ttu-id="11276-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11276-123">Here is a JSON representation of the resource.</span></span>
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




