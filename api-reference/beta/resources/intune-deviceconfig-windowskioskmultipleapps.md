---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 010f8196bd152b872b3910eec9759e31efa4a1e1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463459"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="04a06-103">Тип ресурса windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="04a06-103">windowsKioskMultipleApps resource type</span></span>

<span data-ttu-id="04a06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04a06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04a06-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04a06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04a06-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04a06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04a06-107">Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="04a06-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="04a06-108">Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04a06-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="04a06-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="04a06-109">Properties</span></span>
|<span data-ttu-id="04a06-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="04a06-110">Property</span></span>|<span data-ttu-id="04a06-111">Тип</span><span class="sxs-lookup"><span data-stu-id="04a06-111">Type</span></span>|<span data-ttu-id="04a06-112">Описание</span><span class="sxs-lookup"><span data-stu-id="04a06-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04a06-113">apps</span><span class="sxs-lookup"><span data-stu-id="04a06-113">apps</span></span>|<span data-ttu-id="04a06-114">Коллекция [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="04a06-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="04a06-115">Это единственные приложения Магазина Windows, которые будут доступны для запуска из меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="04a06-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="04a06-116">Эта коллекция может содержать не более 128 элементов.</span><span class="sxs-lookup"><span data-stu-id="04a06-116">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="04a06-117">шовтаскбар</span><span class="sxs-lookup"><span data-stu-id="04a06-117">showTaskBar</span></span>|<span data-ttu-id="04a06-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="04a06-118">Boolean</span></span>|<span data-ttu-id="04a06-119">Этот параметр позволяет администратору указать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="04a06-119">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="04a06-120">алловакцесстодовнлоадсфолдер</span><span class="sxs-lookup"><span data-stu-id="04a06-120">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="04a06-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="04a06-121">Boolean</span></span>|<span data-ttu-id="04a06-122">Этот параметр разрешает доступ к папке "загрузки" в проводнике.</span><span class="sxs-lookup"><span data-stu-id="04a06-122">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="04a06-123">дисалловдесктопаппс</span><span class="sxs-lookup"><span data-stu-id="04a06-123">disallowDesktopApps</span></span>|<span data-ttu-id="04a06-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="04a06-124">Boolean</span></span>|<span data-ttu-id="04a06-125">Этот параметр указывает, что классические приложения разрешены.</span><span class="sxs-lookup"><span data-stu-id="04a06-125">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="04a06-126">Значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="04a06-126">Default to true.</span></span>|
|<span data-ttu-id="04a06-127">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="04a06-127">startMenuLayoutXml</span></span>|<span data-ttu-id="04a06-128">Binary</span><span class="sxs-lookup"><span data-stu-id="04a06-128">Binary</span></span>|<span data-ttu-id="04a06-129">Позволяет администраторам переопределять макет запуска по умолчанию и запрещает пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="04a06-129">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="04a06-130">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="04a06-130"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="04a06-131">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="04a06-131">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04a06-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="04a06-132">Relationships</span></span>
<span data-ttu-id="04a06-133">Нет</span><span class="sxs-lookup"><span data-stu-id="04a06-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04a06-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04a06-134">JSON Representation</span></span>
<span data-ttu-id="04a06-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04a06-135">Here is a JSON representation of the resource.</span></span>
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



