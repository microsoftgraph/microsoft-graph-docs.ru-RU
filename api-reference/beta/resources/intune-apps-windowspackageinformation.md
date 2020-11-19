---
title: Тип ресурса windowsPackageInformation
description: Содержит свойства для сведений о пакете для бизнес-приложения Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 409d9aedf0ef42114269b1d1d23e9fd5d08e8faa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284276"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="f7244-103">Тип ресурса windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="f7244-103">windowsPackageInformation resource type</span></span>

<span data-ttu-id="f7244-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7244-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7244-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7244-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7244-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7244-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7244-107">Содержит свойства для сведений о пакете для бизнес-приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="f7244-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="f7244-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7244-108">Properties</span></span>
|<span data-ttu-id="f7244-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7244-109">Property</span></span>|<span data-ttu-id="f7244-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f7244-110">Type</span></span>|<span data-ttu-id="f7244-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f7244-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7244-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="f7244-112">applicableArchitecture</span></span>|[<span data-ttu-id="f7244-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f7244-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f7244-114">Архитектура Windows, в которой можно запустить это приложение.</span><span class="sxs-lookup"><span data-stu-id="f7244-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="f7244-115">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="f7244-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="f7244-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f7244-116">displayName</span></span>|<span data-ttu-id="f7244-117">String</span><span class="sxs-lookup"><span data-stu-id="f7244-117">String</span></span>|<span data-ttu-id="f7244-118">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="f7244-118">The Display Name.</span></span>|
|<span data-ttu-id="f7244-119">identityName</span><span class="sxs-lookup"><span data-stu-id="f7244-119">identityName</span></span>|<span data-ttu-id="f7244-120">String</span><span class="sxs-lookup"><span data-stu-id="f7244-120">String</span></span>|<span data-ttu-id="f7244-121">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f7244-121">The Identity Name.</span></span>|
|<span data-ttu-id="f7244-122">идентитипублишер</span><span class="sxs-lookup"><span data-stu-id="f7244-122">identityPublisher</span></span>|<span data-ttu-id="f7244-123">String</span><span class="sxs-lookup"><span data-stu-id="f7244-123">String</span></span>|<span data-ttu-id="f7244-124">Издатель удостоверений.</span><span class="sxs-lookup"><span data-stu-id="f7244-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="f7244-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f7244-125">identityResourceIdentifier</span></span>|<span data-ttu-id="f7244-126">String</span><span class="sxs-lookup"><span data-stu-id="f7244-126">String</span></span>|<span data-ttu-id="f7244-127">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="f7244-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="f7244-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f7244-128">identityVersion</span></span>|<span data-ttu-id="f7244-129">String</span><span class="sxs-lookup"><span data-stu-id="f7244-129">String</span></span>|<span data-ttu-id="f7244-130">Версия идентификатора.</span><span class="sxs-lookup"><span data-stu-id="f7244-130">The Identity Version.</span></span>|
|<span data-ttu-id="f7244-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f7244-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f7244-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f7244-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f7244-133">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="f7244-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7244-134">Связи</span><span class="sxs-lookup"><span data-stu-id="f7244-134">Relationships</span></span>
<span data-ttu-id="f7244-135">Нет</span><span class="sxs-lookup"><span data-stu-id="f7244-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7244-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7244-136">JSON Representation</span></span>
<span data-ttu-id="f7244-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7244-137">Here is a JSON representation of the resource.</span></span>
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




