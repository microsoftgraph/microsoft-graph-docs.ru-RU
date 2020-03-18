---
title: Тип ресурса Мобилеаппинтентандстатедетаил
description: Цель мобильного приложения и состояние установки для данного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 98b651168c9cb95e0672398ecad5b572be29de9e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764602"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="9fa01-103">Тип ресурса Мобилеаппинтентандстатедетаил</span><span class="sxs-lookup"><span data-stu-id="9fa01-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="9fa01-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fa01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fa01-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fa01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fa01-106">Цель мобильного приложения и состояние установки для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="9fa01-106">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="9fa01-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fa01-107">Properties</span></span>
|<span data-ttu-id="9fa01-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fa01-108">Property</span></span>|<span data-ttu-id="9fa01-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9fa01-109">Type</span></span>|<span data-ttu-id="9fa01-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9fa01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fa01-111">applicationId</span><span class="sxs-lookup"><span data-stu-id="9fa01-111">applicationId</span></span>|<span data-ttu-id="9fa01-112">String</span><span class="sxs-lookup"><span data-stu-id="9fa01-112">String</span></span>|<span data-ttu-id="9fa01-113">Идентификатор Мобиеапп.</span><span class="sxs-lookup"><span data-stu-id="9fa01-113">MobieApp identifier.</span></span>|
|<span data-ttu-id="9fa01-114">displayName</span><span class="sxs-lookup"><span data-stu-id="9fa01-114">displayName</span></span>|<span data-ttu-id="9fa01-115">String</span><span class="sxs-lookup"><span data-stu-id="9fa01-115">String</span></span>|<span data-ttu-id="9fa01-116">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9fa01-116">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="9fa01-117">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="9fa01-117">mobileAppIntent</span></span>|<span data-ttu-id="9fa01-118">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md);</span><span class="sxs-lookup"><span data-stu-id="9fa01-118">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)</span></span>|<span data-ttu-id="9fa01-119">Цель для мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9fa01-119">Mobile App Intent.</span></span> <span data-ttu-id="9fa01-120">Возможные значения: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="9fa01-120">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="9fa01-121">дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="9fa01-121">displayVersion</span></span>|<span data-ttu-id="9fa01-122">String</span><span class="sxs-lookup"><span data-stu-id="9fa01-122">String</span></span>|<span data-ttu-id="9fa01-123">Доступная для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="9fa01-123">Human readable version of the application</span></span>|
|<span data-ttu-id="9fa01-124">installState</span><span class="sxs-lookup"><span data-stu-id="9fa01-124">installState</span></span>|[<span data-ttu-id="9fa01-125">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="9fa01-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="9fa01-126">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="9fa01-126">The install state of the app.</span></span> <span data-ttu-id="9fa01-127">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="9fa01-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="9fa01-128">суппортеддевицетипес</span><span class="sxs-lookup"><span data-stu-id="9fa01-128">supportedDeviceTypes</span></span>|<span data-ttu-id="9fa01-129">Коллекция [мобилеаппсуппортеддевицетипе](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="9fa01-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="9fa01-130">Поддерживаемые платформы для приложения.</span><span class="sxs-lookup"><span data-stu-id="9fa01-130">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fa01-131">Связи</span><span class="sxs-lookup"><span data-stu-id="9fa01-131">Relationships</span></span>
<span data-ttu-id="9fa01-132">Нет</span><span class="sxs-lookup"><span data-stu-id="9fa01-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fa01-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fa01-133">JSON Representation</span></span>
<span data-ttu-id="9fa01-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fa01-134">Here is a JSON representation of the resource.</span></span>
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



