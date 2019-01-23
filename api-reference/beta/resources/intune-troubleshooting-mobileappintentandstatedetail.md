---
title: Тип ресурса mobileAppIntentAndStateDetail
description: Цель мобильные приложения и состояние установки для данного устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ef88a1fa346784ae00a125a487ca844c58d62eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414258"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="ddb4a-103">Тип ресурса mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="ddb4a-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="ddb4a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ddb4a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddb4a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddb4a-107">Цель мобильные приложения и состояние установки для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="ddb4a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ddb4a-108">Properties</span></span>
|<span data-ttu-id="ddb4a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddb4a-109">Property</span></span>|<span data-ttu-id="ddb4a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ddb4a-110">Type</span></span>|<span data-ttu-id="ddb4a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddb4a-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="ddb4a-112">applicationId</span></span>|<span data-ttu-id="ddb4a-113">String</span><span class="sxs-lookup"><span data-stu-id="ddb4a-113">String</span></span>|<span data-ttu-id="ddb4a-114">Идентификатор MobieApp.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="ddb4a-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ddb4a-115">displayName</span></span>|<span data-ttu-id="ddb4a-116">String</span><span class="sxs-lookup"><span data-stu-id="ddb4a-116">String</span></span>|<span data-ttu-id="ddb4a-117">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="ddb4a-118">mobileAppIntent;</span><span class="sxs-lookup"><span data-stu-id="ddb4a-118">mobileAppIntent</span></span>|<span data-ttu-id="ddb4a-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md);</span><span class="sxs-lookup"><span data-stu-id="ddb4a-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)</span></span>|<span data-ttu-id="ddb4a-120">Цель мобильных приложений.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-120">Mobile App Intent.</span></span> <span data-ttu-id="ddb4a-121">Возможные значения: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="ddb4a-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="ddb4a-122">displayVersion</span></span>|<span data-ttu-id="ddb4a-123">String</span><span class="sxs-lookup"><span data-stu-id="ddb4a-123">String</span></span>|<span data-ttu-id="ddb4a-124">Человеческого для чтения версию приложения</span><span class="sxs-lookup"><span data-stu-id="ddb4a-124">Human readable version of the application</span></span>|
|<span data-ttu-id="ddb4a-125">installState</span><span class="sxs-lookup"><span data-stu-id="ddb4a-125">installState</span></span>|[<span data-ttu-id="ddb4a-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="ddb4a-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="ddb4a-127">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-127">The install state of the app.</span></span> <span data-ttu-id="ddb4a-128">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="ddb4a-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="ddb4a-129">supportedDeviceTypes</span></span>|<span data-ttu-id="ddb4a-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ddb4a-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="ddb4a-131">Поддерживаемые платформы для приложения.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddb4a-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="ddb4a-132">Relationships</span></span>
<span data-ttu-id="ddb4a-133">Нет</span><span class="sxs-lookup"><span data-stu-id="ddb4a-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddb4a-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ddb4a-134">JSON Representation</span></span>
<span data-ttu-id="ddb4a-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddb4a-135">Here is a JSON representation of the resource.</span></span>
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




