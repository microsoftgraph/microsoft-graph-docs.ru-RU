---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cc30f875ff43b7e1b7336754cce5986f9fa702c1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231530"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="c65ca-103">Тип ресурса windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="c65ca-103">windowsKioskMultipleApps resource type</span></span>

<span data-ttu-id="c65ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c65ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c65ca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c65ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c65ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c65ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c65ca-107">Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="c65ca-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="c65ca-108">Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c65ca-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c65ca-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c65ca-109">Properties</span></span>
|<span data-ttu-id="c65ca-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c65ca-110">Property</span></span>|<span data-ttu-id="c65ca-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c65ca-111">Type</span></span>|<span data-ttu-id="c65ca-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c65ca-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c65ca-113">apps</span><span class="sxs-lookup"><span data-stu-id="c65ca-113">apps</span></span>|<span data-ttu-id="c65ca-114">Коллекция [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="c65ca-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="c65ca-115">Это единственные приложения Магазина Windows, которые будут доступны для запуска из меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="c65ca-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="c65ca-116">Эта коллекция может содержать не более 128 элементов.</span><span class="sxs-lookup"><span data-stu-id="c65ca-116">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="c65ca-117">шовтаскбар</span><span class="sxs-lookup"><span data-stu-id="c65ca-117">showTaskBar</span></span>|<span data-ttu-id="c65ca-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c65ca-118">Boolean</span></span>|<span data-ttu-id="c65ca-119">Этот параметр позволяет администратору указать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="c65ca-119">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="c65ca-120">алловакцесстодовнлоадсфолдер</span><span class="sxs-lookup"><span data-stu-id="c65ca-120">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="c65ca-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c65ca-121">Boolean</span></span>|<span data-ttu-id="c65ca-122">Этот параметр разрешает доступ к папке "загрузки" в проводнике.</span><span class="sxs-lookup"><span data-stu-id="c65ca-122">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="c65ca-123">дисалловдесктопаппс</span><span class="sxs-lookup"><span data-stu-id="c65ca-123">disallowDesktopApps</span></span>|<span data-ttu-id="c65ca-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="c65ca-124">Boolean</span></span>|<span data-ttu-id="c65ca-125">Этот параметр указывает, что классические приложения разрешены.</span><span class="sxs-lookup"><span data-stu-id="c65ca-125">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="c65ca-126">Значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="c65ca-126">Default to true.</span></span>|
|<span data-ttu-id="c65ca-127">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="c65ca-127">startMenuLayoutXml</span></span>|<span data-ttu-id="c65ca-128">Binary</span><span class="sxs-lookup"><span data-stu-id="c65ca-128">Binary</span></span>|<span data-ttu-id="c65ca-129">Позволяет администраторам переопределять макет запуска по умолчанию и запрещает пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="c65ca-129">Allows admins to override the default Start layout and prevents the user from changing it.</span></span> <span data-ttu-id="c65ca-130">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="c65ca-130">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="c65ca-131">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="c65ca-131">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c65ca-132">Связи</span><span class="sxs-lookup"><span data-stu-id="c65ca-132">Relationships</span></span>
<span data-ttu-id="c65ca-133">Нет</span><span class="sxs-lookup"><span data-stu-id="c65ca-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c65ca-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c65ca-134">JSON Representation</span></span>
<span data-ttu-id="c65ca-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c65ca-135">Here is a JSON representation of the resource.</span></span>
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




