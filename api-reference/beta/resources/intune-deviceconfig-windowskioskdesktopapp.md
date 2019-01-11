---
title: Тип ресурса windowsKioskDesktopApp
description: Базовый класс для типов приложений
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53eb615dcd1ba2b88c6cdd4bb5a1b76b83b67eaf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830977"
---
# <a name="windowskioskdesktopapp-resource-type"></a><span data-ttu-id="47905-103">Тип ресурса windowsKioskDesktopApp</span><span class="sxs-lookup"><span data-stu-id="47905-103">windowsKioskDesktopApp resource type</span></span>

> <span data-ttu-id="47905-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47905-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47905-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47905-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47905-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47905-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47905-107">Базовый класс для типов приложений</span><span class="sxs-lookup"><span data-stu-id="47905-107">The base class for a type of apps</span></span>

<span data-ttu-id="47905-108">Наследуется от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="47905-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47905-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="47905-109">Properties</span></span>
|<span data-ttu-id="47905-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="47905-110">Property</span></span>|<span data-ttu-id="47905-111">Тип</span><span class="sxs-lookup"><span data-stu-id="47905-111">Type</span></span>|<span data-ttu-id="47905-112">Описание</span><span class="sxs-lookup"><span data-stu-id="47905-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47905-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="47905-113">startLayoutTileSize</span></span>|[<span data-ttu-id="47905-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="47905-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="47905-115">Размер плитку приложение для макета Пуск унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="47905-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="47905-116">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="47905-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="47905-117">name</span><span class="sxs-lookup"><span data-stu-id="47905-117">name</span></span>|<span data-ttu-id="47905-118">Строка</span><span class="sxs-lookup"><span data-stu-id="47905-118">String</span></span>|<span data-ttu-id="47905-119">Представляет понятное имя приложения унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="47905-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="47905-120">path</span><span class="sxs-lookup"><span data-stu-id="47905-120">path</span></span>|<span data-ttu-id="47905-121">String</span><span class="sxs-lookup"><span data-stu-id="47905-121">String</span></span>|<span data-ttu-id="47905-122">Определение пути классического приложения</span><span class="sxs-lookup"><span data-stu-id="47905-122">Define the path of a desktop app</span></span>|
|<span data-ttu-id="47905-123">desktopApplicationId</span><span class="sxs-lookup"><span data-stu-id="47905-123">desktopApplicationId</span></span>|<span data-ttu-id="47905-124">Строка</span><span class="sxs-lookup"><span data-stu-id="47905-124">String</span></span>|<span data-ttu-id="47905-125">Определение DesktopApplicationID приложения</span><span class="sxs-lookup"><span data-stu-id="47905-125">Define the DesktopApplicationID of the app</span></span>|
|<span data-ttu-id="47905-126">desktopApplicationLinkPath</span><span class="sxs-lookup"><span data-stu-id="47905-126">desktopApplicationLinkPath</span></span>|<span data-ttu-id="47905-127">Строка</span><span class="sxs-lookup"><span data-stu-id="47905-127">String</span></span>|<span data-ttu-id="47905-128">Определение DesktopApplicationLinkPath приложения</span><span class="sxs-lookup"><span data-stu-id="47905-128">Define the DesktopApplicationLinkPath of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="47905-129">Связи</span><span class="sxs-lookup"><span data-stu-id="47905-129">Relationships</span></span>
<span data-ttu-id="47905-130">Нет</span><span class="sxs-lookup"><span data-stu-id="47905-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47905-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47905-131">JSON Representation</span></span>
<span data-ttu-id="47905-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47905-132">Here is a JSON representation of the resource.</span></span>
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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





