---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типа приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0487fa24ecd2d27817349b68063cf606a2401944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170478"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="5b7e7-103">Тип ресурса windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="5b7e7-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="5b7e7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b7e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b7e7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b7e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b7e7-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="5b7e7-106">The base class for a type of apps</span></span>


<span data-ttu-id="5b7e7-107">НаСледуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="5b7e7-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b7e7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b7e7-108">Properties</span></span>
|<span data-ttu-id="5b7e7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b7e7-109">Property</span></span>|<span data-ttu-id="5b7e7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5b7e7-110">Type</span></span>|<span data-ttu-id="5b7e7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5b7e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b7e7-112">Стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="5b7e7-112">startLayoutTileSize</span></span>|[<span data-ttu-id="5b7e7-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="5b7e7-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="5b7e7-114">Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="5b7e7-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="5b7e7-115">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="5b7e7-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="5b7e7-116">name</span><span class="sxs-lookup"><span data-stu-id="5b7e7-116">name</span></span>|<span data-ttu-id="5b7e7-117">String</span><span class="sxs-lookup"><span data-stu-id="5b7e7-117">String</span></span>|<span data-ttu-id="5b7e7-118">Представляет понятное имя приложения, наСледуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="5b7e7-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="5b7e7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5b7e7-119">appType</span></span>|[<span data-ttu-id="5b7e7-120">Виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="5b7e7-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="5b7e7-121">Тип приложения, наСледуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="5b7e7-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="5b7e7-122">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="5b7e7-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="5b7e7-123">path</span><span class="sxs-lookup"><span data-stu-id="5b7e7-123">path</span></span>|<span data-ttu-id="5b7e7-124">String</span><span class="sxs-lookup"><span data-stu-id="5b7e7-124">String</span></span>|<span data-ttu-id="5b7e7-125">Определение пути к классическому приложению</span><span class="sxs-lookup"><span data-stu-id="5b7e7-125">Define the path of a desktop app</span></span>|
|<span data-ttu-id="5b7e7-126">Десктопаппликатионид</span><span class="sxs-lookup"><span data-stu-id="5b7e7-126">desktopApplicationId</span></span>|<span data-ttu-id="5b7e7-127">String</span><span class="sxs-lookup"><span data-stu-id="5b7e7-127">String</span></span>|<span data-ttu-id="5b7e7-128">Определение Десктопаппликатионид приложения</span><span class="sxs-lookup"><span data-stu-id="5b7e7-128">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="5b7e7-129">Десктопаппликатионлинкпас</span><span class="sxs-lookup"><span data-stu-id="5b7e7-129">desktopApplicationLinkPath</span></span>|<span data-ttu-id="5b7e7-130">String</span><span class="sxs-lookup"><span data-stu-id="5b7e7-130">String</span></span>|<span data-ttu-id="5b7e7-131">Определение Десктопаппликатионлинкпас приложения</span><span class="sxs-lookup"><span data-stu-id="5b7e7-131">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b7e7-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="5b7e7-132">Relationships</span></span>
<span data-ttu-id="5b7e7-133">Нет</span><span class="sxs-lookup"><span data-stu-id="5b7e7-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b7e7-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b7e7-134">JSON Representation</span></span>
<span data-ttu-id="5b7e7-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b7e7-135">Here is a JSON representation of the resource.</span></span>
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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




