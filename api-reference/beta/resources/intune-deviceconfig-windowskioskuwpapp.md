---
title: Тип ресурса Виндовскиоскувпапп
description: Базовый класс для типа приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 840332c2873f1a42adc5a6f1ef501f411842aa32
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529021"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="8812f-103">Тип ресурса Виндовскиоскувпапп</span><span class="sxs-lookup"><span data-stu-id="8812f-103">windowsKioskUWPApp resource type</span></span>

<span data-ttu-id="8812f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8812f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8812f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8812f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8812f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8812f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8812f-107">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="8812f-107">The base class for a type of apps</span></span>


<span data-ttu-id="8812f-108">Наследуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="8812f-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8812f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8812f-109">Properties</span></span>
|<span data-ttu-id="8812f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8812f-110">Property</span></span>|<span data-ttu-id="8812f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8812f-111">Type</span></span>|<span data-ttu-id="8812f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8812f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8812f-113">стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="8812f-113">startLayoutTileSize</span></span>|[<span data-ttu-id="8812f-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="8812f-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="8812f-115">Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="8812f-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="8812f-116">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="8812f-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="8812f-117">name</span><span class="sxs-lookup"><span data-stu-id="8812f-117">name</span></span>|<span data-ttu-id="8812f-118">String</span><span class="sxs-lookup"><span data-stu-id="8812f-118">String</span></span>|<span data-ttu-id="8812f-119">Представляет понятное имя приложения, наследуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="8812f-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="8812f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8812f-120">appType</span></span>|[<span data-ttu-id="8812f-121">виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="8812f-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="8812f-122">Тип приложения, наследуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="8812f-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="8812f-123">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="8812f-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="8812f-124">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="8812f-124">autoLaunch</span></span>|<span data-ttu-id="8812f-125">Логический</span><span class="sxs-lookup"><span data-stu-id="8812f-125">Boolean</span></span>|<span data-ttu-id="8812f-126">Разрешить автоматический запуск приложения в режиме киоска с несколькими приложениями, унаследованном от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="8812f-126">Allow the app to be auto-launched in multi-app kiosk mode Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="8812f-127">Модели</span><span class="sxs-lookup"><span data-stu-id="8812f-127">appUserModelId</span></span>|<span data-ttu-id="8812f-128">String</span><span class="sxs-lookup"><span data-stu-id="8812f-128">String</span></span>|<span data-ttu-id="8812f-129">Это единственный идентификатор пользовательской модели приложения (AUMID), который будет доступен для запуска в режиме киоска</span><span class="sxs-lookup"><span data-stu-id="8812f-129">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="8812f-130">appId</span><span class="sxs-lookup"><span data-stu-id="8812f-130">appId</span></span>|<span data-ttu-id="8812f-131">String</span><span class="sxs-lookup"><span data-stu-id="8812f-131">String</span></span>|<span data-ttu-id="8812f-132">Это указывает на приложение Intune, которое будет нацелено на те же назначения, что и настройка киоска</span><span class="sxs-lookup"><span data-stu-id="8812f-132">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="8812f-133">контаинедаппид</span><span class="sxs-lookup"><span data-stu-id="8812f-133">containedAppId</span></span>|<span data-ttu-id="8812f-134">String</span><span class="sxs-lookup"><span data-stu-id="8812f-134">String</span></span>|<span data-ttu-id="8812f-135">Это указывает на автономное приложение из приложения Intune</span><span class="sxs-lookup"><span data-stu-id="8812f-135">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="8812f-136">Связи</span><span class="sxs-lookup"><span data-stu-id="8812f-136">Relationships</span></span>
<span data-ttu-id="8812f-137">Нет</span><span class="sxs-lookup"><span data-stu-id="8812f-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8812f-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8812f-138">JSON Representation</span></span>
<span data-ttu-id="8812f-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8812f-139">Here is a JSON representation of the resource.</span></span>
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



