---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типа приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4cccd1b5e7ec7ca16aeb76b87fc31d90e92e7dcd
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30572084"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="74b1d-103">Тип ресурса windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="74b1d-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="74b1d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74b1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74b1d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74b1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74b1d-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="74b1d-106">The base class for a type of apps</span></span>


<span data-ttu-id="74b1d-107">НаСледуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="74b1d-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="74b1d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="74b1d-108">Properties</span></span>
|<span data-ttu-id="74b1d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="74b1d-109">Property</span></span>|<span data-ttu-id="74b1d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="74b1d-110">Type</span></span>|<span data-ttu-id="74b1d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="74b1d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74b1d-112">Стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="74b1d-112">startLayoutTileSize</span></span>|[<span data-ttu-id="74b1d-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="74b1d-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="74b1d-114">Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="74b1d-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="74b1d-115">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="74b1d-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="74b1d-116">name</span><span class="sxs-lookup"><span data-stu-id="74b1d-116">name</span></span>|<span data-ttu-id="74b1d-117">String</span><span class="sxs-lookup"><span data-stu-id="74b1d-117">String</span></span>|<span data-ttu-id="74b1d-118">Представляет понятное имя приложения, наСледуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="74b1d-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="74b1d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="74b1d-119">appType</span></span>|[<span data-ttu-id="74b1d-120">Виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="74b1d-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="74b1d-121">Тип приложения, наСледуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="74b1d-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="74b1d-122">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="74b1d-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="74b1d-123">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="74b1d-123">autoLaunch</span></span>|<span data-ttu-id="74b1d-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="74b1d-124">Boolean</span></span>|<span data-ttu-id="74b1d-125">Разрешить автоматический запуск приложения в режиме киоска с несколькими приложениями, унаследованном от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="74b1d-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="74b1d-126">path</span><span class="sxs-lookup"><span data-stu-id="74b1d-126">path</span></span>|<span data-ttu-id="74b1d-127">String</span><span class="sxs-lookup"><span data-stu-id="74b1d-127">String</span></span>|<span data-ttu-id="74b1d-128">Определение пути к классическому приложению</span><span class="sxs-lookup"><span data-stu-id="74b1d-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="74b1d-129">Десктопаппликатионид</span><span class="sxs-lookup"><span data-stu-id="74b1d-129">desktopApplicationId</span></span>|<span data-ttu-id="74b1d-130">Строка</span><span class="sxs-lookup"><span data-stu-id="74b1d-130">String</span></span>|<span data-ttu-id="74b1d-131">Определение Десктопаппликатионид приложения</span><span class="sxs-lookup"><span data-stu-id="74b1d-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="74b1d-132">Десктопаппликатионлинкпас</span><span class="sxs-lookup"><span data-stu-id="74b1d-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="74b1d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="74b1d-133">String</span></span>|<span data-ttu-id="74b1d-134">Определение Десктопаппликатионлинкпас приложения</span><span class="sxs-lookup"><span data-stu-id="74b1d-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="74b1d-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="74b1d-135">Relationships</span></span>
<span data-ttu-id="74b1d-136">Нет</span><span class="sxs-lookup"><span data-stu-id="74b1d-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74b1d-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74b1d-137">JSON Representation</span></span>
<span data-ttu-id="74b1d-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74b1d-138">Here is a JSON representation of the resource.</span></span>
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




