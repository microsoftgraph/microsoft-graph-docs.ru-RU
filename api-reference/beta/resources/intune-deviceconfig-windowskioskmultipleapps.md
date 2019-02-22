---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения с многоРежимным режимом для конфигурации киоска
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2d2ff38e3b07920f474d9e3894bbd1f8855e277
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162022"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="91e12-103">Тип ресурса windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="91e12-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="91e12-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91e12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91e12-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91e12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91e12-106">Класс, используемый для определения конфигурации приложения с многоРежимным режимом для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="91e12-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="91e12-107">НаСледуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91e12-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91e12-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="91e12-108">Properties</span></span>
|<span data-ttu-id="91e12-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="91e12-109">Property</span></span>|<span data-ttu-id="91e12-110">Тип</span><span class="sxs-lookup"><span data-stu-id="91e12-110">Type</span></span>|<span data-ttu-id="91e12-111">Описание</span><span class="sxs-lookup"><span data-stu-id="91e12-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91e12-112">apps</span><span class="sxs-lookup"><span data-stu-id="91e12-112">apps</span></span>|<span data-ttu-id="91e12-113">Коллекция [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="91e12-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="91e12-114">Это единственные приложения Магазина Windows, которые будут доступны для запуска из меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="91e12-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="91e12-115">Эта коллекция может содержать не более 128 элементов.</span><span class="sxs-lookup"><span data-stu-id="91e12-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="91e12-116">Шовтаскбар</span><span class="sxs-lookup"><span data-stu-id="91e12-116">showTaskBar</span></span>|<span data-ttu-id="91e12-117">Логический</span><span class="sxs-lookup"><span data-stu-id="91e12-117">Boolean</span></span>|<span data-ttu-id="91e12-118">Этот параметр позволяет администратору указать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="91e12-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="91e12-119">Дисалловдесктопаппс</span><span class="sxs-lookup"><span data-stu-id="91e12-119">disallowDesktopApps</span></span>|<span data-ttu-id="91e12-120">Логический</span><span class="sxs-lookup"><span data-stu-id="91e12-120">Boolean</span></span>|<span data-ttu-id="91e12-121">Этот параметр указывает, что классические приложения разрешены.</span><span class="sxs-lookup"><span data-stu-id="91e12-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="91e12-122">Значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="91e12-122">Default to true.</span></span>|
|<span data-ttu-id="91e12-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="91e12-123">startMenuLayoutXml</span></span>|<span data-ttu-id="91e12-124">Binary</span><span class="sxs-lookup"><span data-stu-id="91e12-124">Binary</span></span>|<span data-ttu-id="91e12-125">Позволяет администраторам переопределять макет запуска по умолчанию и запрещает пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="91e12-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="91e12-126">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="91e12-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="91e12-127">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="91e12-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91e12-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="91e12-128">Relationships</span></span>
<span data-ttu-id="91e12-129">Нет</span><span class="sxs-lookup"><span data-stu-id="91e12-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91e12-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91e12-130">JSON Representation</span></span>
<span data-ttu-id="91e12-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91e12-131">Here is a JSON representation of the resource.</span></span>
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




