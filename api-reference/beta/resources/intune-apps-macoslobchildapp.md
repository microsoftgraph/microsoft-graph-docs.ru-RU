---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3eb06ecc8937fd8f2d6c8d74cd0aaf560a22b89c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989460"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="b6962-103">Тип ресурса Макослобчилдапп</span><span class="sxs-lookup"><span data-stu-id="b6962-103">macOSLobChildApp resource type</span></span>

<span data-ttu-id="b6962-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6962-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6962-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6962-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6962-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6962-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6962-107">Содержит свойства бизнес-приложения MacOS в пакете набора</span><span class="sxs-lookup"><span data-stu-id="b6962-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="b6962-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6962-108">Properties</span></span>
|<span data-ttu-id="b6962-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6962-109">Property</span></span>|<span data-ttu-id="b6962-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b6962-110">Type</span></span>|<span data-ttu-id="b6962-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b6962-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6962-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="b6962-112">bundleId</span></span>|<span data-ttu-id="b6962-113">String</span><span class="sxs-lookup"><span data-stu-id="b6962-113">String</span></span>|<span data-ttu-id="b6962-114">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="b6962-114">The Identity Name.</span></span>|
|<span data-ttu-id="b6962-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="b6962-115">buildNumber</span></span>|<span data-ttu-id="b6962-116">String</span><span class="sxs-lookup"><span data-stu-id="b6962-116">String</span></span>|<span data-ttu-id="b6962-117">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="b6962-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b6962-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="b6962-118">versionNumber</span></span>|<span data-ttu-id="b6962-119">String</span><span class="sxs-lookup"><span data-stu-id="b6962-119">String</span></span>|<span data-ttu-id="b6962-120">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="b6962-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6962-121">Связи</span><span class="sxs-lookup"><span data-stu-id="b6962-121">Relationships</span></span>
<span data-ttu-id="b6962-122">Нет</span><span class="sxs-lookup"><span data-stu-id="b6962-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6962-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6962-123">JSON Representation</span></span>
<span data-ttu-id="b6962-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6962-124">Here is a JSON representation of the resource.</span></span>
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






