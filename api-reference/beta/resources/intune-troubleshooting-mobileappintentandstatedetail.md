---
title: Тип ресурса mobileAppIntentAndStateDetail
description: Цель мобильные приложения и состояние установки для данного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 169988d8a3a114bbae7a06583565c9abd3414b4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946688"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="e35fe-103">Тип ресурса mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="e35fe-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="e35fe-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e35fe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e35fe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e35fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e35fe-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e35fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e35fe-107">Цель мобильные приложения и состояние установки для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="e35fe-107">Mobile App Intent and Install State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="e35fe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e35fe-108">Properties</span></span>
|<span data-ttu-id="e35fe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e35fe-109">Property</span></span>|<span data-ttu-id="e35fe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e35fe-110">Type</span></span>|<span data-ttu-id="e35fe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e35fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e35fe-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="e35fe-112">applicationId</span></span>|<span data-ttu-id="e35fe-113">String</span><span class="sxs-lookup"><span data-stu-id="e35fe-113">String</span></span>|<span data-ttu-id="e35fe-114">Идентификатор MobieApp.</span><span class="sxs-lookup"><span data-stu-id="e35fe-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="e35fe-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e35fe-115">displayName</span></span>|<span data-ttu-id="e35fe-116">String</span><span class="sxs-lookup"><span data-stu-id="e35fe-116">String</span></span>|<span data-ttu-id="e35fe-117">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e35fe-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="e35fe-118">mobileAppIntent;</span><span class="sxs-lookup"><span data-stu-id="e35fe-118">mobileAppIntent</span></span>|<span data-ttu-id="e35fe-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md);</span><span class="sxs-lookup"><span data-stu-id="e35fe-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)</span></span>|<span data-ttu-id="e35fe-120">Цель мобильных приложений.</span><span class="sxs-lookup"><span data-stu-id="e35fe-120">Mobile App Intent.</span></span> <span data-ttu-id="e35fe-121">Возможные значения: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="e35fe-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="e35fe-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="e35fe-122">displayVersion</span></span>|<span data-ttu-id="e35fe-123">Строка</span><span class="sxs-lookup"><span data-stu-id="e35fe-123">String</span></span>|<span data-ttu-id="e35fe-124">Человеческого для чтения версию приложения</span><span class="sxs-lookup"><span data-stu-id="e35fe-124">Human readable version of the application</span></span>|
|<span data-ttu-id="e35fe-125">installState</span><span class="sxs-lookup"><span data-stu-id="e35fe-125">installState</span></span>|[<span data-ttu-id="e35fe-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e35fe-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e35fe-127">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="e35fe-127">The install state of the app.</span></span> <span data-ttu-id="e35fe-128">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e35fe-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e35fe-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="e35fe-129">supportedDeviceTypes</span></span>|<span data-ttu-id="e35fe-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e35fe-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="e35fe-131">Поддерживаемые платформы для приложения.</span><span class="sxs-lookup"><span data-stu-id="e35fe-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e35fe-132">Связи</span><span class="sxs-lookup"><span data-stu-id="e35fe-132">Relationships</span></span>
<span data-ttu-id="e35fe-133">Нет</span><span class="sxs-lookup"><span data-stu-id="e35fe-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e35fe-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e35fe-134">JSON Representation</span></span>
<span data-ttu-id="e35fe-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e35fe-135">Here is a JSON representation of the resource.</span></span>
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





