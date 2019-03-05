---
title: Тип ресурса Виндовскиоскаппбасе
description: Базовый класс для типа приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0247febfbeebe7fc047df4bb14a9d421b79bf01
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145299"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="dd2f3-103">Тип ресурса Виндовскиоскаппбасе</span><span class="sxs-lookup"><span data-stu-id="dd2f3-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="dd2f3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd2f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd2f3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd2f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd2f3-106">Базовый класс для типа приложений</span><span class="sxs-lookup"><span data-stu-id="dd2f3-106">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="dd2f3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd2f3-107">Properties</span></span>
|<span data-ttu-id="dd2f3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd2f3-108">Property</span></span>|<span data-ttu-id="dd2f3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dd2f3-109">Type</span></span>|<span data-ttu-id="dd2f3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dd2f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd2f3-111">Стартлайауттилесизе</span><span class="sxs-lookup"><span data-stu-id="dd2f3-111">startLayoutTileSize</span></span>|[<span data-ttu-id="dd2f3-112">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="dd2f3-112">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="dd2f3-113">Размер плитки приложения для начального макета.</span><span class="sxs-lookup"><span data-stu-id="dd2f3-113">The app tile size for the start layout.</span></span> <span data-ttu-id="dd2f3-114">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="dd2f3-114">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="dd2f3-115">name</span><span class="sxs-lookup"><span data-stu-id="dd2f3-115">name</span></span>|<span data-ttu-id="dd2f3-116">String</span><span class="sxs-lookup"><span data-stu-id="dd2f3-116">String</span></span>|<span data-ttu-id="dd2f3-117">Представляет понятное имя приложения.</span><span class="sxs-lookup"><span data-stu-id="dd2f3-117">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="dd2f3-118">Тип</span><span class="sxs-lookup"><span data-stu-id="dd2f3-118">appType</span></span>|[<span data-ttu-id="dd2f3-119">Виндовскиоскапптипе</span><span class="sxs-lookup"><span data-stu-id="dd2f3-119">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="dd2f3-120">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="dd2f3-120">The app type.</span></span> <span data-ttu-id="dd2f3-121">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="dd2f3-121">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd2f3-122">Связи</span><span class="sxs-lookup"><span data-stu-id="dd2f3-122">Relationships</span></span>
<span data-ttu-id="dd2f3-123">Нет</span><span class="sxs-lookup"><span data-stu-id="dd2f3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd2f3-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd2f3-124">JSON Representation</span></span>
<span data-ttu-id="dd2f3-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd2f3-125">Here is a JSON representation of the resource.</span></span>
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
  "appType": "String"
}
```




