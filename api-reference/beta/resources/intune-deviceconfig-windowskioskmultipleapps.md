---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для идентификации конфигурацию разных приложения для базовой конфигурации
ms.openlocfilehash: 2b52cbe343c4a8d81391ad448e8f10f64fef295e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077450"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="5e6a4-103">Тип ресурса windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="5e6a4-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="5e6a4-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e6a4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e6a4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e6a4-107">Класс, используемый для идентификации конфигурацию разных приложения для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="5e6a4-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>

<span data-ttu-id="5e6a4-108">Наследуется от [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e6a4-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5e6a4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e6a4-109">Properties</span></span>
|<span data-ttu-id="5e6a4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e6a4-110">Property</span></span>|<span data-ttu-id="5e6a4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5e6a4-111">Type</span></span>|<span data-ttu-id="5e6a4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5e6a4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e6a4-113">apps</span><span class="sxs-lookup"><span data-stu-id="5e6a4-113">apps</span></span>|<span data-ttu-id="5e6a4-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5e6a4-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="5e6a4-115">Это единственный приложений для магазина Windows, чтобы оно было доступно для запуска в меню Пуск.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="5e6a4-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="5e6a4-116">showTaskBar</span></span>|<span data-ttu-id="5e6a4-117">Логический</span><span class="sxs-lookup"><span data-stu-id="5e6a4-117">Boolean</span></span>|<span data-ttu-id="5e6a4-118">Этот параметр позволяет администратору задать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="5e6a4-119">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="5e6a4-119">disallowDesktopApps</span></span>|<span data-ttu-id="5e6a4-120">Логический</span><span class="sxs-lookup"><span data-stu-id="5e6a4-120">Boolean</span></span>|<span data-ttu-id="5e6a4-121">Этот параметр показывает, что приложений для настольных систем.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="5e6a4-122">По умолчанию установлено значение true.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-122">Default to true.</span></span>|
|<span data-ttu-id="5e6a4-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="5e6a4-123">startMenuLayoutXml</span></span>|<span data-ttu-id="5e6a4-124">Binary</span><span class="sxs-lookup"><span data-stu-id="5e6a4-124">Binary</span></span>|<span data-ttu-id="5e6a4-125">Позволяет администраторам переопределить макет Пуск по умолчанию и не позволяет пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="5e6a4-126">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="5e6a4-127">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e6a4-128">Связи</span><span class="sxs-lookup"><span data-stu-id="5e6a4-128">Relationships</span></span>
<span data-ttu-id="5e6a4-129">Нет</span><span class="sxs-lookup"><span data-stu-id="5e6a4-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5e6a4-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e6a4-130">JSON Representation</span></span>
<span data-ttu-id="5e6a4-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e6a4-131">Here is a JSON representation of the resource.</span></span>
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





