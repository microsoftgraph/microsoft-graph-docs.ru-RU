---
title: Тип ресурса windowsPackageInformation
description: Содержит свойства для сведений о пакете для бизнес-приложения Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9a7871a101062e9d835c68f37299d83a8bfb5e8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726558"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="91b6a-103">Тип ресурса windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="91b6a-103">windowsPackageInformation resource type</span></span>

<span data-ttu-id="91b6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91b6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91b6a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91b6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91b6a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91b6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91b6a-107">Содержит свойства для сведений о пакете для бизнес-приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="91b6a-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="91b6a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="91b6a-108">Properties</span></span>
|<span data-ttu-id="91b6a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="91b6a-109">Property</span></span>|<span data-ttu-id="91b6a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="91b6a-110">Type</span></span>|<span data-ttu-id="91b6a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="91b6a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91b6a-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="91b6a-112">applicableArchitecture</span></span>|[<span data-ttu-id="91b6a-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="91b6a-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="91b6a-114">Архитектура Windows, в которой можно запустить это приложение.</span><span class="sxs-lookup"><span data-stu-id="91b6a-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="91b6a-115">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="91b6a-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="91b6a-116">displayName</span><span class="sxs-lookup"><span data-stu-id="91b6a-116">displayName</span></span>|<span data-ttu-id="91b6a-117">Строка</span><span class="sxs-lookup"><span data-stu-id="91b6a-117">String</span></span>|<span data-ttu-id="91b6a-118">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="91b6a-118">The Display Name.</span></span>|
|<span data-ttu-id="91b6a-119">identityName</span><span class="sxs-lookup"><span data-stu-id="91b6a-119">identityName</span></span>|<span data-ttu-id="91b6a-120">String</span><span class="sxs-lookup"><span data-stu-id="91b6a-120">String</span></span>|<span data-ttu-id="91b6a-121">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="91b6a-121">The Identity Name.</span></span>|
|<span data-ttu-id="91b6a-122">идентитипублишер</span><span class="sxs-lookup"><span data-stu-id="91b6a-122">identityPublisher</span></span>|<span data-ttu-id="91b6a-123">Строка</span><span class="sxs-lookup"><span data-stu-id="91b6a-123">String</span></span>|<span data-ttu-id="91b6a-124">Издатель удостоверений.</span><span class="sxs-lookup"><span data-stu-id="91b6a-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="91b6a-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="91b6a-125">identityResourceIdentifier</span></span>|<span data-ttu-id="91b6a-126">String</span><span class="sxs-lookup"><span data-stu-id="91b6a-126">String</span></span>|<span data-ttu-id="91b6a-127">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="91b6a-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="91b6a-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="91b6a-128">identityVersion</span></span>|<span data-ttu-id="91b6a-129">String</span><span class="sxs-lookup"><span data-stu-id="91b6a-129">String</span></span>|<span data-ttu-id="91b6a-130">Версия идентификатора.</span><span class="sxs-lookup"><span data-stu-id="91b6a-130">The Identity Version.</span></span>|
|<span data-ttu-id="91b6a-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="91b6a-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="91b6a-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="91b6a-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="91b6a-133">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="91b6a-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91b6a-134">Связи</span><span class="sxs-lookup"><span data-stu-id="91b6a-134">Relationships</span></span>
<span data-ttu-id="91b6a-135">Нет</span><span class="sxs-lookup"><span data-stu-id="91b6a-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91b6a-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91b6a-136">JSON Representation</span></span>
<span data-ttu-id="91b6a-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91b6a-137">Here is a JSON representation of the resource.</span></span>
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





