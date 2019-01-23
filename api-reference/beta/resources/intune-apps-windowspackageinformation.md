---
title: Тип ресурса windowsPackageInformation
description: Содержит свойства для сведения о пакете для строки Windows бизнес-приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 112d84c5bae889e24b889b4598d61a6b3d63db50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403282"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="748e3-103">Тип ресурса windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="748e3-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="748e3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="748e3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="748e3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="748e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="748e3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="748e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="748e3-107">Содержит свойства для сведения о пакете для строки Windows бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="748e3-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="748e3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="748e3-108">Properties</span></span>
|<span data-ttu-id="748e3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="748e3-109">Property</span></span>|<span data-ttu-id="748e3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="748e3-110">Type</span></span>|<span data-ttu-id="748e3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="748e3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="748e3-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="748e3-112">applicableArchitecture</span></span>|[<span data-ttu-id="748e3-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="748e3-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="748e3-114">Архитектура Windows, для которого это приложение можно запустить на.</span><span class="sxs-lookup"><span data-stu-id="748e3-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="748e3-115">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="748e3-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="748e3-116">displayName</span><span class="sxs-lookup"><span data-stu-id="748e3-116">displayName</span></span>|<span data-ttu-id="748e3-117">String</span><span class="sxs-lookup"><span data-stu-id="748e3-117">String</span></span>|<span data-ttu-id="748e3-118">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="748e3-118">The Display Name.</span></span>|
|<span data-ttu-id="748e3-119">identityName</span><span class="sxs-lookup"><span data-stu-id="748e3-119">identityName</span></span>|<span data-ttu-id="748e3-120">String</span><span class="sxs-lookup"><span data-stu-id="748e3-120">String</span></span>|<span data-ttu-id="748e3-121">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="748e3-121">The Identity Name.</span></span>|
|<span data-ttu-id="748e3-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="748e3-122">identityPublisher</span></span>|<span data-ttu-id="748e3-123">String</span><span class="sxs-lookup"><span data-stu-id="748e3-123">String</span></span>|<span data-ttu-id="748e3-124">Издатель удостоверений.</span><span class="sxs-lookup"><span data-stu-id="748e3-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="748e3-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="748e3-125">identityResourceIdentifier</span></span>|<span data-ttu-id="748e3-126">String</span><span class="sxs-lookup"><span data-stu-id="748e3-126">String</span></span>|<span data-ttu-id="748e3-127">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="748e3-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="748e3-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="748e3-128">identityVersion</span></span>|<span data-ttu-id="748e3-129">String</span><span class="sxs-lookup"><span data-stu-id="748e3-129">String</span></span>|<span data-ttu-id="748e3-130">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="748e3-130">The Identity Version.</span></span>|
|<span data-ttu-id="748e3-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="748e3-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="748e3-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="748e3-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="748e3-133">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="748e3-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="748e3-134">Связи</span><span class="sxs-lookup"><span data-stu-id="748e3-134">Relationships</span></span>
<span data-ttu-id="748e3-135">Нет</span><span class="sxs-lookup"><span data-stu-id="748e3-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="748e3-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="748e3-136">JSON Representation</span></span>
<span data-ttu-id="748e3-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="748e3-137">Here is a JSON representation of the resource.</span></span>
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




