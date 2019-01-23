---
title: Тип ресурса windowsKioskUWPApp
description: Базовый класс для типов приложений
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ba5367721890f02af3b348ad469b15024de4800
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392684"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="a1ba4-103">Тип ресурса windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="a1ba4-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="a1ba4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a1ba4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1ba4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1ba4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1ba4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1ba4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1ba4-107">Базовый класс для типов приложений</span><span class="sxs-lookup"><span data-stu-id="a1ba4-107">The base class for a type of apps</span></span>


<span data-ttu-id="a1ba4-108">Наследуется от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="a1ba4-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a1ba4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1ba4-109">Properties</span></span>
|<span data-ttu-id="a1ba4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1ba4-110">Property</span></span>|<span data-ttu-id="a1ba4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a1ba4-111">Type</span></span>|<span data-ttu-id="a1ba4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a1ba4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1ba4-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="a1ba4-113">startLayoutTileSize</span></span>|[<span data-ttu-id="a1ba4-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="a1ba4-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="a1ba4-115">Размер плитку приложение для макета Пуск унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="a1ba4-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="a1ba4-116">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="a1ba4-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="a1ba4-117">name</span><span class="sxs-lookup"><span data-stu-id="a1ba4-117">name</span></span>|<span data-ttu-id="a1ba4-118">String</span><span class="sxs-lookup"><span data-stu-id="a1ba4-118">String</span></span>|<span data-ttu-id="a1ba4-119">Представляет понятное имя приложения унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="a1ba4-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="a1ba4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a1ba4-120">appType</span></span>|[<span data-ttu-id="a1ba4-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="a1ba4-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="a1ba4-122">Тип приложения унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="a1ba4-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="a1ba4-123">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="a1ba4-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="a1ba4-124">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="a1ba4-124">appUserModelId</span></span>|<span data-ttu-id="a1ba4-125">String</span><span class="sxs-lookup"><span data-stu-id="a1ba4-125">String</span></span>|<span data-ttu-id="a1ba4-126">Это единственный идентификатор модели приложения пользователя (AUMID), чтобы оно было доступно для использования в полноэкранном режиме запуска</span><span class="sxs-lookup"><span data-stu-id="a1ba4-126">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="a1ba4-127">appId</span><span class="sxs-lookup"><span data-stu-id="a1ba4-127">appId</span></span>|<span data-ttu-id="a1ba4-128">String</span><span class="sxs-lookup"><span data-stu-id="a1ba4-128">String</span></span>|<span data-ttu-id="a1ba4-129">Это ссылается на Intune приложения, который будет целевой для те же назначения как базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="a1ba4-129">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="a1ba4-130">containedAppId</span><span class="sxs-lookup"><span data-stu-id="a1ba4-130">containedAppId</span></span>|<span data-ttu-id="a1ba4-131">String</span><span class="sxs-lookup"><span data-stu-id="a1ba4-131">String</span></span>|<span data-ttu-id="a1ba4-132">Это ссылается автономные приложения из приложения для Intune</span><span class="sxs-lookup"><span data-stu-id="a1ba4-132">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1ba4-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="a1ba4-133">Relationships</span></span>
<span data-ttu-id="a1ba4-134">Нет</span><span class="sxs-lookup"><span data-stu-id="a1ba4-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1ba4-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1ba4-135">JSON Representation</span></span>
<span data-ttu-id="a1ba4-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1ba4-136">Here is a JSON representation of the resource.</span></span>
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




