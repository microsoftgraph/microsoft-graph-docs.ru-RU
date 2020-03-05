---
title: Тип ресурса Мобилеаппинтентандстатедетаил
description: Цель мобильного приложения и состояние установки для данного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 598cacd35ba5416c51388ef6ecb101d302ad9864
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523333"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="87058-103">Тип ресурса Мобилеаппинтентандстатедетаил</span><span class="sxs-lookup"><span data-stu-id="87058-103">mobileAppIntentAndStateDetail resource type</span></span>

<span data-ttu-id="87058-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="87058-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87058-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87058-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87058-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87058-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87058-107">Цель мобильного приложения и состояние установки для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="87058-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="87058-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="87058-108">Properties</span></span>
|<span data-ttu-id="87058-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="87058-109">Property</span></span>|<span data-ttu-id="87058-110">Тип</span><span class="sxs-lookup"><span data-stu-id="87058-110">Type</span></span>|<span data-ttu-id="87058-111">Описание</span><span class="sxs-lookup"><span data-stu-id="87058-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87058-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="87058-112">applicationId</span></span>|<span data-ttu-id="87058-113">String</span><span class="sxs-lookup"><span data-stu-id="87058-113">String</span></span>|<span data-ttu-id="87058-114">Идентификатор Мобиеапп.</span><span class="sxs-lookup"><span data-stu-id="87058-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="87058-115">displayName</span><span class="sxs-lookup"><span data-stu-id="87058-115">displayName</span></span>|<span data-ttu-id="87058-116">String</span><span class="sxs-lookup"><span data-stu-id="87058-116">String</span></span>|<span data-ttu-id="87058-117">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="87058-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="87058-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="87058-118">mobileAppIntent</span></span>|<span data-ttu-id="87058-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md);</span><span class="sxs-lookup"><span data-stu-id="87058-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)</span></span>|<span data-ttu-id="87058-120">Цель для мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="87058-120">Mobile App Intent.</span></span> <span data-ttu-id="87058-121">Возможные значения: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="87058-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="87058-122">дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="87058-122">displayVersion</span></span>|<span data-ttu-id="87058-123">String</span><span class="sxs-lookup"><span data-stu-id="87058-123">String</span></span>|<span data-ttu-id="87058-124">Доступная для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="87058-124">Human readable version of the application</span></span>|
|<span data-ttu-id="87058-125">installState</span><span class="sxs-lookup"><span data-stu-id="87058-125">installState</span></span>|[<span data-ttu-id="87058-126">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="87058-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="87058-127">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="87058-127">The install state of the app.</span></span> <span data-ttu-id="87058-128">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="87058-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="87058-129">суппортеддевицетипес</span><span class="sxs-lookup"><span data-stu-id="87058-129">supportedDeviceTypes</span></span>|<span data-ttu-id="87058-130">Коллекция [мобилеаппсуппортеддевицетипе](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="87058-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="87058-131">Поддерживаемые платформы для приложения.</span><span class="sxs-lookup"><span data-stu-id="87058-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87058-132">Связи</span><span class="sxs-lookup"><span data-stu-id="87058-132">Relationships</span></span>
<span data-ttu-id="87058-133">Нет</span><span class="sxs-lookup"><span data-stu-id="87058-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87058-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87058-134">JSON Representation</span></span>
<span data-ttu-id="87058-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87058-135">Here is a JSON representation of the resource.</span></span>
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



