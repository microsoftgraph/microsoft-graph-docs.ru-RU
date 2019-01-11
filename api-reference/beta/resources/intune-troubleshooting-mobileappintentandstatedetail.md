---
title: Тип ресурса mobileAppIntentAndStateDetail
description: Цель мобильные приложения и состояние установки для данного устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ad20ef00cbc8e5295a96107fbce2f5e7f1cb978a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805812"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="d2ceb-103">Тип ресурса mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="d2ceb-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="d2ceb-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2ceb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2ceb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2ceb-107">Цель мобильные приложения и состояние установки для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-107">Mobile App Intent and Install State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="d2ceb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2ceb-108">Properties</span></span>
|<span data-ttu-id="d2ceb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2ceb-109">Property</span></span>|<span data-ttu-id="d2ceb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d2ceb-110">Type</span></span>|<span data-ttu-id="d2ceb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d2ceb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2ceb-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="d2ceb-112">applicationId</span></span>|<span data-ttu-id="d2ceb-113">String</span><span class="sxs-lookup"><span data-stu-id="d2ceb-113">String</span></span>|<span data-ttu-id="d2ceb-114">Идентификатор MobieApp.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="d2ceb-115">displayName</span><span class="sxs-lookup"><span data-stu-id="d2ceb-115">displayName</span></span>|<span data-ttu-id="d2ceb-116">String</span><span class="sxs-lookup"><span data-stu-id="d2ceb-116">String</span></span>|<span data-ttu-id="d2ceb-117">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="d2ceb-118">mobileAppIntent;</span><span class="sxs-lookup"><span data-stu-id="d2ceb-118">mobileAppIntent</span></span>|<span data-ttu-id="d2ceb-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md);</span><span class="sxs-lookup"><span data-stu-id="d2ceb-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)</span></span>|<span data-ttu-id="d2ceb-120">Цель мобильных приложений.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-120">Mobile App Intent.</span></span> <span data-ttu-id="d2ceb-121">Возможные значения: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="d2ceb-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="d2ceb-122">displayVersion</span></span>|<span data-ttu-id="d2ceb-123">Строка</span><span class="sxs-lookup"><span data-stu-id="d2ceb-123">String</span></span>|<span data-ttu-id="d2ceb-124">Человеческого для чтения версию приложения</span><span class="sxs-lookup"><span data-stu-id="d2ceb-124">Human readable version of the application</span></span>|
|<span data-ttu-id="d2ceb-125">installState</span><span class="sxs-lookup"><span data-stu-id="d2ceb-125">installState</span></span>|[<span data-ttu-id="d2ceb-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d2ceb-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="d2ceb-127">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-127">The install state of the app.</span></span> <span data-ttu-id="d2ceb-128">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="d2ceb-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="d2ceb-129">supportedDeviceTypes</span></span>|<span data-ttu-id="d2ceb-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d2ceb-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="d2ceb-131">Поддерживаемые платформы для приложения.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2ceb-132">Связи</span><span class="sxs-lookup"><span data-stu-id="d2ceb-132">Relationships</span></span>
<span data-ttu-id="d2ceb-133">Нет</span><span class="sxs-lookup"><span data-stu-id="d2ceb-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2ceb-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2ceb-134">JSON Representation</span></span>
<span data-ttu-id="d2ceb-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2ceb-135">Here is a JSON representation of the resource.</span></span>
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





