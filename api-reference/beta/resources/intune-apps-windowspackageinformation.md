---
title: Тип ресурса windowsPackageInformation
description: Содержит свойства для сведения о пакете для строки Windows бизнес-приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f7f3cd593670e071ae62bdb287bcebeee01d555
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849534"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="a91d7-103">Тип ресурса windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="a91d7-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="a91d7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a91d7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a91d7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a91d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a91d7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a91d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a91d7-107">Содержит свойства для сведения о пакете для строки Windows бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="a91d7-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="a91d7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a91d7-108">Properties</span></span>
|<span data-ttu-id="a91d7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a91d7-109">Property</span></span>|<span data-ttu-id="a91d7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a91d7-110">Type</span></span>|<span data-ttu-id="a91d7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a91d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a91d7-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="a91d7-112">applicableArchitecture</span></span>|[<span data-ttu-id="a91d7-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a91d7-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a91d7-114">Архитектура Windows, для которого это приложение можно запустить на.</span><span class="sxs-lookup"><span data-stu-id="a91d7-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="a91d7-115">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="a91d7-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="a91d7-116">displayName</span><span class="sxs-lookup"><span data-stu-id="a91d7-116">displayName</span></span>|<span data-ttu-id="a91d7-117">Строка</span><span class="sxs-lookup"><span data-stu-id="a91d7-117">String</span></span>|<span data-ttu-id="a91d7-118">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="a91d7-118">The Display Name.</span></span>|
|<span data-ttu-id="a91d7-119">identityName</span><span class="sxs-lookup"><span data-stu-id="a91d7-119">identityName</span></span>|<span data-ttu-id="a91d7-120">String</span><span class="sxs-lookup"><span data-stu-id="a91d7-120">String</span></span>|<span data-ttu-id="a91d7-121">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a91d7-121">The Identity Name.</span></span>|
|<span data-ttu-id="a91d7-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="a91d7-122">identityPublisher</span></span>|<span data-ttu-id="a91d7-123">Строка</span><span class="sxs-lookup"><span data-stu-id="a91d7-123">String</span></span>|<span data-ttu-id="a91d7-124">Издатель удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a91d7-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="a91d7-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a91d7-125">identityResourceIdentifier</span></span>|<span data-ttu-id="a91d7-126">String</span><span class="sxs-lookup"><span data-stu-id="a91d7-126">String</span></span>|<span data-ttu-id="a91d7-127">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="a91d7-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="a91d7-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a91d7-128">identityVersion</span></span>|<span data-ttu-id="a91d7-129">String</span><span class="sxs-lookup"><span data-stu-id="a91d7-129">String</span></span>|<span data-ttu-id="a91d7-130">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a91d7-130">The Identity Version.</span></span>|
|<span data-ttu-id="a91d7-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a91d7-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a91d7-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a91d7-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="a91d7-133">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="a91d7-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a91d7-134">Связи</span><span class="sxs-lookup"><span data-stu-id="a91d7-134">Relationships</span></span>
<span data-ttu-id="a91d7-135">Нет</span><span class="sxs-lookup"><span data-stu-id="a91d7-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a91d7-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a91d7-136">JSON Representation</span></span>
<span data-ttu-id="a91d7-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a91d7-137">Here is a JSON representation of the resource.</span></span>
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





