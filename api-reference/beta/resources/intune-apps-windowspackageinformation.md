---
title: Тип ресурса windowsPackageInformation
description: Содержит свойства для сведений о пакете для бизнес-приложения Windows.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 31c99e8732f100e7d4797fda7d4c71a5086bd227
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797495"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="3ab0a-103">Тип ресурса windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="3ab0a-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="3ab0a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ab0a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ab0a-106">Содержит свойства для сведений о пакете для бизнес-приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="3ab0a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ab0a-107">Properties</span></span>
|<span data-ttu-id="3ab0a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ab0a-108">Property</span></span>|<span data-ttu-id="3ab0a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3ab0a-109">Type</span></span>|<span data-ttu-id="3ab0a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3ab0a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ab0a-111">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="3ab0a-111">applicableArchitecture</span></span>|[<span data-ttu-id="3ab0a-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="3ab0a-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="3ab0a-113">Архитектура Windows, в которой можно запустить это приложение.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="3ab0a-114">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="3ab0a-115">displayName</span><span class="sxs-lookup"><span data-stu-id="3ab0a-115">displayName</span></span>|<span data-ttu-id="3ab0a-116">String</span><span class="sxs-lookup"><span data-stu-id="3ab0a-116">String</span></span>|<span data-ttu-id="3ab0a-117">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-117">The Display Name.</span></span>|
|<span data-ttu-id="3ab0a-118">identityName</span><span class="sxs-lookup"><span data-stu-id="3ab0a-118">identityName</span></span>|<span data-ttu-id="3ab0a-119">String</span><span class="sxs-lookup"><span data-stu-id="3ab0a-119">String</span></span>|<span data-ttu-id="3ab0a-120">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-120">The Identity Name.</span></span>|
|<span data-ttu-id="3ab0a-121">идентитипублишер</span><span class="sxs-lookup"><span data-stu-id="3ab0a-121">identityPublisher</span></span>|<span data-ttu-id="3ab0a-122">String</span><span class="sxs-lookup"><span data-stu-id="3ab0a-122">String</span></span>|<span data-ttu-id="3ab0a-123">Издатель удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="3ab0a-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3ab0a-124">identityResourceIdentifier</span></span>|<span data-ttu-id="3ab0a-125">String</span><span class="sxs-lookup"><span data-stu-id="3ab0a-125">String</span></span>|<span data-ttu-id="3ab0a-126">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="3ab0a-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3ab0a-127">identityVersion</span></span>|<span data-ttu-id="3ab0a-128">String</span><span class="sxs-lookup"><span data-stu-id="3ab0a-128">String</span></span>|<span data-ttu-id="3ab0a-129">Версия идентификатора.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-129">The Identity Version.</span></span>|
|<span data-ttu-id="3ab0a-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3ab0a-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3ab0a-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3ab0a-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="3ab0a-132">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ab0a-133">Связи</span><span class="sxs-lookup"><span data-stu-id="3ab0a-133">Relationships</span></span>
<span data-ttu-id="3ab0a-134">Нет</span><span class="sxs-lookup"><span data-stu-id="3ab0a-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ab0a-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ab0a-135">JSON Representation</span></span>
<span data-ttu-id="3ab0a-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ab0a-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsPackageInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPackageInformation",
  "applicableArchitecture": "String",
  "displayName": "String",
  "identityName": "String",
  "identityPublisher": "String",
  "identityResourceIdentifier": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  }
}
```



