---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типа приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 82773d7bedc5bb4221327217195e98e12621dfde
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729541"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="7afbf-103">Тип ресурса windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="7afbf-103">windowsKioskDesktopApp resource type</span></span>

<span data-ttu-id="7afbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7afbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7afbf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7afbf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7afbf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7afbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7afbf-107">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="7afbf-107">The base class for a type of apps</span></span>


<span data-ttu-id="7afbf-108">Наследуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="7afbf-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7afbf-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7afbf-109">Properties</span></span>
|<span data-ttu-id="7afbf-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7afbf-110">Property</span></span>|<span data-ttu-id="7afbf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7afbf-111">Type</span></span>|<span data-ttu-id="7afbf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7afbf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7afbf-113">стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="7afbf-113">startLayoutTileSize</span></span>|[<span data-ttu-id="7afbf-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="7afbf-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="7afbf-115">Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="7afbf-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="7afbf-116">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="7afbf-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="7afbf-117">name</span><span class="sxs-lookup"><span data-stu-id="7afbf-117">name</span></span>|<span data-ttu-id="7afbf-118">String</span><span class="sxs-lookup"><span data-stu-id="7afbf-118">String</span></span>|<span data-ttu-id="7afbf-119">Представляет понятное имя приложения, наследуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="7afbf-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="7afbf-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7afbf-120">appType</span></span>|[<span data-ttu-id="7afbf-121">виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="7afbf-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="7afbf-122">Тип приложения, наследуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="7afbf-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="7afbf-123">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="7afbf-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="7afbf-124">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="7afbf-124">autoLaunch</span></span>|<span data-ttu-id="7afbf-125">Логический</span><span class="sxs-lookup"><span data-stu-id="7afbf-125">Boolean</span></span>|<span data-ttu-id="7afbf-126">Разрешить автоматический запуск приложения в режиме киоска с несколькими приложениями, унаследованном от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="7afbf-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="7afbf-127">path</span><span class="sxs-lookup"><span data-stu-id="7afbf-127">path</span></span>|<span data-ttu-id="7afbf-128">String</span><span class="sxs-lookup"><span data-stu-id="7afbf-128">String</span></span>|<span data-ttu-id="7afbf-129">Определение пути к классическому приложению</span><span class="sxs-lookup"><span data-stu-id="7afbf-129">Define the path of a desktop app</span></span>|
|<span data-ttu-id="7afbf-130">десктопаппликатионид</span><span class="sxs-lookup"><span data-stu-id="7afbf-130">desktopApplicationId</span></span>|<span data-ttu-id="7afbf-131">Строка</span><span class="sxs-lookup"><span data-stu-id="7afbf-131">String</span></span>|<span data-ttu-id="7afbf-132">Определение Десктопаппликатионид приложения</span><span class="sxs-lookup"><span data-stu-id="7afbf-132">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="7afbf-133">десктопаппликатионлинкпас</span><span class="sxs-lookup"><span data-stu-id="7afbf-133">desktopApplicationLinkPath</span></span>|<span data-ttu-id="7afbf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7afbf-134">String</span></span>|<span data-ttu-id="7afbf-135">Определение Десктопаппликатионлинкпас приложения</span><span class="sxs-lookup"><span data-stu-id="7afbf-135">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="7afbf-136">Связи</span><span class="sxs-lookup"><span data-stu-id="7afbf-136">Relationships</span></span>
<span data-ttu-id="7afbf-137">Нет</span><span class="sxs-lookup"><span data-stu-id="7afbf-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7afbf-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7afbf-138">JSON Representation</span></span>
<span data-ttu-id="7afbf-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7afbf-139">Here is a JSON representation of the resource.</span></span>
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





