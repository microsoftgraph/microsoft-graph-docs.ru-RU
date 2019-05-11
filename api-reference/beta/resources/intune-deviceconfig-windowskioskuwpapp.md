---
title: Тип ресурса Виндовскиоскувпапп
description: Базовый класс для типа приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9340006ee74e640e21dc6bef99cc1f0e297999b9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943776"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="8be7d-103">Тип ресурса Виндовскиоскувпапп</span><span class="sxs-lookup"><span data-stu-id="8be7d-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="8be7d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8be7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8be7d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8be7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8be7d-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="8be7d-106">The base class for a type of apps</span></span>


<span data-ttu-id="8be7d-107">Наследуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="8be7d-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8be7d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8be7d-108">Properties</span></span>
|<span data-ttu-id="8be7d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8be7d-109">Property</span></span>|<span data-ttu-id="8be7d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8be7d-110">Type</span></span>|<span data-ttu-id="8be7d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8be7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8be7d-112">Стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="8be7d-112">startLayoutTileSize</span></span>|[<span data-ttu-id="8be7d-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="8be7d-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="8be7d-114">Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="8be7d-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="8be7d-115">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="8be7d-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="8be7d-116">name</span><span class="sxs-lookup"><span data-stu-id="8be7d-116">name</span></span>|<span data-ttu-id="8be7d-117">String</span><span class="sxs-lookup"><span data-stu-id="8be7d-117">String</span></span>|<span data-ttu-id="8be7d-118">Представляет понятное имя приложения, наследуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="8be7d-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="8be7d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8be7d-119">appType</span></span>|[<span data-ttu-id="8be7d-120">Виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="8be7d-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="8be7d-121">Тип приложения, наследуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="8be7d-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="8be7d-122">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="8be7d-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="8be7d-123">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="8be7d-123">autoLaunch</span></span>|<span data-ttu-id="8be7d-124">Логический</span><span class="sxs-lookup"><span data-stu-id="8be7d-124">Boolean</span></span>|<span data-ttu-id="8be7d-125">Разрешить автоматический запуск приложения в режиме киоска с несколькими приложениями, унаследованном от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="8be7d-125">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="8be7d-126">Модели</span><span class="sxs-lookup"><span data-stu-id="8be7d-126">appUserModelId</span></span>|<span data-ttu-id="8be7d-127">Строка</span><span class="sxs-lookup"><span data-stu-id="8be7d-127">String</span></span>|<span data-ttu-id="8be7d-128">Это единственный идентификатор пользовательской модели приложения (AUMID), который будет доступен для запуска в режиме киоска</span><span class="sxs-lookup"><span data-stu-id="8be7d-128">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="8be7d-129">appId</span><span class="sxs-lookup"><span data-stu-id="8be7d-129">appId</span></span>|<span data-ttu-id="8be7d-130">String</span><span class="sxs-lookup"><span data-stu-id="8be7d-130">String</span></span>|<span data-ttu-id="8be7d-131">Это указывает на приложение Intune, которое будет нацелено на те же назначения, что и настройка киоска</span><span class="sxs-lookup"><span data-stu-id="8be7d-131">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="8be7d-132">Контаинедаппид</span><span class="sxs-lookup"><span data-stu-id="8be7d-132">containedAppId</span></span>|<span data-ttu-id="8be7d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8be7d-133">String</span></span>|<span data-ttu-id="8be7d-134">Это указывает на автономное приложение из приложения Intune</span><span class="sxs-lookup"><span data-stu-id="8be7d-134">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="8be7d-135">Связи</span><span class="sxs-lookup"><span data-stu-id="8be7d-135">Relationships</span></span>
<span data-ttu-id="8be7d-136">Нет</span><span class="sxs-lookup"><span data-stu-id="8be7d-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8be7d-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8be7d-137">JSON Representation</span></span>
<span data-ttu-id="8be7d-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8be7d-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




