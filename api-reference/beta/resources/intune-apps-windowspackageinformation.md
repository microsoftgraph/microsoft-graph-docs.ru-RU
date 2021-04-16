---
title: тип ресурса windowsPackageInformation
description: Содержит свойства для сведений о пакете для бизнес-приложения Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b2474fe5458c7a8c8fcc54d354f46ec7386952e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866309"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="9cca8-103">тип ресурса windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="9cca8-103">windowsPackageInformation resource type</span></span>

<span data-ttu-id="9cca8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cca8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cca8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cca8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cca8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cca8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cca8-107">Содержит свойства для сведений о пакете для бизнес-приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="9cca8-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="9cca8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cca8-108">Properties</span></span>
|<span data-ttu-id="9cca8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cca8-109">Property</span></span>|<span data-ttu-id="9cca8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9cca8-110">Type</span></span>|<span data-ttu-id="9cca8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9cca8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cca8-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="9cca8-112">applicableArchitecture</span></span>|[<span data-ttu-id="9cca8-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9cca8-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9cca8-114">Архитектура Windows, для которой это приложение может работать.</span><span class="sxs-lookup"><span data-stu-id="9cca8-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="9cca8-115">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="9cca8-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="9cca8-116">displayName</span><span class="sxs-lookup"><span data-stu-id="9cca8-116">displayName</span></span>|<span data-ttu-id="9cca8-117">String</span><span class="sxs-lookup"><span data-stu-id="9cca8-117">String</span></span>|<span data-ttu-id="9cca8-118">Имя отображения.</span><span class="sxs-lookup"><span data-stu-id="9cca8-118">The Display Name.</span></span>|
|<span data-ttu-id="9cca8-119">identityName</span><span class="sxs-lookup"><span data-stu-id="9cca8-119">identityName</span></span>|<span data-ttu-id="9cca8-120">String</span><span class="sxs-lookup"><span data-stu-id="9cca8-120">String</span></span>|<span data-ttu-id="9cca8-121">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9cca8-121">The Identity Name.</span></span>|
|<span data-ttu-id="9cca8-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="9cca8-122">identityPublisher</span></span>|<span data-ttu-id="9cca8-123">String</span><span class="sxs-lookup"><span data-stu-id="9cca8-123">String</span></span>|<span data-ttu-id="9cca8-124">Издатель удостоверений.</span><span class="sxs-lookup"><span data-stu-id="9cca8-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="9cca8-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9cca8-125">identityResourceIdentifier</span></span>|<span data-ttu-id="9cca8-126">String</span><span class="sxs-lookup"><span data-stu-id="9cca8-126">String</span></span>|<span data-ttu-id="9cca8-127">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="9cca8-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="9cca8-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9cca8-128">identityVersion</span></span>|<span data-ttu-id="9cca8-129">String</span><span class="sxs-lookup"><span data-stu-id="9cca8-129">String</span></span>|<span data-ttu-id="9cca8-130">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9cca8-130">The Identity Version.</span></span>|
|<span data-ttu-id="9cca8-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9cca8-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9cca8-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9cca8-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9cca8-133">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9cca8-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cca8-134">Связи</span><span class="sxs-lookup"><span data-stu-id="9cca8-134">Relationships</span></span>
<span data-ttu-id="9cca8-135">Нет</span><span class="sxs-lookup"><span data-stu-id="9cca8-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cca8-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cca8-136">JSON Representation</span></span>
<span data-ttu-id="9cca8-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cca8-137">Here is a JSON representation of the resource.</span></span>
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
    "v10_2004": true,
    "v10_2H20": true
  }
}
```




