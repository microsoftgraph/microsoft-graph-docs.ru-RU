---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типа приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60b930ece0d938527666b2f00e84791aacdc3e59
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370909"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="c3949-103">Тип ресурса windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="c3949-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="c3949-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3949-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3949-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3949-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3949-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="c3949-106">The base class for a type of apps</span></span>


<span data-ttu-id="c3949-107">Наследуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="c3949-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3949-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3949-108">Properties</span></span>
|<span data-ttu-id="c3949-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3949-109">Property</span></span>|<span data-ttu-id="c3949-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c3949-110">Type</span></span>|<span data-ttu-id="c3949-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3949-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3949-112">стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="c3949-112">startLayoutTileSize</span></span>|[<span data-ttu-id="c3949-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="c3949-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="c3949-114">Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="c3949-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="c3949-115">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="c3949-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="c3949-116">name</span><span class="sxs-lookup"><span data-stu-id="c3949-116">name</span></span>|<span data-ttu-id="c3949-117">String</span><span class="sxs-lookup"><span data-stu-id="c3949-117">String</span></span>|<span data-ttu-id="c3949-118">Представляет понятное имя приложения, наследуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="c3949-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="c3949-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c3949-119">appType</span></span>|[<span data-ttu-id="c3949-120">виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="c3949-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="c3949-121">Тип приложения, наследуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="c3949-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="c3949-122">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="c3949-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="c3949-123">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="c3949-123">autoLaunch</span></span>|<span data-ttu-id="c3949-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3949-124">Boolean</span></span>|<span data-ttu-id="c3949-125">Разрешить автоматический запуск приложения в режиме киоска с несколькими приложениями, унаследованном от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="c3949-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="c3949-126">path</span><span class="sxs-lookup"><span data-stu-id="c3949-126">path</span></span>|<span data-ttu-id="c3949-127">String</span><span class="sxs-lookup"><span data-stu-id="c3949-127">String</span></span>|<span data-ttu-id="c3949-128">Определение пути к классическому приложению</span><span class="sxs-lookup"><span data-stu-id="c3949-128">Define the path of a desktop app</span></span>|
|<span data-ttu-id="c3949-129">десктопаппликатионид</span><span class="sxs-lookup"><span data-stu-id="c3949-129">desktopApplicationId</span></span>|<span data-ttu-id="c3949-130">String</span><span class="sxs-lookup"><span data-stu-id="c3949-130">String</span></span>|<span data-ttu-id="c3949-131">Определение Десктопаппликатионид приложения</span><span class="sxs-lookup"><span data-stu-id="c3949-131">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="c3949-132">десктопаппликатионлинкпас</span><span class="sxs-lookup"><span data-stu-id="c3949-132">desktopApplicationLinkPath</span></span>|<span data-ttu-id="c3949-133">String</span><span class="sxs-lookup"><span data-stu-id="c3949-133">String</span></span>|<span data-ttu-id="c3949-134">Определение Десктопаппликатионлинкпас приложения</span><span class="sxs-lookup"><span data-stu-id="c3949-134">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3949-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="c3949-135">Relationships</span></span>
<span data-ttu-id="c3949-136">Нет</span><span class="sxs-lookup"><span data-stu-id="c3949-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3949-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3949-137">JSON Representation</span></span>
<span data-ttu-id="c3949-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3949-138">Here is a JSON representation of the resource.</span></span>
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



