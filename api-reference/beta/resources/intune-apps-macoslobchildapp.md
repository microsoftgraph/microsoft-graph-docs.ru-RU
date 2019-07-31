---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ca4d371966781378c9097769d9178de69d8f7d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012592"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="1a7db-103">Тип ресурса Макослобчилдапп</span><span class="sxs-lookup"><span data-stu-id="1a7db-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="1a7db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a7db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a7db-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a7db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a7db-106">Содержит свойства бизнес-приложения MacOS в пакете набора</span><span class="sxs-lookup"><span data-stu-id="1a7db-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="1a7db-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a7db-107">Properties</span></span>
|<span data-ttu-id="1a7db-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a7db-108">Property</span></span>|<span data-ttu-id="1a7db-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1a7db-109">Type</span></span>|<span data-ttu-id="1a7db-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1a7db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a7db-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="1a7db-111">bundleId</span></span>|<span data-ttu-id="1a7db-112">String</span><span class="sxs-lookup"><span data-stu-id="1a7db-112">String</span></span>|<span data-ttu-id="1a7db-113">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="1a7db-113">The Identity Name.</span></span>|
|<span data-ttu-id="1a7db-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="1a7db-114">buildNumber</span></span>|<span data-ttu-id="1a7db-115">String</span><span class="sxs-lookup"><span data-stu-id="1a7db-115">String</span></span>|<span data-ttu-id="1a7db-116">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="1a7db-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1a7db-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="1a7db-117">versionNumber</span></span>|<span data-ttu-id="1a7db-118">String</span><span class="sxs-lookup"><span data-stu-id="1a7db-118">String</span></span>|<span data-ttu-id="1a7db-119">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="1a7db-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a7db-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="1a7db-120">Relationships</span></span>
<span data-ttu-id="1a7db-121">Нет</span><span class="sxs-lookup"><span data-stu-id="1a7db-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a7db-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a7db-122">JSON Representation</span></span>
<span data-ttu-id="1a7db-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a7db-123">Here is a JSON representation of the resource.</span></span>
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





