---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34ad5669235df33a3933c34001da9bae993a8faf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458888"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="d557e-103">Тип ресурса Макослобчилдапп</span><span class="sxs-lookup"><span data-stu-id="d557e-103">macOSLobChildApp resource type</span></span>

<span data-ttu-id="d557e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d557e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d557e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d557e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d557e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d557e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d557e-107">Содержит свойства бизнес-приложения MacOS в пакете набора</span><span class="sxs-lookup"><span data-stu-id="d557e-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="d557e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d557e-108">Properties</span></span>
|<span data-ttu-id="d557e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d557e-109">Property</span></span>|<span data-ttu-id="d557e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d557e-110">Type</span></span>|<span data-ttu-id="d557e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d557e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d557e-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="d557e-112">bundleId</span></span>|<span data-ttu-id="d557e-113">String</span><span class="sxs-lookup"><span data-stu-id="d557e-113">String</span></span>|<span data-ttu-id="d557e-114">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d557e-114">The Identity Name.</span></span>|
|<span data-ttu-id="d557e-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="d557e-115">buildNumber</span></span>|<span data-ttu-id="d557e-116">String</span><span class="sxs-lookup"><span data-stu-id="d557e-116">String</span></span>|<span data-ttu-id="d557e-117">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="d557e-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d557e-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="d557e-118">versionNumber</span></span>|<span data-ttu-id="d557e-119">String</span><span class="sxs-lookup"><span data-stu-id="d557e-119">String</span></span>|<span data-ttu-id="d557e-120">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="d557e-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d557e-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d557e-121">Relationships</span></span>
<span data-ttu-id="d557e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d557e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d557e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d557e-123">JSON Representation</span></span>
<span data-ttu-id="d557e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d557e-124">Here is a JSON representation of the resource.</span></span>
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



