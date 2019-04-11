---
title: Тип ресурса Мобилеаппинтентандстатедетаил
description: Цель мобильного приложения и состояние установки для данного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e39a8e869a688dc74ebcc18e4ef56fc16459013d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777979"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="c1992-103">Тип ресурса Мобилеаппинтентандстатедетаил</span><span class="sxs-lookup"><span data-stu-id="c1992-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="c1992-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1992-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1992-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1992-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1992-106">Цель мобильного приложения и состояние установки для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="c1992-106">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="c1992-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1992-107">Properties</span></span>
|<span data-ttu-id="c1992-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1992-108">Property</span></span>|<span data-ttu-id="c1992-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c1992-109">Type</span></span>|<span data-ttu-id="c1992-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c1992-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1992-111">applicationId</span><span class="sxs-lookup"><span data-stu-id="c1992-111">applicationId</span></span>|<span data-ttu-id="c1992-112">String</span><span class="sxs-lookup"><span data-stu-id="c1992-112">String</span></span>|<span data-ttu-id="c1992-113">Идентификатор Мобиеапп.</span><span class="sxs-lookup"><span data-stu-id="c1992-113">MobieApp identifier.</span></span>|
|<span data-ttu-id="c1992-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c1992-114">displayName</span></span>|<span data-ttu-id="c1992-115">String</span><span class="sxs-lookup"><span data-stu-id="c1992-115">String</span></span>|<span data-ttu-id="c1992-116">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c1992-116">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="c1992-117">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="c1992-117">mobileAppIntent</span></span>|[<span data-ttu-id="c1992-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="c1992-118">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="c1992-119">Цель для мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c1992-119">Mobile App Intent.</span></span> <span data-ttu-id="c1992-120">Возможные значения: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="c1992-120">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="c1992-121">Дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="c1992-121">displayVersion</span></span>|<span data-ttu-id="c1992-122">String</span><span class="sxs-lookup"><span data-stu-id="c1992-122">String</span></span>|<span data-ttu-id="c1992-123">Доступная для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="c1992-123">Human readable version of the application</span></span>|
|<span data-ttu-id="c1992-124">installState</span><span class="sxs-lookup"><span data-stu-id="c1992-124">installState</span></span>|[<span data-ttu-id="c1992-125">Ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="c1992-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="c1992-126">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="c1992-126">The install state of the app.</span></span> <span data-ttu-id="c1992-127">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="c1992-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="c1992-128">Суппортеддевицетипес</span><span class="sxs-lookup"><span data-stu-id="c1992-128">supportedDeviceTypes</span></span>|<span data-ttu-id="c1992-129">Коллекция [мобилеаппсуппортеддевицетипе](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="c1992-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="c1992-130">Поддерживаемые платформы для приложения.</span><span class="sxs-lookup"><span data-stu-id="c1992-130">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1992-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="c1992-131">Relationships</span></span>
<span data-ttu-id="c1992-132">Нет</span><span class="sxs-lookup"><span data-stu-id="c1992-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1992-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1992-133">JSON Representation</span></span>
<span data-ttu-id="c1992-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1992-134">Here is a JSON representation of the resource.</span></span>
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



