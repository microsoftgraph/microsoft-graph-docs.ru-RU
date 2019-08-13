---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b665391a4e7832feea72302db9ffb49c98f69964
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365918"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="4d42d-103">Тип ресурса Макослобчилдапп</span><span class="sxs-lookup"><span data-stu-id="4d42d-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="4d42d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d42d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d42d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d42d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d42d-106">Содержит свойства бизнес-приложения MacOS в пакете набора</span><span class="sxs-lookup"><span data-stu-id="4d42d-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="4d42d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d42d-107">Properties</span></span>
|<span data-ttu-id="4d42d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d42d-108">Property</span></span>|<span data-ttu-id="4d42d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4d42d-109">Type</span></span>|<span data-ttu-id="4d42d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4d42d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d42d-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="4d42d-111">bundleId</span></span>|<span data-ttu-id="4d42d-112">String</span><span class="sxs-lookup"><span data-stu-id="4d42d-112">String</span></span>|<span data-ttu-id="4d42d-113">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4d42d-113">The Identity Name.</span></span>|
|<span data-ttu-id="4d42d-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="4d42d-114">buildNumber</span></span>|<span data-ttu-id="4d42d-115">String</span><span class="sxs-lookup"><span data-stu-id="4d42d-115">String</span></span>|<span data-ttu-id="4d42d-116">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="4d42d-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4d42d-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="4d42d-117">versionNumber</span></span>|<span data-ttu-id="4d42d-118">String</span><span class="sxs-lookup"><span data-stu-id="4d42d-118">String</span></span>|<span data-ttu-id="4d42d-119">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="4d42d-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d42d-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="4d42d-120">Relationships</span></span>
<span data-ttu-id="4d42d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4d42d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d42d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d42d-122">JSON Representation</span></span>
<span data-ttu-id="4d42d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d42d-123">Here is a JSON representation of the resource.</span></span>
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



