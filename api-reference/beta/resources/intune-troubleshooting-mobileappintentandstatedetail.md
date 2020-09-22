---
title: Тип ресурса Мобилеаппинтентандстатедетаил
description: Цель мобильного приложения и состояние установки для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2fa57fb4218d961d8d3e58eb284062998903325b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003593"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="e1e32-103">Тип ресурса Мобилеаппинтентандстатедетаил</span><span class="sxs-lookup"><span data-stu-id="e1e32-103">mobileAppIntentAndStateDetail resource type</span></span>

<span data-ttu-id="e1e32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1e32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1e32-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1e32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1e32-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1e32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1e32-107">Цель мобильного приложения и состояние установки для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="e1e32-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="e1e32-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1e32-108">Properties</span></span>
|<span data-ttu-id="e1e32-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1e32-109">Property</span></span>|<span data-ttu-id="e1e32-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e1e32-110">Type</span></span>|<span data-ttu-id="e1e32-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e1e32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1e32-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="e1e32-112">applicationId</span></span>|<span data-ttu-id="e1e32-113">String</span><span class="sxs-lookup"><span data-stu-id="e1e32-113">String</span></span>|<span data-ttu-id="e1e32-114">Идентификатор Мобиеапп.</span><span class="sxs-lookup"><span data-stu-id="e1e32-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="e1e32-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e1e32-115">displayName</span></span>|<span data-ttu-id="e1e32-116">String</span><span class="sxs-lookup"><span data-stu-id="e1e32-116">String</span></span>|<span data-ttu-id="e1e32-117">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e1e32-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="e1e32-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="e1e32-118">mobileAppIntent</span></span>|<span data-ttu-id="e1e32-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md);</span><span class="sxs-lookup"><span data-stu-id="e1e32-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)</span></span>|<span data-ttu-id="e1e32-120">Цель для мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e1e32-120">Mobile App Intent.</span></span> <span data-ttu-id="e1e32-121">Возможные значения: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="e1e32-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="e1e32-122">дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="e1e32-122">displayVersion</span></span>|<span data-ttu-id="e1e32-123">String</span><span class="sxs-lookup"><span data-stu-id="e1e32-123">String</span></span>|<span data-ttu-id="e1e32-124">Доступная для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="e1e32-124">Human readable version of the application</span></span>|
|<span data-ttu-id="e1e32-125">installState</span><span class="sxs-lookup"><span data-stu-id="e1e32-125">installState</span></span>|[<span data-ttu-id="e1e32-126">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="e1e32-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e1e32-127">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="e1e32-127">The install state of the app.</span></span> <span data-ttu-id="e1e32-128">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e1e32-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e1e32-129">суппортеддевицетипес</span><span class="sxs-lookup"><span data-stu-id="e1e32-129">supportedDeviceTypes</span></span>|<span data-ttu-id="e1e32-130">Коллекция [мобилеаппсуппортеддевицетипе](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="e1e32-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="e1e32-131">Поддерживаемые платформы для приложения.</span><span class="sxs-lookup"><span data-stu-id="e1e32-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1e32-132">Связи</span><span class="sxs-lookup"><span data-stu-id="e1e32-132">Relationships</span></span>
<span data-ttu-id="e1e32-133">Нет</span><span class="sxs-lookup"><span data-stu-id="e1e32-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1e32-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1e32-134">JSON Representation</span></span>
<span data-ttu-id="e1e32-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1e32-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndStateDetail",
  "applicationId": "String",
  "displayName": "String",
  "mobileAppIntent": "String",
  "displayVersion": "String",
  "installState": "String",
  "supportedDeviceTypes": [
    {
      "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
      "type": "String",
      "minimumOperatingSystemVersion": "String",
      "maximumOperatingSystemVersion": "String"
    }
  ]
}
```






