---
title: Тип ресурса Виндовскиоскаппбасе
description: Базовый класс для типа приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4212dfd0362ed6253c10a2b2796241c74678dda2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736214"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="74fda-103">Тип ресурса Виндовскиоскаппбасе</span><span class="sxs-lookup"><span data-stu-id="74fda-103">windowsKioskAppBase resource type</span></span>

<span data-ttu-id="74fda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74fda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74fda-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74fda-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74fda-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74fda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74fda-107">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="74fda-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="74fda-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="74fda-108">Properties</span></span>
|<span data-ttu-id="74fda-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="74fda-109">Property</span></span>|<span data-ttu-id="74fda-110">Тип</span><span class="sxs-lookup"><span data-stu-id="74fda-110">Type</span></span>|<span data-ttu-id="74fda-111">Описание</span><span class="sxs-lookup"><span data-stu-id="74fda-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74fda-112">стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="74fda-112">startLayoutTileSize</span></span>|[<span data-ttu-id="74fda-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="74fda-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="74fda-114">Размер плитки приложения для начального макета.</span><span class="sxs-lookup"><span data-stu-id="74fda-114">The app tile size for the start layout.</span></span> <span data-ttu-id="74fda-115">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="74fda-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="74fda-116">name</span><span class="sxs-lookup"><span data-stu-id="74fda-116">name</span></span>|<span data-ttu-id="74fda-117">String</span><span class="sxs-lookup"><span data-stu-id="74fda-117">String</span></span>|<span data-ttu-id="74fda-118">Представляет понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="74fda-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="74fda-119">Тип</span><span class="sxs-lookup"><span data-stu-id="74fda-119">appType</span></span>|[<span data-ttu-id="74fda-120">виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="74fda-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="74fda-121">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="74fda-121">The app type.</span></span> <span data-ttu-id="74fda-122">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="74fda-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="74fda-123">Автозапуск</span><span class="sxs-lookup"><span data-stu-id="74fda-123">autoLaunch</span></span>|<span data-ttu-id="74fda-124">Логический</span><span class="sxs-lookup"><span data-stu-id="74fda-124">Boolean</span></span>|<span data-ttu-id="74fda-125">Разрешение автоматического запуска приложения в полноэкранном режиме с поддержкой нескольких приложений</span><span class="sxs-lookup"><span data-stu-id="74fda-125">Allow the app to be auto-launched in multi-app kiosk mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="74fda-126">Связи</span><span class="sxs-lookup"><span data-stu-id="74fda-126">Relationships</span></span>
<span data-ttu-id="74fda-127">Нет</span><span class="sxs-lookup"><span data-stu-id="74fda-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74fda-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74fda-128">JSON Representation</span></span>
<span data-ttu-id="74fda-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74fda-129">Here is a JSON representation of the resource.</span></span>
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





