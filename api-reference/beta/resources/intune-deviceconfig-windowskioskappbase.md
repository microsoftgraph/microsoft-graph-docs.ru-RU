---
title: Тип ресурса Виндовскиоскаппбасе
description: Базовый класс для типа приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93884a53ce20f67fadbd60fa2a8f180aba8fa826
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944091"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="7b0d9-103">Тип ресурса Виндовскиоскаппбасе</span><span class="sxs-lookup"><span data-stu-id="7b0d9-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="7b0d9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b0d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b0d9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b0d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b0d9-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="7b0d9-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="7b0d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b0d9-107">Properties</span></span>
|<span data-ttu-id="7b0d9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b0d9-108">Property</span></span>|<span data-ttu-id="7b0d9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7b0d9-109">Type</span></span>|<span data-ttu-id="7b0d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b0d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b0d9-111">Стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="7b0d9-111">startLayoutTileSize</span></span>|[<span data-ttu-id="7b0d9-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="7b0d9-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="7b0d9-113">Размер плитки приложения для начального макета.</span><span class="sxs-lookup"><span data-stu-id="7b0d9-113">The app tile size for the start layout.</span></span> <span data-ttu-id="7b0d9-114">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="7b0d9-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="7b0d9-115">name</span><span class="sxs-lookup"><span data-stu-id="7b0d9-115">name</span></span>|<span data-ttu-id="7b0d9-116">String</span><span class="sxs-lookup"><span data-stu-id="7b0d9-116">String</span></span>|<span data-ttu-id="7b0d9-117">Представляет понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="7b0d9-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="7b0d9-118">Тип</span><span class="sxs-lookup"><span data-stu-id="7b0d9-118">appType</span></span>|[<span data-ttu-id="7b0d9-119">Виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="7b0d9-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="7b0d9-120">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="7b0d9-120">The app type.</span></span> <span data-ttu-id="7b0d9-121">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="7b0d9-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="7b0d9-122">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="7b0d9-122">autoLaunch</span></span>|<span data-ttu-id="7b0d9-123">Логический</span><span class="sxs-lookup"><span data-stu-id="7b0d9-123">Boolean</span></span>|<span data-ttu-id="7b0d9-124">Разрешение автоматического запуска приложения в полноэкранном режиме с поддержкой нескольких приложений</span><span class="sxs-lookup"><span data-stu-id="7b0d9-124">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b0d9-125">Связи</span><span class="sxs-lookup"><span data-stu-id="7b0d9-125">Relationships</span></span>
<span data-ttu-id="7b0d9-126">Нет</span><span class="sxs-lookup"><span data-stu-id="7b0d9-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b0d9-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b0d9-127">JSON Representation</span></span>
<span data-ttu-id="7b0d9-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b0d9-128">Here is a JSON representation of the resource.</span></span>
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




