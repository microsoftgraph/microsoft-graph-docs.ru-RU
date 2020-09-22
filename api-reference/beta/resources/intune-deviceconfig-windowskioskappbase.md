---
title: Тип ресурса Виндовскиоскаппбасе
description: Базовый класс для типа приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2162086c2a70a44207830f61f4456574a5bfe9bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039890"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="2907c-103">Тип ресурса Виндовскиоскаппбасе</span><span class="sxs-lookup"><span data-stu-id="2907c-103">windowsKioskAppBase resource type</span></span>

<span data-ttu-id="2907c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2907c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2907c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2907c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2907c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2907c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2907c-107">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="2907c-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="2907c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2907c-108">Properties</span></span>
|<span data-ttu-id="2907c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2907c-109">Property</span></span>|<span data-ttu-id="2907c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2907c-110">Type</span></span>|<span data-ttu-id="2907c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2907c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2907c-112">стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="2907c-112">startLayoutTileSize</span></span>|[<span data-ttu-id="2907c-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="2907c-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="2907c-114">Размер плитки приложения для начального макета.</span><span class="sxs-lookup"><span data-stu-id="2907c-114">The app tile size for the start layout.</span></span> <span data-ttu-id="2907c-115">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="2907c-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="2907c-116">name</span><span class="sxs-lookup"><span data-stu-id="2907c-116">name</span></span>|<span data-ttu-id="2907c-117">String</span><span class="sxs-lookup"><span data-stu-id="2907c-117">String</span></span>|<span data-ttu-id="2907c-118">Представляет понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="2907c-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="2907c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2907c-119">appType</span></span>|[<span data-ttu-id="2907c-120">виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="2907c-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="2907c-121">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="2907c-121">The app type.</span></span> <span data-ttu-id="2907c-122">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="2907c-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="2907c-123">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="2907c-123">autoLaunch</span></span>|<span data-ttu-id="2907c-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="2907c-124">Boolean</span></span>|<span data-ttu-id="2907c-125">Разрешение автоматического запуска приложения в полноэкранном режиме с поддержкой нескольких приложений</span><span class="sxs-lookup"><span data-stu-id="2907c-125">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="2907c-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="2907c-126">Relationships</span></span>
<span data-ttu-id="2907c-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2907c-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2907c-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2907c-128">JSON Representation</span></span>
<span data-ttu-id="2907c-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2907c-129">Here is a JSON representation of the resource.</span></span>
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






