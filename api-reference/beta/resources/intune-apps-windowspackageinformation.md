---
title: Тип ресурса windowsPackageInformation
description: Содержит свойства для сведений о пакете для бизнес-приложения Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2803779830d0e2bb88a0a91a96abfc101d15cb66
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949502"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="7c21f-103">Тип ресурса windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="7c21f-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="7c21f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c21f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c21f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c21f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c21f-106">Содержит свойства для сведений о пакете для бизнес-приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="7c21f-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="7c21f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c21f-107">Properties</span></span>
|<span data-ttu-id="7c21f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c21f-108">Property</span></span>|<span data-ttu-id="7c21f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7c21f-109">Type</span></span>|<span data-ttu-id="7c21f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7c21f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c21f-111">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="7c21f-111">applicableArchitecture</span></span>|[<span data-ttu-id="7c21f-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7c21f-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7c21f-113">Архитектура Windows, в которой можно запустить это приложение.</span><span class="sxs-lookup"><span data-stu-id="7c21f-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="7c21f-114">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="7c21f-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="7c21f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="7c21f-115">displayName</span></span>|<span data-ttu-id="7c21f-116">Строка</span><span class="sxs-lookup"><span data-stu-id="7c21f-116">String</span></span>|<span data-ttu-id="7c21f-117">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="7c21f-117">The Display Name.</span></span>|
|<span data-ttu-id="7c21f-118">identityName</span><span class="sxs-lookup"><span data-stu-id="7c21f-118">identityName</span></span>|<span data-ttu-id="7c21f-119">Строка</span><span class="sxs-lookup"><span data-stu-id="7c21f-119">String</span></span>|<span data-ttu-id="7c21f-120">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7c21f-120">The Identity Name.</span></span>|
|<span data-ttu-id="7c21f-121">Идентитипублишер</span><span class="sxs-lookup"><span data-stu-id="7c21f-121">identityPublisher</span></span>|<span data-ttu-id="7c21f-122">Строка</span><span class="sxs-lookup"><span data-stu-id="7c21f-122">String</span></span>|<span data-ttu-id="7c21f-123">Издатель удостоверений.</span><span class="sxs-lookup"><span data-stu-id="7c21f-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="7c21f-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7c21f-124">identityResourceIdentifier</span></span>|<span data-ttu-id="7c21f-125">String</span><span class="sxs-lookup"><span data-stu-id="7c21f-125">String</span></span>|<span data-ttu-id="7c21f-126">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="7c21f-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="7c21f-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7c21f-127">identityVersion</span></span>|<span data-ttu-id="7c21f-128">String</span><span class="sxs-lookup"><span data-stu-id="7c21f-128">String</span></span>|<span data-ttu-id="7c21f-129">Версия идентификатора.</span><span class="sxs-lookup"><span data-stu-id="7c21f-129">The Identity Version.</span></span>|
|<span data-ttu-id="7c21f-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7c21f-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7c21f-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7c21f-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7c21f-132">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="7c21f-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c21f-133">Связи</span><span class="sxs-lookup"><span data-stu-id="7c21f-133">Relationships</span></span>
<span data-ttu-id="7c21f-134">Нет</span><span class="sxs-lookup"><span data-stu-id="7c21f-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c21f-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c21f-135">JSON Representation</span></span>
<span data-ttu-id="7c21f-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c21f-136">Here is a JSON representation of the resource.</span></span>
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
    "v10_1803": true
  }
}
```




