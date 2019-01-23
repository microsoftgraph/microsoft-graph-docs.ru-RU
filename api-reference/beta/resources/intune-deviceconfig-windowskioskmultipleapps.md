---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для идентификации конфигурацию разных приложения для базовой конфигурации
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71b8a57151b08d0297a89dfd815f72d66c2d12a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396030"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="4cf38-103">Тип ресурса windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="4cf38-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="4cf38-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4cf38-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4cf38-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cf38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4cf38-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cf38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cf38-107">Класс, используемый для идентификации конфигурацию разных приложения для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="4cf38-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="4cf38-108">Наследуется от [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cf38-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4cf38-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cf38-109">Properties</span></span>
|<span data-ttu-id="4cf38-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cf38-110">Property</span></span>|<span data-ttu-id="4cf38-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4cf38-111">Type</span></span>|<span data-ttu-id="4cf38-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4cf38-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf38-113">apps</span><span class="sxs-lookup"><span data-stu-id="4cf38-113">apps</span></span>|<span data-ttu-id="4cf38-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4cf38-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="4cf38-115">Это единственный приложений для магазина Windows, чтобы оно было доступно для запуска в меню Пуск.</span><span class="sxs-lookup"><span data-stu-id="4cf38-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="4cf38-116">Эта коллекция может содержать не более 128 элементов.</span><span class="sxs-lookup"><span data-stu-id="4cf38-116">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="4cf38-117">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="4cf38-117">showTaskBar</span></span>|<span data-ttu-id="4cf38-118">Логический</span><span class="sxs-lookup"><span data-stu-id="4cf38-118">Boolean</span></span>|<span data-ttu-id="4cf38-119">Этот параметр позволяет администратору задать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="4cf38-119">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="4cf38-120">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="4cf38-120">disallowDesktopApps</span></span>|<span data-ttu-id="4cf38-121">Логический</span><span class="sxs-lookup"><span data-stu-id="4cf38-121">Boolean</span></span>|<span data-ttu-id="4cf38-122">Этот параметр показывает, что приложений для настольных систем.</span><span class="sxs-lookup"><span data-stu-id="4cf38-122">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="4cf38-123">По умолчанию установлено значение true.</span><span class="sxs-lookup"><span data-stu-id="4cf38-123">Default to true.</span></span>|
|<span data-ttu-id="4cf38-124">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="4cf38-124">startMenuLayoutXml</span></span>|<span data-ttu-id="4cf38-125">Binary</span><span class="sxs-lookup"><span data-stu-id="4cf38-125">Binary</span></span>|<span data-ttu-id="4cf38-126">Позволяет администраторам переопределить макет Пуск по умолчанию и не позволяет пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="4cf38-126">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="4cf38-127">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="4cf38-127"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="4cf38-128">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="4cf38-128">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cf38-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="4cf38-129">Relationships</span></span>
<span data-ttu-id="4cf38-130">Нет</span><span class="sxs-lookup"><span data-stu-id="4cf38-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cf38-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4cf38-131">JSON Representation</span></span>
<span data-ttu-id="4cf38-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cf38-132">Here is a JSON representation of the resource.</span></span>
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
      "appType": "String",
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




