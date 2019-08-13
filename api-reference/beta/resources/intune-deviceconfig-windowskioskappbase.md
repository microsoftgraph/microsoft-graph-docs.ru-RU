---
title: Тип ресурса Виндовскиоскаппбасе
description: Базовый класс для типа приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 167244028d1d0773caf1802092d70a1cf3ec7560
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371035"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="cd32b-103">Тип ресурса Виндовскиоскаппбасе</span><span class="sxs-lookup"><span data-stu-id="cd32b-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="cd32b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd32b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd32b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd32b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd32b-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="cd32b-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="cd32b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd32b-107">Properties</span></span>
|<span data-ttu-id="cd32b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd32b-108">Property</span></span>|<span data-ttu-id="cd32b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cd32b-109">Type</span></span>|<span data-ttu-id="cd32b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd32b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd32b-111">стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="cd32b-111">startLayoutTileSize</span></span>|[<span data-ttu-id="cd32b-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="cd32b-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="cd32b-113">Размер плитки приложения для начального макета.</span><span class="sxs-lookup"><span data-stu-id="cd32b-113">The app tile size for the start layout.</span></span> <span data-ttu-id="cd32b-114">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="cd32b-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="cd32b-115">name</span><span class="sxs-lookup"><span data-stu-id="cd32b-115">name</span></span>|<span data-ttu-id="cd32b-116">String</span><span class="sxs-lookup"><span data-stu-id="cd32b-116">String</span></span>|<span data-ttu-id="cd32b-117">Представляет понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="cd32b-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="cd32b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="cd32b-118">appType</span></span>|[<span data-ttu-id="cd32b-119">виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="cd32b-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="cd32b-120">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="cd32b-120">The app type.</span></span> <span data-ttu-id="cd32b-121">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="cd32b-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="cd32b-122">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="cd32b-122">autoLaunch</span></span>|<span data-ttu-id="cd32b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd32b-123">Boolean</span></span>|<span data-ttu-id="cd32b-124">Разрешение автоматического запуска приложения в полноэкранном режиме с поддержкой нескольких приложений</span><span class="sxs-lookup"><span data-stu-id="cd32b-124">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd32b-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="cd32b-125">Relationships</span></span>
<span data-ttu-id="cd32b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="cd32b-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd32b-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd32b-127">JSON Representation</span></span>
<span data-ttu-id="cd32b-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd32b-128">Here is a JSON representation of the resource.</span></span>
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



