---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cbe64a4c58d405c0ea43e6201f3207169f3c1268
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370853"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="81040-103">Тип ресурса windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="81040-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="81040-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81040-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81040-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81040-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81040-106">Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="81040-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="81040-107">Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81040-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81040-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="81040-108">Properties</span></span>
|<span data-ttu-id="81040-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="81040-109">Property</span></span>|<span data-ttu-id="81040-110">Тип</span><span class="sxs-lookup"><span data-stu-id="81040-110">Type</span></span>|<span data-ttu-id="81040-111">Описание</span><span class="sxs-lookup"><span data-stu-id="81040-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81040-112">apps</span><span class="sxs-lookup"><span data-stu-id="81040-112">apps</span></span>|<span data-ttu-id="81040-113">Коллекция [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="81040-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="81040-114">Это единственные приложения Магазина Windows, которые будут доступны для запуска из меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="81040-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="81040-115">Эта коллекция может содержать не более 128 элементов.</span><span class="sxs-lookup"><span data-stu-id="81040-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="81040-116">шовтаскбар</span><span class="sxs-lookup"><span data-stu-id="81040-116">showTaskBar</span></span>|<span data-ttu-id="81040-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="81040-117">Boolean</span></span>|<span data-ttu-id="81040-118">Этот параметр позволяет администратору указать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="81040-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="81040-119">алловакцесстодовнлоадсфолдер</span><span class="sxs-lookup"><span data-stu-id="81040-119">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="81040-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="81040-120">Boolean</span></span>|<span data-ttu-id="81040-121">Этот параметр разрешает доступ к папке "загрузки" в проводнике.</span><span class="sxs-lookup"><span data-stu-id="81040-121">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="81040-122">дисалловдесктопаппс</span><span class="sxs-lookup"><span data-stu-id="81040-122">disallowDesktopApps</span></span>|<span data-ttu-id="81040-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="81040-123">Boolean</span></span>|<span data-ttu-id="81040-124">Этот параметр указывает, что классические приложения разрешены.</span><span class="sxs-lookup"><span data-stu-id="81040-124">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="81040-125">Значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="81040-125">Default to true.</span></span>|
|<span data-ttu-id="81040-126">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="81040-126">startMenuLayoutXml</span></span>|<span data-ttu-id="81040-127">Binary</span><span class="sxs-lookup"><span data-stu-id="81040-127">Binary</span></span>|<span data-ttu-id="81040-128">Позволяет администраторам переопределять макет запуска по умолчанию и запрещает пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="81040-128">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="81040-129">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="81040-129"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="81040-130">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="81040-130">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81040-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="81040-131">Relationships</span></span>
<span data-ttu-id="81040-132">Нет</span><span class="sxs-lookup"><span data-stu-id="81040-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81040-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81040-133">JSON Representation</span></span>
<span data-ttu-id="81040-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81040-134">Here is a JSON representation of the resource.</span></span>
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



