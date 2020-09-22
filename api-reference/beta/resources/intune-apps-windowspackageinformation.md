---
title: Тип ресурса windowsPackageInformation
description: Содержит свойства для сведений о пакете для бизнес-приложения Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d743454f5b0acfa9a8ba6c1b205d67fcb3c11595
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070921"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="2f2f7-103">Тип ресурса windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="2f2f7-103">windowsPackageInformation resource type</span></span>

<span data-ttu-id="2f2f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f2f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f2f7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f2f7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f2f7-107">Содержит свойства для сведений о пакете для бизнес-приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="2f2f7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f2f7-108">Properties</span></span>
|<span data-ttu-id="2f2f7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f2f7-109">Property</span></span>|<span data-ttu-id="2f2f7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2f2f7-110">Type</span></span>|<span data-ttu-id="2f2f7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2f2f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f2f7-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="2f2f7-112">applicableArchitecture</span></span>|[<span data-ttu-id="2f2f7-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="2f2f7-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="2f2f7-114">Архитектура Windows, в которой можно запустить это приложение.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="2f2f7-115">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="2f2f7-116">displayName</span><span class="sxs-lookup"><span data-stu-id="2f2f7-116">displayName</span></span>|<span data-ttu-id="2f2f7-117">String</span><span class="sxs-lookup"><span data-stu-id="2f2f7-117">String</span></span>|<span data-ttu-id="2f2f7-118">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-118">The Display Name.</span></span>|
|<span data-ttu-id="2f2f7-119">identityName</span><span class="sxs-lookup"><span data-stu-id="2f2f7-119">identityName</span></span>|<span data-ttu-id="2f2f7-120">String</span><span class="sxs-lookup"><span data-stu-id="2f2f7-120">String</span></span>|<span data-ttu-id="2f2f7-121">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-121">The Identity Name.</span></span>|
|<span data-ttu-id="2f2f7-122">идентитипублишер</span><span class="sxs-lookup"><span data-stu-id="2f2f7-122">identityPublisher</span></span>|<span data-ttu-id="2f2f7-123">String</span><span class="sxs-lookup"><span data-stu-id="2f2f7-123">String</span></span>|<span data-ttu-id="2f2f7-124">Издатель удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="2f2f7-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f2f7-125">identityResourceIdentifier</span></span>|<span data-ttu-id="2f2f7-126">String</span><span class="sxs-lookup"><span data-stu-id="2f2f7-126">String</span></span>|<span data-ttu-id="2f2f7-127">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="2f2f7-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2f2f7-128">identityVersion</span></span>|<span data-ttu-id="2f2f7-129">String</span><span class="sxs-lookup"><span data-stu-id="2f2f7-129">String</span></span>|<span data-ttu-id="2f2f7-130">Версия идентификатора.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-130">The Identity Version.</span></span>|
|<span data-ttu-id="2f2f7-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2f2f7-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2f2f7-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2f2f7-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="2f2f7-133">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f2f7-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="2f2f7-134">Relationships</span></span>
<span data-ttu-id="2f2f7-135">Нет</span><span class="sxs-lookup"><span data-stu-id="2f2f7-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f2f7-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f2f7-136">JSON Representation</span></span>
<span data-ttu-id="2f2f7-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f2f7-137">Here is a JSON representation of the resource.</span></span>
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






