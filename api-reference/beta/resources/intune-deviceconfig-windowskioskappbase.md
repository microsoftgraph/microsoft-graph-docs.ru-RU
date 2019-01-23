---
title: Тип ресурса windowsKioskAppBase
description: Базовый класс для типов приложений
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ca86969eb32a1a1d129fb5ba4cd48bbb04ffd78
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407146"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="d544f-103">Тип ресурса windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="d544f-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="d544f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d544f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d544f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d544f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d544f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d544f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d544f-107">Базовый класс для типов приложений</span><span class="sxs-lookup"><span data-stu-id="d544f-107">The base class for a type of apps</span></span>

## <a name="properties"></a><span data-ttu-id="d544f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d544f-108">Properties</span></span>
|<span data-ttu-id="d544f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d544f-109">Property</span></span>|<span data-ttu-id="d544f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d544f-110">Type</span></span>|<span data-ttu-id="d544f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d544f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d544f-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="d544f-112">startLayoutTileSize</span></span>|[<span data-ttu-id="d544f-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="d544f-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="d544f-114">Размер плитку приложение для макета Пуск.</span><span class="sxs-lookup"><span data-stu-id="d544f-114">The app tile size for the start layout.</span></span> <span data-ttu-id="d544f-115">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="d544f-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="d544f-116">name</span><span class="sxs-lookup"><span data-stu-id="d544f-116">name</span></span>|<span data-ttu-id="d544f-117">String</span><span class="sxs-lookup"><span data-stu-id="d544f-117">String</span></span>|<span data-ttu-id="d544f-118">Представляет понятное имя приложения</span><span class="sxs-lookup"><span data-stu-id="d544f-118">Represents the friendly name of an app</span></span>|
|<span data-ttu-id="d544f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d544f-119">appType</span></span>|[<span data-ttu-id="d544f-120">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="d544f-120">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="d544f-121">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="d544f-121">The app type.</span></span> <span data-ttu-id="d544f-122">Возможные значения: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="d544f-122">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d544f-123">Связи</span><span class="sxs-lookup"><span data-stu-id="d544f-123">Relationships</span></span>
<span data-ttu-id="d544f-124">Нет</span><span class="sxs-lookup"><span data-stu-id="d544f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d544f-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d544f-125">JSON Representation</span></span>
<span data-ttu-id="d544f-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d544f-126">Here is a JSON representation of the resource.</span></span>
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




