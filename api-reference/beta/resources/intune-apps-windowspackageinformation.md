---
title: Тип ресурса windowsPackageInformation
description: Содержит свойства сведений о пакете для бизнес-приложения Для Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c53ce1f9dac5c4b01129df32ff96ceb8645a842a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154392"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="c18bd-103">Тип ресурса windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="c18bd-103">windowsPackageInformation resource type</span></span>

<span data-ttu-id="c18bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c18bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c18bd-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c18bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c18bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c18bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c18bd-107">Содержит свойства сведений о пакете для бизнес-приложения Для Windows.</span><span class="sxs-lookup"><span data-stu-id="c18bd-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="c18bd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c18bd-108">Properties</span></span>
|<span data-ttu-id="c18bd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c18bd-109">Property</span></span>|<span data-ttu-id="c18bd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c18bd-110">Type</span></span>|<span data-ttu-id="c18bd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c18bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c18bd-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="c18bd-112">applicableArchitecture</span></span>|[<span data-ttu-id="c18bd-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="c18bd-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="c18bd-114">Архитектура Windows, для которой может работать это приложение.</span><span class="sxs-lookup"><span data-stu-id="c18bd-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="c18bd-115">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="c18bd-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="c18bd-116">displayName</span><span class="sxs-lookup"><span data-stu-id="c18bd-116">displayName</span></span>|<span data-ttu-id="c18bd-117">String</span><span class="sxs-lookup"><span data-stu-id="c18bd-117">String</span></span>|<span data-ttu-id="c18bd-118">Отображаемая фамилия.</span><span class="sxs-lookup"><span data-stu-id="c18bd-118">The Display Name.</span></span>|
|<span data-ttu-id="c18bd-119">identityName</span><span class="sxs-lookup"><span data-stu-id="c18bd-119">identityName</span></span>|<span data-ttu-id="c18bd-120">String</span><span class="sxs-lookup"><span data-stu-id="c18bd-120">String</span></span>|<span data-ttu-id="c18bd-121">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c18bd-121">The Identity Name.</span></span>|
|<span data-ttu-id="c18bd-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="c18bd-122">identityPublisher</span></span>|<span data-ttu-id="c18bd-123">String</span><span class="sxs-lookup"><span data-stu-id="c18bd-123">String</span></span>|<span data-ttu-id="c18bd-124">Издатель удостоверений.</span><span class="sxs-lookup"><span data-stu-id="c18bd-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="c18bd-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c18bd-125">identityResourceIdentifier</span></span>|<span data-ttu-id="c18bd-126">String</span><span class="sxs-lookup"><span data-stu-id="c18bd-126">String</span></span>|<span data-ttu-id="c18bd-127">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="c18bd-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="c18bd-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="c18bd-128">identityVersion</span></span>|<span data-ttu-id="c18bd-129">String</span><span class="sxs-lookup"><span data-stu-id="c18bd-129">String</span></span>|<span data-ttu-id="c18bd-130">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c18bd-130">The Identity Version.</span></span>|
|<span data-ttu-id="c18bd-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c18bd-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c18bd-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c18bd-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="c18bd-133">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="c18bd-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c18bd-134">Связи</span><span class="sxs-lookup"><span data-stu-id="c18bd-134">Relationships</span></span>
<span data-ttu-id="c18bd-135">Нет</span><span class="sxs-lookup"><span data-stu-id="c18bd-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c18bd-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c18bd-136">JSON Representation</span></span>
<span data-ttu-id="c18bd-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c18bd-137">Here is a JSON representation of the resource.</span></span>
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
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  }
}
```




