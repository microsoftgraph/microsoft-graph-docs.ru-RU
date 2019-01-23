---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типов приложений
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 831ed86da24791cde549687ecaff42cabc29a99e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415308"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="5d7ce-103">Тип ресурса windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="5d7ce-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="5d7ce-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5d7ce-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5d7ce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d7ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d7ce-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d7ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d7ce-107">Базовый класс для типов приложений</span><span class="sxs-lookup"><span data-stu-id="5d7ce-107">The base class for a type of apps</span></span>


<span data-ttu-id="5d7ce-108">Наследуется от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="5d7ce-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5d7ce-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d7ce-109">Properties</span></span>
|<span data-ttu-id="5d7ce-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d7ce-110">Property</span></span>|<span data-ttu-id="5d7ce-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5d7ce-111">Type</span></span>|<span data-ttu-id="5d7ce-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5d7ce-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d7ce-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="5d7ce-113">startLayoutTileSize</span></span>|[<span data-ttu-id="5d7ce-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="5d7ce-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="5d7ce-115">Размер плитку приложение для макета Пуск унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="5d7ce-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="5d7ce-116">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="5d7ce-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="5d7ce-117">name</span><span class="sxs-lookup"><span data-stu-id="5d7ce-117">name</span></span>|<span data-ttu-id="5d7ce-118">String</span><span class="sxs-lookup"><span data-stu-id="5d7ce-118">String</span></span>|<span data-ttu-id="5d7ce-119">Представляет понятное имя приложения унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="5d7ce-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="5d7ce-120">Тип</span><span class="sxs-lookup"><span data-stu-id="5d7ce-120">appType</span></span>|[<span data-ttu-id="5d7ce-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="5d7ce-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="5d7ce-122">Тип приложения унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="5d7ce-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="5d7ce-123">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="5d7ce-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="5d7ce-124">path</span><span class="sxs-lookup"><span data-stu-id="5d7ce-124">path</span></span>|<span data-ttu-id="5d7ce-125">String</span><span class="sxs-lookup"><span data-stu-id="5d7ce-125">String</span></span>|<span data-ttu-id="5d7ce-126">Определение пути классического приложения</span><span class="sxs-lookup"><span data-stu-id="5d7ce-126">Define the path of a desktop app</span></span>|
|<span data-ttu-id="5d7ce-127">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="5d7ce-127">desktopApplicationId</span></span>|<span data-ttu-id="5d7ce-128">String</span><span class="sxs-lookup"><span data-stu-id="5d7ce-128">String</span></span>|<span data-ttu-id="5d7ce-129">Определение DesktopApplicationID приложения</span><span class="sxs-lookup"><span data-stu-id="5d7ce-129">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="5d7ce-130">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="5d7ce-130">desktopApplicationLinkPath</span></span>|<span data-ttu-id="5d7ce-131">String</span><span class="sxs-lookup"><span data-stu-id="5d7ce-131">String</span></span>|<span data-ttu-id="5d7ce-132">Определение DesktopApplicationLinkPath приложения</span><span class="sxs-lookup"><span data-stu-id="5d7ce-132">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d7ce-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="5d7ce-133">Relationships</span></span>
<span data-ttu-id="5d7ce-134">Нет</span><span class="sxs-lookup"><span data-stu-id="5d7ce-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d7ce-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d7ce-135">JSON Representation</span></span>
<span data-ttu-id="5d7ce-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d7ce-136">Here is a JSON representation of the resource.</span></span>
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




