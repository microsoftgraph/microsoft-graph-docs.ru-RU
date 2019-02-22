---
title: Тип ресурса Виндовскиоскувпапп
description: Базовый класс для типа приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1dbaf8dfd7f2cd488de37378f934ca3f31daedd6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147329"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="3311c-103">Тип ресурса Виндовскиоскувпапп</span><span class="sxs-lookup"><span data-stu-id="3311c-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="3311c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3311c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3311c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3311c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3311c-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="3311c-106">The base class for a type of apps</span></span>


<span data-ttu-id="3311c-107">НаСледуется от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="3311c-107">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3311c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3311c-108">Properties</span></span>
|<span data-ttu-id="3311c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3311c-109">Property</span></span>|<span data-ttu-id="3311c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3311c-110">Type</span></span>|<span data-ttu-id="3311c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3311c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3311c-112">Стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="3311c-112">startLayoutTileSize</span></span>|[<span data-ttu-id="3311c-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="3311c-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="3311c-114">Размер плитки приложения для начального макета, унаследованного от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="3311c-114">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="3311c-115">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="3311c-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="3311c-116">name</span><span class="sxs-lookup"><span data-stu-id="3311c-116">name</span></span>|<span data-ttu-id="3311c-117">String</span><span class="sxs-lookup"><span data-stu-id="3311c-117">String</span></span>|<span data-ttu-id="3311c-118">Представляет понятное имя приложения, наСледуемого от [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="3311c-118">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="3311c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3311c-119">appType</span></span>|[<span data-ttu-id="3311c-120">Виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="3311c-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="3311c-121">Тип приложения, наСледуемого из [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="3311c-121">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="3311c-122">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="3311c-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="3311c-123">Модели</span><span class="sxs-lookup"><span data-stu-id="3311c-123">appUserModelId</span></span>|<span data-ttu-id="3311c-124">String</span><span class="sxs-lookup"><span data-stu-id="3311c-124">String</span></span>|<span data-ttu-id="3311c-125">Это единственный идентификатор пользовательской модели приложения (AUMID), который будет доступен для запуска в режиме киоска</span><span class="sxs-lookup"><span data-stu-id="3311c-125">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="3311c-126">appId</span><span class="sxs-lookup"><span data-stu-id="3311c-126">appId</span></span>|<span data-ttu-id="3311c-127">String</span><span class="sxs-lookup"><span data-stu-id="3311c-127">String</span></span>|<span data-ttu-id="3311c-128">Это указывает на приложение Intune, которое будет нацелено на те же назначения, что и настройка киоска</span><span class="sxs-lookup"><span data-stu-id="3311c-128">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="3311c-129">Контаинедаппид</span><span class="sxs-lookup"><span data-stu-id="3311c-129">containedAppId</span></span>|<span data-ttu-id="3311c-130">String</span><span class="sxs-lookup"><span data-stu-id="3311c-130">String</span></span>|<span data-ttu-id="3311c-131">Это указывает на автономное приложение из приложения Intune</span><span class="sxs-lookup"><span data-stu-id="3311c-131">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="3311c-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="3311c-132">Relationships</span></span>
<span data-ttu-id="3311c-133">Нет</span><span class="sxs-lookup"><span data-stu-id="3311c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3311c-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3311c-134">JSON Representation</span></span>
<span data-ttu-id="3311c-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3311c-135">Here is a JSON representation of the resource.</span></span>
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
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




