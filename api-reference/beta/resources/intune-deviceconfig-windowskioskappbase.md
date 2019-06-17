---
title: Тип ресурса Виндовскиоскаппбасе
description: Базовый класс для типа приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4dc6c54c9b788ae3456017fc0be63c636d980af8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993966"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="f019f-103">Тип ресурса Виндовскиоскаппбасе</span><span class="sxs-lookup"><span data-stu-id="f019f-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="f019f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f019f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f019f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f019f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f019f-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="f019f-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="f019f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f019f-107">Properties</span></span>
|<span data-ttu-id="f019f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f019f-108">Property</span></span>|<span data-ttu-id="f019f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f019f-109">Type</span></span>|<span data-ttu-id="f019f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f019f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f019f-111">Стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="f019f-111">startLayoutTileSize</span></span>|[<span data-ttu-id="f019f-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="f019f-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="f019f-113">Размер плитки приложения для начального макета.</span><span class="sxs-lookup"><span data-stu-id="f019f-113">The app tile size for the start layout.</span></span> <span data-ttu-id="f019f-114">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="f019f-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="f019f-115">name</span><span class="sxs-lookup"><span data-stu-id="f019f-115">name</span></span>|<span data-ttu-id="f019f-116">String</span><span class="sxs-lookup"><span data-stu-id="f019f-116">String</span></span>|<span data-ttu-id="f019f-117">Представляет понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="f019f-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="f019f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="f019f-118">appType</span></span>|[<span data-ttu-id="f019f-119">Виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="f019f-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="f019f-120">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="f019f-120">The app type.</span></span> <span data-ttu-id="f019f-121">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="f019f-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="f019f-122">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="f019f-122">autoLaunch</span></span>|<span data-ttu-id="f019f-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="f019f-123">Boolean</span></span>|<span data-ttu-id="f019f-124">Разрешение автоматического запуска приложения в полноэкранном режиме с поддержкой нескольких приложений</span><span class="sxs-lookup"><span data-stu-id="f019f-124">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="f019f-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="f019f-125">Relationships</span></span>
<span data-ttu-id="f019f-126">Нет</span><span class="sxs-lookup"><span data-stu-id="f019f-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f019f-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f019f-127">JSON Representation</span></span>
<span data-ttu-id="f019f-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f019f-128">Here is a JSON representation of the resource.</span></span>
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





