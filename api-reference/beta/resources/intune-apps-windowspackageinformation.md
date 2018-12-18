---
title: Тип ресурса windowsPackageInformation
description: Содержит свойства для сведения о пакете для строки Windows бизнес-приложения.
author: tfitzmac
ms.openlocfilehash: dcc277c610e6ceb27a94ab41993e599a258dd55e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342828"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="0c783-103">Тип ресурса windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="0c783-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="0c783-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c783-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c783-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c783-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c783-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0c783-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c783-107">Содержит свойства для сведения о пакете для строки Windows бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="0c783-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="0c783-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c783-108">Properties</span></span>
|<span data-ttu-id="0c783-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c783-109">Property</span></span>|<span data-ttu-id="0c783-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0c783-110">Type</span></span>|<span data-ttu-id="0c783-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c783-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c783-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="0c783-112">applicableArchitecture</span></span>|[<span data-ttu-id="0c783-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="0c783-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="0c783-114">Архитектура Windows, для которого это приложение можно запустить на.</span><span class="sxs-lookup"><span data-stu-id="0c783-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="0c783-115">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="0c783-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="0c783-116">displayName</span><span class="sxs-lookup"><span data-stu-id="0c783-116">displayName</span></span>|<span data-ttu-id="0c783-117">Строка</span><span class="sxs-lookup"><span data-stu-id="0c783-117">String</span></span>|<span data-ttu-id="0c783-118">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="0c783-118">The Display Name.</span></span>|
|<span data-ttu-id="0c783-119">identityName</span><span class="sxs-lookup"><span data-stu-id="0c783-119">identityName</span></span>|<span data-ttu-id="0c783-120">String</span><span class="sxs-lookup"><span data-stu-id="0c783-120">String</span></span>|<span data-ttu-id="0c783-121">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="0c783-121">The Identity Name.</span></span>|
|<span data-ttu-id="0c783-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="0c783-122">identityPublisher</span></span>|<span data-ttu-id="0c783-123">String.</span><span class="sxs-lookup"><span data-stu-id="0c783-123">String</span></span>|<span data-ttu-id="0c783-124">Издатель удостоверений.</span><span class="sxs-lookup"><span data-stu-id="0c783-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="0c783-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c783-125">identityResourceIdentifier</span></span>|<span data-ttu-id="0c783-126">String</span><span class="sxs-lookup"><span data-stu-id="0c783-126">String</span></span>|<span data-ttu-id="0c783-127">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="0c783-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="0c783-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="0c783-128">identityVersion</span></span>|<span data-ttu-id="0c783-129">String</span><span class="sxs-lookup"><span data-stu-id="0c783-129">String</span></span>|<span data-ttu-id="0c783-130">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="0c783-130">The Identity Version.</span></span>|
|<span data-ttu-id="0c783-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0c783-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0c783-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0c783-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="0c783-133">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="0c783-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c783-134">Связи</span><span class="sxs-lookup"><span data-stu-id="0c783-134">Relationships</span></span>
<span data-ttu-id="0c783-135">Нет</span><span class="sxs-lookup"><span data-stu-id="0c783-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c783-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c783-136">JSON Representation</span></span>
<span data-ttu-id="0c783-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c783-137">Here is a JSON representation of the resource.</span></span>
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





