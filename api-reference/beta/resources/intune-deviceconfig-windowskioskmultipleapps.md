---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 240625f8cac334375fe1f02b4de0c48f49b73478
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786371"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="b4891-103">Тип ресурса windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="b4891-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="b4891-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4891-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4891-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4891-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4891-106">Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="b4891-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="b4891-107">Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4891-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4891-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4891-108">Properties</span></span>
|<span data-ttu-id="b4891-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4891-109">Property</span></span>|<span data-ttu-id="b4891-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b4891-110">Type</span></span>|<span data-ttu-id="b4891-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b4891-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4891-112">apps</span><span class="sxs-lookup"><span data-stu-id="b4891-112">apps</span></span>|<span data-ttu-id="b4891-113">Коллекция [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="b4891-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="b4891-114">Это единственные приложения Магазина Windows, которые будут доступны для запуска из меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="b4891-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="b4891-115">Эта коллекция может содержать не более 128 элементов.</span><span class="sxs-lookup"><span data-stu-id="b4891-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="b4891-116">шовтаскбар</span><span class="sxs-lookup"><span data-stu-id="b4891-116">showTaskBar</span></span>|<span data-ttu-id="b4891-117">Логический</span><span class="sxs-lookup"><span data-stu-id="b4891-117">Boolean</span></span>|<span data-ttu-id="b4891-118">Этот параметр позволяет администратору указать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="b4891-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="b4891-119">алловакцесстодовнлоадсфолдер</span><span class="sxs-lookup"><span data-stu-id="b4891-119">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="b4891-120">Логический</span><span class="sxs-lookup"><span data-stu-id="b4891-120">Boolean</span></span>|<span data-ttu-id="b4891-121">Этот параметр разрешает доступ к папке "загрузки" в проводнике.</span><span class="sxs-lookup"><span data-stu-id="b4891-121">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="b4891-122">дисалловдесктопаппс</span><span class="sxs-lookup"><span data-stu-id="b4891-122">disallowDesktopApps</span></span>|<span data-ttu-id="b4891-123">Логический</span><span class="sxs-lookup"><span data-stu-id="b4891-123">Boolean</span></span>|<span data-ttu-id="b4891-124">Этот параметр указывает, что классические приложения разрешены.</span><span class="sxs-lookup"><span data-stu-id="b4891-124">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="b4891-125">Значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="b4891-125">Default to true.</span></span>|
|<span data-ttu-id="b4891-126">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="b4891-126">startMenuLayoutXml</span></span>|<span data-ttu-id="b4891-127">Binary</span><span class="sxs-lookup"><span data-stu-id="b4891-127">Binary</span></span>|<span data-ttu-id="b4891-128">Позволяет администраторам переопределять макет запуска по умолчанию и запрещает пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="b4891-128">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="b4891-129">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="b4891-129"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="b4891-130">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="b4891-130">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4891-131">Связи</span><span class="sxs-lookup"><span data-stu-id="b4891-131">Relationships</span></span>
<span data-ttu-id="b4891-132">Нет</span><span class="sxs-lookup"><span data-stu-id="b4891-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4891-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4891-133">JSON Representation</span></span>
<span data-ttu-id="b4891-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4891-134">Here is a JSON representation of the resource.</span></span>
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
      "autoLaunch": true,
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "allowAccessToDownloadsFolder": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```



