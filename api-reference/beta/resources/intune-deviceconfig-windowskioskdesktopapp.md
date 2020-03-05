---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типа приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7df38deba11cae5199a781a38dda6cd4b5abb698
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529030"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="50a5d-103">Тип ресурса windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="50a5d-103">windowsKioskDesktopApp resource type</span></span>

<span data-ttu-id="50a5d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="50a5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50a5d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50a5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50a5d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50a5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50a5d-107">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="50a5d-107">The base class for a type of apps</span></span>


<span data-ttu-id="50a5d-108">Наследуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="50a5d-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="50a5d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="50a5d-109">Properties</span></span>
|<span data-ttu-id="50a5d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="50a5d-110">Property</span></span>|<span data-ttu-id="50a5d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="50a5d-111">Type</span></span>|<span data-ttu-id="50a5d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="50a5d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50a5d-113">стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="50a5d-113">startLayoutTileSize</span></span>|[<span data-ttu-id="50a5d-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="50a5d-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="50a5d-115">Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="50a5d-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="50a5d-116">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="50a5d-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="50a5d-117">name</span><span class="sxs-lookup"><span data-stu-id="50a5d-117">name</span></span>|<span data-ttu-id="50a5d-118">String</span><span class="sxs-lookup"><span data-stu-id="50a5d-118">String</span></span>|<span data-ttu-id="50a5d-119">Представляет понятное имя приложения, наследуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="50a5d-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="50a5d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="50a5d-120">appType</span></span>|[<span data-ttu-id="50a5d-121">виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="50a5d-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="50a5d-122">Тип приложения, наследуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="50a5d-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="50a5d-123">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="50a5d-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="50a5d-124">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="50a5d-124">autoLaunch</span></span>|<span data-ttu-id="50a5d-125">Логический</span><span class="sxs-lookup"><span data-stu-id="50a5d-125">Boolean</span></span>|<span data-ttu-id="50a5d-126">Разрешить автоматический запуск приложения в режиме киоска с несколькими приложениями, унаследованном от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="50a5d-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="50a5d-127">path</span><span class="sxs-lookup"><span data-stu-id="50a5d-127">path</span></span>|<span data-ttu-id="50a5d-128">String</span><span class="sxs-lookup"><span data-stu-id="50a5d-128">String</span></span>|<span data-ttu-id="50a5d-129">Определение пути к классическому приложению</span><span class="sxs-lookup"><span data-stu-id="50a5d-129">Define the path of a desktop app</span></span>|
|<span data-ttu-id="50a5d-130">десктопаппликатионид</span><span class="sxs-lookup"><span data-stu-id="50a5d-130">desktopApplicationId</span></span>|<span data-ttu-id="50a5d-131">String</span><span class="sxs-lookup"><span data-stu-id="50a5d-131">String</span></span>|<span data-ttu-id="50a5d-132">Определение Десктопаппликатионид приложения</span><span class="sxs-lookup"><span data-stu-id="50a5d-132">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="50a5d-133">десктопаппликатионлинкпас</span><span class="sxs-lookup"><span data-stu-id="50a5d-133">desktopApplicationLinkPath</span></span>|<span data-ttu-id="50a5d-134">String</span><span class="sxs-lookup"><span data-stu-id="50a5d-134">String</span></span>|<span data-ttu-id="50a5d-135">Определение Десктопаппликатионлинкпас приложения</span><span class="sxs-lookup"><span data-stu-id="50a5d-135">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="50a5d-136">Связи</span><span class="sxs-lookup"><span data-stu-id="50a5d-136">Relationships</span></span>
<span data-ttu-id="50a5d-137">Нет</span><span class="sxs-lookup"><span data-stu-id="50a5d-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50a5d-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50a5d-138">JSON Representation</span></span>
<span data-ttu-id="50a5d-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50a5d-139">Here is a JSON representation of the resource.</span></span>
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



