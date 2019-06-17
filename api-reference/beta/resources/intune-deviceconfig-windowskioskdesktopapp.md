---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типа приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5c3381637cb0bc24224f632b0c08e22e28a68af
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978495"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="adcef-103">Тип ресурса windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="adcef-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="adcef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adcef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adcef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="adcef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adcef-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="adcef-106">The base class for a type of apps</span></span>


<span data-ttu-id="adcef-107">Наследуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="adcef-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="adcef-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="adcef-108">Properties</span></span>
|<span data-ttu-id="adcef-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="adcef-109">Property</span></span>|<span data-ttu-id="adcef-110">Тип</span><span class="sxs-lookup"><span data-stu-id="adcef-110">Type</span></span>|<span data-ttu-id="adcef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="adcef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adcef-112">Стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="adcef-112">startLayoutTileSize</span></span>|[<span data-ttu-id="adcef-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="adcef-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="adcef-114">Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="adcef-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="adcef-115">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="adcef-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="adcef-116">name</span><span class="sxs-lookup"><span data-stu-id="adcef-116">name</span></span>|<span data-ttu-id="adcef-117">String</span><span class="sxs-lookup"><span data-stu-id="adcef-117">String</span></span>|<span data-ttu-id="adcef-118">Представляет понятное имя приложения, наследуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="adcef-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="adcef-119">Тип</span><span class="sxs-lookup"><span data-stu-id="adcef-119">appType</span></span>|[<span data-ttu-id="adcef-120">Виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="adcef-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="adcef-121">Тип приложения, наследуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="adcef-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="adcef-122">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="adcef-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="adcef-123">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="adcef-123">autoLaunch</span></span>|<span data-ttu-id="adcef-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="adcef-124">Boolean</span></span>|<span data-ttu-id="adcef-125">Разрешить автоматический запуск приложения в режиме киоска с несколькими приложениями, унаследованном от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="adcef-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="adcef-126">path</span><span class="sxs-lookup"><span data-stu-id="adcef-126">path</span></span>|<span data-ttu-id="adcef-127">String</span><span class="sxs-lookup"><span data-stu-id="adcef-127">String</span></span>|<span data-ttu-id="adcef-128">Определение пути к классическому приложению</span><span class="sxs-lookup"><span data-stu-id="adcef-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="adcef-129">Десктопаппликатионид</span><span class="sxs-lookup"><span data-stu-id="adcef-129">desktopApplicationId</span></span>|<span data-ttu-id="adcef-130">String</span><span class="sxs-lookup"><span data-stu-id="adcef-130">String</span></span>|<span data-ttu-id="adcef-131">Определение Десктопаппликатионид приложения</span><span class="sxs-lookup"><span data-stu-id="adcef-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="adcef-132">Десктопаппликатионлинкпас</span><span class="sxs-lookup"><span data-stu-id="adcef-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="adcef-133">String</span><span class="sxs-lookup"><span data-stu-id="adcef-133">String</span></span>|<span data-ttu-id="adcef-134">Определение Десктопаппликатионлинкпас приложения</span><span class="sxs-lookup"><span data-stu-id="adcef-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="adcef-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="adcef-135">Relationships</span></span>
<span data-ttu-id="adcef-136">Нет</span><span class="sxs-lookup"><span data-stu-id="adcef-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="adcef-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="adcef-137">JSON Representation</span></span>
<span data-ttu-id="adcef-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adcef-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





