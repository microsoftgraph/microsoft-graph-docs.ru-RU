---
title: тип ресурса windowsKioskWin32App
description: KioskModeApp v4 для поддержки приложений Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7b0dd1a5afb5dcad27bd0b2656f29336be3332d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446717"
---
# <a name="windowskioskwin32app-resource-type"></a><span data-ttu-id="82beb-103">тип ресурса windowsKioskWin32App</span><span class="sxs-lookup"><span data-stu-id="82beb-103">windowsKioskWin32App resource type</span></span>

<span data-ttu-id="82beb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82beb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82beb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82beb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82beb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82beb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82beb-107">KioskModeApp v4 для поддержки приложений Win32</span><span class="sxs-lookup"><span data-stu-id="82beb-107">KioskModeApp v4 for Win32 app support</span></span>


<span data-ttu-id="82beb-108">Наследуется [от windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="82beb-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82beb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="82beb-109">Properties</span></span>
|<span data-ttu-id="82beb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="82beb-110">Property</span></span>|<span data-ttu-id="82beb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="82beb-111">Type</span></span>|<span data-ttu-id="82beb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="82beb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82beb-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="82beb-113">startLayoutTileSize</span></span>|[<span data-ttu-id="82beb-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="82beb-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="82beb-115">Размер плитки приложения для макета старта, унаследованный от [windowsKioskAppBase.](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="82beb-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="82beb-116">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="82beb-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="82beb-117">name</span><span class="sxs-lookup"><span data-stu-id="82beb-117">name</span></span>|<span data-ttu-id="82beb-118">String</span><span class="sxs-lookup"><span data-stu-id="82beb-118">String</span></span>|<span data-ttu-id="82beb-119">Представляет удобное имя приложения, унаследованной от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="82beb-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="82beb-120">appType</span><span class="sxs-lookup"><span data-stu-id="82beb-120">appType</span></span>|[<span data-ttu-id="82beb-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="82beb-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="82beb-122">Тип приложения, унаследованный от [windowsKioskAppBase.](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="82beb-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="82beb-123">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="82beb-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="82beb-124">autoLaunch</span><span class="sxs-lookup"><span data-stu-id="82beb-124">autoLaunch</span></span>|<span data-ttu-id="82beb-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="82beb-125">Boolean</span></span>|<span data-ttu-id="82beb-126">Разрешить автоматическое запуск приложения в режиме киоска с несколькими приложениями, унаследованных от [windowsKioskAppBase.](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="82beb-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="82beb-127">classicAppPath</span><span class="sxs-lookup"><span data-stu-id="82beb-127">classicAppPath</span></span>|<span data-ttu-id="82beb-128">String</span><span class="sxs-lookup"><span data-stu-id="82beb-128">String</span></span>|<span data-ttu-id="82beb-129">Это классическийapppath, используемый приложением v4 Win32 в режиме киоска</span><span class="sxs-lookup"><span data-stu-id="82beb-129">This is the classicapppath to be used by v4 Win32 app while in Kiosk Mode</span></span>|
|<span data-ttu-id="82beb-130">edgeNoFirstRun</span><span class="sxs-lookup"><span data-stu-id="82beb-130">edgeNoFirstRun</span></span>|<span data-ttu-id="82beb-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="82beb-131">Boolean</span></span>|<span data-ttu-id="82beb-132">Edge first run flag for Edge kiosk mode</span><span class="sxs-lookup"><span data-stu-id="82beb-132">Edge first run flag for Edge kiosk mode</span></span>|
|<span data-ttu-id="82beb-133">edgeKioskIdleTimeoutMinutes</span><span class="sxs-lookup"><span data-stu-id="82beb-133">edgeKioskIdleTimeoutMinutes</span></span>|<span data-ttu-id="82beb-134">Int32</span><span class="sxs-lookup"><span data-stu-id="82beb-134">Int32</span></span>|<span data-ttu-id="82beb-135">Время ожидания в киоске Edge в минутах для режима киоска Edge.</span><span class="sxs-lookup"><span data-stu-id="82beb-135">Edge kiosk idle timeout in minutes for Edge kiosk mode.</span></span> <span data-ttu-id="82beb-136">Допустимые значения от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="82beb-136">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="82beb-137">edgeKioskType</span><span class="sxs-lookup"><span data-stu-id="82beb-137">edgeKioskType</span></span>|[<span data-ttu-id="82beb-138">windowsEdgeKioskType</span><span class="sxs-lookup"><span data-stu-id="82beb-138">windowsEdgeKioskType</span></span>](../resources/intune-deviceconfig-windowsedgekiosktype.md)|<span data-ttu-id="82beb-139">Тип edge-киоска для режима киоска Edge.</span><span class="sxs-lookup"><span data-stu-id="82beb-139">Edge kiosk type for Edge kiosk mode.</span></span> <span data-ttu-id="82beb-140">Возможные значения: `publicBrowsing`, `fullScreen`.</span><span class="sxs-lookup"><span data-stu-id="82beb-140">Possible values are: `publicBrowsing`, `fullScreen`.</span></span>|
|<span data-ttu-id="82beb-141">edgeKiosk</span><span class="sxs-lookup"><span data-stu-id="82beb-141">edgeKiosk</span></span>|<span data-ttu-id="82beb-142">String</span><span class="sxs-lookup"><span data-stu-id="82beb-142">String</span></span>|<span data-ttu-id="82beb-143">Edge kiosk (URL) для режима киоска Edge</span><span class="sxs-lookup"><span data-stu-id="82beb-143">Edge kiosk (url) for Edge kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="82beb-144">Связи</span><span class="sxs-lookup"><span data-stu-id="82beb-144">Relationships</span></span>
<span data-ttu-id="82beb-145">Нет</span><span class="sxs-lookup"><span data-stu-id="82beb-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82beb-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="82beb-146">JSON Representation</span></span>
<span data-ttu-id="82beb-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82beb-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskWin32App",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "classicAppPath": "String",
  "edgeNoFirstRun": true,
  "edgeKioskIdleTimeoutMinutes": 1024,
  "edgeKioskType": "String",
  "edgeKiosk": "String"
}
```




