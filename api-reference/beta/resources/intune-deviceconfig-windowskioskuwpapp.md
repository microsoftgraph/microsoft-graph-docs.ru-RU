---
title: Тип ресурса windowsKioskUWPApp
description: Базовый класс для типов приложений
ms.openlocfilehash: 8d0d6c609eec4b8194bb72d2fb723d1816873e75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077443"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="39c58-103">Тип ресурса windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="39c58-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="39c58-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="39c58-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39c58-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39c58-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39c58-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="39c58-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39c58-107">Базовый класс для типов приложений</span><span class="sxs-lookup"><span data-stu-id="39c58-107">The base class for a type of apps</span></span>

<span data-ttu-id="39c58-108">Наследуется от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="39c58-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="39c58-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="39c58-109">Properties</span></span>
|<span data-ttu-id="39c58-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="39c58-110">Property</span></span>|<span data-ttu-id="39c58-111">Тип</span><span class="sxs-lookup"><span data-stu-id="39c58-111">Type</span></span>|<span data-ttu-id="39c58-112">Description</span><span class="sxs-lookup"><span data-stu-id="39c58-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39c58-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="39c58-113">startLayoutTileSize</span></span>|[<span data-ttu-id="39c58-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="39c58-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="39c58-115">Размер плитку приложение для макета Пуск унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="39c58-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="39c58-116">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="39c58-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="39c58-117">name</span><span class="sxs-lookup"><span data-stu-id="39c58-117">name</span></span>|<span data-ttu-id="39c58-118">String</span><span class="sxs-lookup"><span data-stu-id="39c58-118">String</span></span>|<span data-ttu-id="39c58-119">Представляет понятное имя приложения унаследованные от [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="39c58-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="39c58-120">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="39c58-120">appUserModelId</span></span>|<span data-ttu-id="39c58-121">String</span><span class="sxs-lookup"><span data-stu-id="39c58-121">String</span></span>|<span data-ttu-id="39c58-122">Это единственный идентификатор модели приложения пользователя (AUMID), чтобы оно было доступно для использования в полноэкранном режиме запуска</span><span class="sxs-lookup"><span data-stu-id="39c58-122">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="39c58-123">appId</span><span class="sxs-lookup"><span data-stu-id="39c58-123">appId</span></span>|<span data-ttu-id="39c58-124">String</span><span class="sxs-lookup"><span data-stu-id="39c58-124">String</span></span>|<span data-ttu-id="39c58-125">Это ссылается на Intune приложения, который будет целевой для те же назначения как базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="39c58-125">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="39c58-126">containedAppId</span><span class="sxs-lookup"><span data-stu-id="39c58-126">containedAppId</span></span>|<span data-ttu-id="39c58-127">String</span><span class="sxs-lookup"><span data-stu-id="39c58-127">String</span></span>|<span data-ttu-id="39c58-128">Это ссылается автономные приложения из приложения для Intune</span><span class="sxs-lookup"><span data-stu-id="39c58-128">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="39c58-129">Связи</span><span class="sxs-lookup"><span data-stu-id="39c58-129">Relationships</span></span>
<span data-ttu-id="39c58-130">Нет</span><span class="sxs-lookup"><span data-stu-id="39c58-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39c58-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39c58-131">JSON Representation</span></span>
<span data-ttu-id="39c58-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39c58-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```





