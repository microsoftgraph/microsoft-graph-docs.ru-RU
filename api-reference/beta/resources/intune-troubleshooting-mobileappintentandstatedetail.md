---
title: Тип ресурса mobileAppIntentAndStateDetail
description: Цель мобильные приложения и состояние установки для данного устройства.
author: tfitzmac
ms.openlocfilehash: 6a0a52d1cf8576778060c6f7b5e337e6e7a115e5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339223"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="47a6e-103">Тип ресурса mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="47a6e-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="47a6e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47a6e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47a6e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47a6e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47a6e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47a6e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47a6e-107">Цель мобильные приложения и состояние установки для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="47a6e-107">Mobile App Intent and Install State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="47a6e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="47a6e-108">Properties</span></span>
|<span data-ttu-id="47a6e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="47a6e-109">Property</span></span>|<span data-ttu-id="47a6e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="47a6e-110">Type</span></span>|<span data-ttu-id="47a6e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="47a6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47a6e-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="47a6e-112">applicationId</span></span>|<span data-ttu-id="47a6e-113">String</span><span class="sxs-lookup"><span data-stu-id="47a6e-113">String</span></span>|<span data-ttu-id="47a6e-114">Идентификатор MobieApp.</span><span class="sxs-lookup"><span data-stu-id="47a6e-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="47a6e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="47a6e-115">displayName</span></span>|<span data-ttu-id="47a6e-116">String</span><span class="sxs-lookup"><span data-stu-id="47a6e-116">String</span></span>|<span data-ttu-id="47a6e-117">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="47a6e-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="47a6e-118">mobileAppIntent;</span><span class="sxs-lookup"><span data-stu-id="47a6e-118">mobileAppIntent</span></span>|<span data-ttu-id="47a6e-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md);</span><span class="sxs-lookup"><span data-stu-id="47a6e-119">[mobileAppIntent](../resources/intune-troubleshooting-mobileappintent.md)</span></span>|<span data-ttu-id="47a6e-120">Цель мобильных приложений.</span><span class="sxs-lookup"><span data-stu-id="47a6e-120">Mobile App Intent.</span></span> <span data-ttu-id="47a6e-121">Возможные значения: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="47a6e-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="47a6e-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="47a6e-122">displayVersion</span></span>|<span data-ttu-id="47a6e-123">String.</span><span class="sxs-lookup"><span data-stu-id="47a6e-123">String</span></span>|<span data-ttu-id="47a6e-124">Человеческого для чтения версию приложения</span><span class="sxs-lookup"><span data-stu-id="47a6e-124">Human readable version of the application</span></span>|
|<span data-ttu-id="47a6e-125">installState</span><span class="sxs-lookup"><span data-stu-id="47a6e-125">installState</span></span>|[<span data-ttu-id="47a6e-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="47a6e-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="47a6e-127">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="47a6e-127">The install state of the app.</span></span> <span data-ttu-id="47a6e-128">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="47a6e-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="47a6e-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="47a6e-129">supportedDeviceTypes</span></span>|<span data-ttu-id="47a6e-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="47a6e-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="47a6e-131">Поддерживаемые платформы для приложения.</span><span class="sxs-lookup"><span data-stu-id="47a6e-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47a6e-132">Связи</span><span class="sxs-lookup"><span data-stu-id="47a6e-132">Relationships</span></span>
<span data-ttu-id="47a6e-133">Нет</span><span class="sxs-lookup"><span data-stu-id="47a6e-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47a6e-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47a6e-134">JSON Representation</span></span>
<span data-ttu-id="47a6e-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47a6e-135">Here is a JSON representation of the resource.</span></span>
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





