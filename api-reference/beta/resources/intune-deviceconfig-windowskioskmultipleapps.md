---
title: Тип ресурса windowsKioskMultipleApps
description: Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a5cb62fe9423978e1c5a93423770e429127b70de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968962"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="214b4-103">Тип ресурса windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="214b4-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="214b4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="214b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="214b4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="214b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="214b4-106">Класс, используемый для определения конфигурации приложения с многорежимным режимом для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="214b4-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="214b4-107">Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="214b4-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="214b4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="214b4-108">Properties</span></span>
|<span data-ttu-id="214b4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="214b4-109">Property</span></span>|<span data-ttu-id="214b4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="214b4-110">Type</span></span>|<span data-ttu-id="214b4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="214b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="214b4-112">apps</span><span class="sxs-lookup"><span data-stu-id="214b4-112">apps</span></span>|<span data-ttu-id="214b4-113">Коллекция [виндовскиоскаппбасе](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="214b4-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="214b4-114">Это единственные приложения Магазина Windows, которые будут доступны для запуска из меню "Пуск".</span><span class="sxs-lookup"><span data-stu-id="214b4-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="214b4-115">Эта коллекция может содержать не более 128 элементов.</span><span class="sxs-lookup"><span data-stu-id="214b4-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="214b4-116">Шовтаскбар</span><span class="sxs-lookup"><span data-stu-id="214b4-116">showTaskBar</span></span>|<span data-ttu-id="214b4-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="214b4-117">Boolean</span></span>|<span data-ttu-id="214b4-118">Этот параметр позволяет администратору указать, отображается ли панель задач.</span><span class="sxs-lookup"><span data-stu-id="214b4-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="214b4-119">Алловакцесстодовнлоадсфолдер</span><span class="sxs-lookup"><span data-stu-id="214b4-119">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="214b4-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="214b4-120">Boolean</span></span>|<span data-ttu-id="214b4-121">Этот параметр разрешает доступ к папке "загрузки" в проводнике.</span><span class="sxs-lookup"><span data-stu-id="214b4-121">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="214b4-122">Дисалловдесктопаппс</span><span class="sxs-lookup"><span data-stu-id="214b4-122">disallowDesktopApps</span></span>|<span data-ttu-id="214b4-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="214b4-123">Boolean</span></span>|<span data-ttu-id="214b4-124">Этот параметр указывает, что классические приложения разрешены.</span><span class="sxs-lookup"><span data-stu-id="214b4-124">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="214b4-125">Значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="214b4-125">Default to true.</span></span>|
|<span data-ttu-id="214b4-126">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="214b4-126">startMenuLayoutXml</span></span>|<span data-ttu-id="214b4-127">Binary</span><span class="sxs-lookup"><span data-stu-id="214b4-127">Binary</span></span>|<span data-ttu-id="214b4-128">Позволяет администраторам переопределять макет запуска по умолчанию и запрещает пользователю изменять его.</span><span class="sxs-lookup"><span data-stu-id="214b4-128">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="214b4-129">Чтобы изменить макет, необходимо указать XML-файл на основе схемы изменения макета.</span><span class="sxs-lookup"><span data-stu-id="214b4-129"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="214b4-130">XML должен быть в двоичном формате.</span><span class="sxs-lookup"><span data-stu-id="214b4-130">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="214b4-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="214b4-131">Relationships</span></span>
<span data-ttu-id="214b4-132">Нет</span><span class="sxs-lookup"><span data-stu-id="214b4-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="214b4-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="214b4-133">JSON Representation</span></span>
<span data-ttu-id="214b4-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="214b4-134">Here is a JSON representation of the resource.</span></span>
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





