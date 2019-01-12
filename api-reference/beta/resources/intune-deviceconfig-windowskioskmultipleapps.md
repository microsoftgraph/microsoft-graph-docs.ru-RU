---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для идентификации конфигурацию разных приложения для базовой конфигурации
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3770f8c63be230dff97e43d3706ed35d79826751
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977131"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="c9073-103">Тип ресурса windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="c9073-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="c9073-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9073-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9073-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9073-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9073-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c9073-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9073-107">Класс, используемый для идентификации конфигурацию разных приложения для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="c9073-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>

<span data-ttu-id="c9073-108">Наследуется от [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9073-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9073-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9073-109">Properties</span></span>
|<span data-ttu-id="c9073-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9073-110">Property</span></span>|<span data-ttu-id="c9073-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c9073-111">Type</span></span>|<span data-ttu-id="c9073-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c9073-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9073-113">apps</span><span class="sxs-lookup"><span data-stu-id="c9073-113">apps</span></span>|<span data-ttu-id="c9073-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c9073-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="c9073-115">Это единственный приложений для магазина Windows, чтобы оно было доступно для запуска в меню Пуск.</span><span class="sxs-lookup"><span data-stu-id="c9073-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="c9073-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="c9073-116">showTaskBar</span></span>|<span data-ttu-id="c9073-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9073-117">Boolean</span></span>|<span data-ttu-id="c9073-118">Этот параметр позволяет администратору задать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="c9073-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="c9073-119">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="c9073-119">disallowDesktopApps</span></span>|<span data-ttu-id="c9073-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9073-120">Boolean</span></span>|<span data-ttu-id="c9073-121">Этот параметр показывает, что приложений для настольных систем.</span><span class="sxs-lookup"><span data-stu-id="c9073-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="c9073-122">По умолчанию установлено значение true.</span><span class="sxs-lookup"><span data-stu-id="c9073-122">Default to true.</span></span>|
|<span data-ttu-id="c9073-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="c9073-123">startMenuLayoutXml</span></span>|<span data-ttu-id="c9073-124">Binary</span><span class="sxs-lookup"><span data-stu-id="c9073-124">Binary</span></span>|<span data-ttu-id="c9073-125">Позволяет администраторам переопределить макет Пуск по умолчанию и не позволяет пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="c9073-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="c9073-126">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="c9073-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="c9073-127">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="c9073-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9073-128">Связи</span><span class="sxs-lookup"><span data-stu-id="c9073-128">Relationships</span></span>
<span data-ttu-id="c9073-129">Нет</span><span class="sxs-lookup"><span data-stu-id="c9073-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9073-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9073-130">JSON Representation</span></span>
<span data-ttu-id="c9073-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9073-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
  "apps": [
    {
      "@odata.type": "microsoft.graph.windowsKioskUWPApp",
      "startLayoutTileSize": "String",
      "name": "String",
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```





