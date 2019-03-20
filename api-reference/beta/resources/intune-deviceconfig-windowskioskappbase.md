---
title: Тип ресурса Виндовскиоскаппбасе
description: Базовый класс для типа приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b86921fcdaa11b37b985184dfbc645c2a193bfdb
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572308"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="cbe12-103">Тип ресурса Виндовскиоскаппбасе</span><span class="sxs-lookup"><span data-stu-id="cbe12-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="cbe12-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbe12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbe12-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cbe12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbe12-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="cbe12-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="cbe12-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbe12-107">Properties</span></span>
|<span data-ttu-id="cbe12-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbe12-108">Property</span></span>|<span data-ttu-id="cbe12-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cbe12-109">Type</span></span>|<span data-ttu-id="cbe12-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cbe12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbe12-111">Стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="cbe12-111">startLayoutTileSize</span></span>|[<span data-ttu-id="cbe12-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="cbe12-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="cbe12-113">Размер плитки приложения для начального макета.</span><span class="sxs-lookup"><span data-stu-id="cbe12-113">The app tile size for the start layout.</span></span> <span data-ttu-id="cbe12-114">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="cbe12-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="cbe12-115">name</span><span class="sxs-lookup"><span data-stu-id="cbe12-115">name</span></span>|<span data-ttu-id="cbe12-116">String</span><span class="sxs-lookup"><span data-stu-id="cbe12-116">String</span></span>|<span data-ttu-id="cbe12-117">Представляет понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="cbe12-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="cbe12-118">Тип</span><span class="sxs-lookup"><span data-stu-id="cbe12-118">appType</span></span>|[<span data-ttu-id="cbe12-119">Виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="cbe12-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="cbe12-120">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="cbe12-120">The app type.</span></span> <span data-ttu-id="cbe12-121">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="cbe12-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="cbe12-122">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="cbe12-122">autoLaunch</span></span>|<span data-ttu-id="cbe12-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbe12-123">Boolean</span></span>|<span data-ttu-id="cbe12-124">Разрешение автоматического запуска приложения в полноэкранном режиме с поддержкой нескольких приложений</span><span class="sxs-lookup"><span data-stu-id="cbe12-124">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbe12-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="cbe12-125">Relationships</span></span>
<span data-ttu-id="cbe12-126">Нет</span><span class="sxs-lookup"><span data-stu-id="cbe12-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbe12-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbe12-127">JSON Representation</span></span>
<span data-ttu-id="cbe12-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbe12-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```




