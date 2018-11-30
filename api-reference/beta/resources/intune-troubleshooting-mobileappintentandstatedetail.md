---
title: Тип ресурса mobileAppIntentAndStateDetail
description: Цель мобильные приложения и состояние установки для данного устройства.
ms.openlocfilehash: d793f23346991c681ecfd4e0d55272153496ae36
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074628"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="0a8f6-103">Тип ресурса mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="0a8f6-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="0a8f6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a8f6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a8f6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a8f6-107">Цель мобильные приложения и состояние установки для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-107">Mobile App Intent and Install State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="0a8f6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a8f6-108">Properties</span></span>
|<span data-ttu-id="0a8f6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a8f6-109">Property</span></span>|<span data-ttu-id="0a8f6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0a8f6-110">Type</span></span>|<span data-ttu-id="0a8f6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a8f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a8f6-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="0a8f6-112">applicationId</span></span>|<span data-ttu-id="0a8f6-113">String</span><span class="sxs-lookup"><span data-stu-id="0a8f6-113">String</span></span>|<span data-ttu-id="0a8f6-114">Идентификатор MobieApp.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="0a8f6-115">displayName</span><span class="sxs-lookup"><span data-stu-id="0a8f6-115">displayName</span></span>|<span data-ttu-id="0a8f6-116">String</span><span class="sxs-lookup"><span data-stu-id="0a8f6-116">String</span></span>|<span data-ttu-id="0a8f6-117">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="0a8f6-118">mobileAppIntent;</span><span class="sxs-lookup"><span data-stu-id="0a8f6-118">mobileAppIntent</span></span>|<span data-ttu-id="0a8f6-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md);</span><span class="sxs-lookup"><span data-stu-id="0a8f6-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)</span></span>|<span data-ttu-id="0a8f6-120">Цель мобильных приложений.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-120">Mobile App Intent.</span></span> <span data-ttu-id="0a8f6-121">Возможные значения: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="0a8f6-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="0a8f6-122">displayVersion</span></span>|<span data-ttu-id="0a8f6-123">String</span><span class="sxs-lookup"><span data-stu-id="0a8f6-123">String</span></span>|<span data-ttu-id="0a8f6-124">Человеческого для чтения версию приложения</span><span class="sxs-lookup"><span data-stu-id="0a8f6-124">Human readable version of the application</span></span>|
|<span data-ttu-id="0a8f6-125">installState</span><span class="sxs-lookup"><span data-stu-id="0a8f6-125">installState</span></span>|[<span data-ttu-id="0a8f6-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="0a8f6-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="0a8f6-127">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-127">The install state of the app.</span></span> <span data-ttu-id="0a8f6-128">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="0a8f6-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="0a8f6-129">supportedDeviceTypes</span></span>|<span data-ttu-id="0a8f6-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0a8f6-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="0a8f6-131">Поддерживаемые платформы для приложения.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a8f6-132">Связи</span><span class="sxs-lookup"><span data-stu-id="0a8f6-132">Relationships</span></span>
<span data-ttu-id="0a8f6-133">Нет</span><span class="sxs-lookup"><span data-stu-id="0a8f6-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a8f6-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a8f6-134">JSON Representation</span></span>
<span data-ttu-id="0a8f6-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a8f6-135">Here is a JSON representation of the resource.</span></span>
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





