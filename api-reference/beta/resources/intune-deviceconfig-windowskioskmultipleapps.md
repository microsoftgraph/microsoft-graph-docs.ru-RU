---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df9fec1c5d21d7d23c5c7a56c3760b88348c556b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944007"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="5c607-103">Тип ресурса windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="5c607-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="5c607-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c607-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c607-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c607-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c607-106">Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="5c607-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="5c607-107">Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c607-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5c607-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c607-108">Properties</span></span>
|<span data-ttu-id="5c607-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c607-109">Property</span></span>|<span data-ttu-id="5c607-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5c607-110">Type</span></span>|<span data-ttu-id="5c607-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5c607-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c607-112">apps</span><span class="sxs-lookup"><span data-stu-id="5c607-112">apps</span></span>|<span data-ttu-id="5c607-113">Коллекция [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="5c607-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="5c607-114">Это единственные приложения Магазина Windows, которые будут доступны для запуска из меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="5c607-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="5c607-115">Эта коллекция может содержать не более 128 элементов.</span><span class="sxs-lookup"><span data-stu-id="5c607-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="5c607-116">Шовтаскбар</span><span class="sxs-lookup"><span data-stu-id="5c607-116">showTaskBar</span></span>|<span data-ttu-id="5c607-117">Логический</span><span class="sxs-lookup"><span data-stu-id="5c607-117">Boolean</span></span>|<span data-ttu-id="5c607-118">Этот параметр позволяет администратору указать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="5c607-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="5c607-119">Алловакцесстодовнлоадсфолдер</span><span class="sxs-lookup"><span data-stu-id="5c607-119">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="5c607-120">Логический</span><span class="sxs-lookup"><span data-stu-id="5c607-120">Boolean</span></span>|<span data-ttu-id="5c607-121">Этот параметр разрешает доступ к папке "загрузки" в проводнике.</span><span class="sxs-lookup"><span data-stu-id="5c607-121">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="5c607-122">Дисалловдесктопаппс</span><span class="sxs-lookup"><span data-stu-id="5c607-122">disallowDesktopApps</span></span>|<span data-ttu-id="5c607-123">Логический</span><span class="sxs-lookup"><span data-stu-id="5c607-123">Boolean</span></span>|<span data-ttu-id="5c607-124">Этот параметр указывает, что классические приложения разрешены.</span><span class="sxs-lookup"><span data-stu-id="5c607-124">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="5c607-125">Значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="5c607-125">Default to true.</span></span>|
|<span data-ttu-id="5c607-126">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="5c607-126">startMenuLayoutXml</span></span>|<span data-ttu-id="5c607-127">Binary</span><span class="sxs-lookup"><span data-stu-id="5c607-127">Binary</span></span>|<span data-ttu-id="5c607-128">Позволяет администраторам переопределять макет запуска по умолчанию и запрещает пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="5c607-128">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="5c607-129">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="5c607-129"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="5c607-130">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="5c607-130">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c607-131">Связи</span><span class="sxs-lookup"><span data-stu-id="5c607-131">Relationships</span></span>
<span data-ttu-id="5c607-132">Нет</span><span class="sxs-lookup"><span data-stu-id="5c607-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c607-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c607-133">JSON Representation</span></span>
<span data-ttu-id="5c607-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c607-134">Here is a JSON representation of the resource.</span></span>
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




