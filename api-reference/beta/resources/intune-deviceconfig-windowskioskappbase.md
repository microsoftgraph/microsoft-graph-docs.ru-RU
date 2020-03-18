---
title: Тип ресурса Виндовскиоскаппбасе
description: Базовый класс для типа приложений
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3ba4a27f1107b35264d1671530b5314ea28026c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786448"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="7a4f8-103">Тип ресурса Виндовскиоскаппбасе</span><span class="sxs-lookup"><span data-stu-id="7a4f8-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="7a4f8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a4f8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a4f8-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="7a4f8-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="7a4f8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a4f8-107">Properties</span></span>
|<span data-ttu-id="7a4f8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a4f8-108">Property</span></span>|<span data-ttu-id="7a4f8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7a4f8-109">Type</span></span>|<span data-ttu-id="7a4f8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7a4f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a4f8-111">стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="7a4f8-111">startLayoutTileSize</span></span>|[<span data-ttu-id="7a4f8-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="7a4f8-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="7a4f8-113">Размер плитки приложения для начального макета.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-113">The app tile size for the start layout.</span></span> <span data-ttu-id="7a4f8-114">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="7a4f8-115">name</span><span class="sxs-lookup"><span data-stu-id="7a4f8-115">name</span></span>|<span data-ttu-id="7a4f8-116">String</span><span class="sxs-lookup"><span data-stu-id="7a4f8-116">String</span></span>|<span data-ttu-id="7a4f8-117">Представляет понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="7a4f8-118">Тип</span><span class="sxs-lookup"><span data-stu-id="7a4f8-118">appType</span></span>|[<span data-ttu-id="7a4f8-119">виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="7a4f8-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="7a4f8-120">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-120">The app type.</span></span> <span data-ttu-id="7a4f8-121">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="7a4f8-122">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="7a4f8-122">autoLaunch</span></span>|<span data-ttu-id="7a4f8-123">Логический</span><span class="sxs-lookup"><span data-stu-id="7a4f8-123">Boolean</span></span>|<span data-ttu-id="7a4f8-124">Разрешение автоматического запуска приложения в полноэкранном режиме с поддержкой нескольких приложений</span><span class="sxs-lookup"><span data-stu-id="7a4f8-124">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a4f8-125">Связи</span><span class="sxs-lookup"><span data-stu-id="7a4f8-125">Relationships</span></span>
<span data-ttu-id="7a4f8-126">Нет</span><span class="sxs-lookup"><span data-stu-id="7a4f8-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a4f8-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a4f8-127">JSON Representation</span></span>
<span data-ttu-id="7a4f8-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-128">Here is a JSON representation of the resource.</span></span>
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



