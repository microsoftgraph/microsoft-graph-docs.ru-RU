---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типа приложений
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af8e97b8b1aac3fcee5592da78b96bc2ccfd5143
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463466"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="1dc2c-103">Тип ресурса windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="1dc2c-103">windowsKioskDesktopApp resource type</span></span>

<span data-ttu-id="1dc2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dc2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dc2c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dc2c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dc2c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1dc2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dc2c-107">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="1dc2c-107">The base class for a type of apps</span></span>


<span data-ttu-id="1dc2c-108">Наследуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="1dc2c-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1dc2c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1dc2c-109">Properties</span></span>
|<span data-ttu-id="1dc2c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1dc2c-110">Property</span></span>|<span data-ttu-id="1dc2c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1dc2c-111">Type</span></span>|<span data-ttu-id="1dc2c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1dc2c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dc2c-113">стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="1dc2c-113">startLayoutTileSize</span></span>|[<span data-ttu-id="1dc2c-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="1dc2c-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="1dc2c-115">Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="1dc2c-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="1dc2c-116">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="1dc2c-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="1dc2c-117">name</span><span class="sxs-lookup"><span data-stu-id="1dc2c-117">name</span></span>|<span data-ttu-id="1dc2c-118">String</span><span class="sxs-lookup"><span data-stu-id="1dc2c-118">String</span></span>|<span data-ttu-id="1dc2c-119">Представляет понятное имя приложения, наследуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="1dc2c-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="1dc2c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1dc2c-120">appType</span></span>|[<span data-ttu-id="1dc2c-121">виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="1dc2c-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="1dc2c-122">Тип приложения, наследуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="1dc2c-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="1dc2c-123">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="1dc2c-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="1dc2c-124">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="1dc2c-124">autoLaunch</span></span>|<span data-ttu-id="1dc2c-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dc2c-125">Boolean</span></span>|<span data-ttu-id="1dc2c-126">Разрешить автоматический запуск приложения в режиме киоска с несколькими приложениями, унаследованном от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="1dc2c-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="1dc2c-127">path</span><span class="sxs-lookup"><span data-stu-id="1dc2c-127">path</span></span>|<span data-ttu-id="1dc2c-128">String</span><span class="sxs-lookup"><span data-stu-id="1dc2c-128">String</span></span>|<span data-ttu-id="1dc2c-129">Определение пути к классическому приложению</span><span class="sxs-lookup"><span data-stu-id="1dc2c-129">Define the path of a desktop app</span></span>|
|<span data-ttu-id="1dc2c-130">десктопаппликатионид</span><span class="sxs-lookup"><span data-stu-id="1dc2c-130">desktopApplicationId</span></span>|<span data-ttu-id="1dc2c-131">String</span><span class="sxs-lookup"><span data-stu-id="1dc2c-131">String</span></span>|<span data-ttu-id="1dc2c-132">Определение Десктопаппликатионид приложения</span><span class="sxs-lookup"><span data-stu-id="1dc2c-132">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="1dc2c-133">десктопаппликатионлинкпас</span><span class="sxs-lookup"><span data-stu-id="1dc2c-133">desktopApplicationLinkPath</span></span>|<span data-ttu-id="1dc2c-134">String</span><span class="sxs-lookup"><span data-stu-id="1dc2c-134">String</span></span>|<span data-ttu-id="1dc2c-135">Определение Десктопаппликатионлинкпас приложения</span><span class="sxs-lookup"><span data-stu-id="1dc2c-135">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dc2c-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="1dc2c-136">Relationships</span></span>
<span data-ttu-id="1dc2c-137">Нет</span><span class="sxs-lookup"><span data-stu-id="1dc2c-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dc2c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1dc2c-138">JSON Representation</span></span>
<span data-ttu-id="1dc2c-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1dc2c-139">Here is a JSON representation of the resource.</span></span>
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



