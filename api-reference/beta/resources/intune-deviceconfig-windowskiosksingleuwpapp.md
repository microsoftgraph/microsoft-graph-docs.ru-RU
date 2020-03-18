---
title: Тип ресурса Виндовскиосксинглеувпапп
description: Класс, используемый для определения сведений о приложении UWP для конфигурации киоска
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ae650af23985c26b00f99513ecfa4b3f691e14b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786357"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="4ff82-103">Тип ресурса Виндовскиосксинглеувпапп</span><span class="sxs-lookup"><span data-stu-id="4ff82-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="4ff82-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ff82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ff82-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ff82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ff82-106">Класс, используемый для определения сведений о приложении UWP для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="4ff82-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="4ff82-107">Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ff82-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ff82-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ff82-108">Properties</span></span>
|<span data-ttu-id="4ff82-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ff82-109">Property</span></span>|<span data-ttu-id="4ff82-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4ff82-110">Type</span></span>|<span data-ttu-id="4ff82-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4ff82-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ff82-112">увпапп</span><span class="sxs-lookup"><span data-stu-id="4ff82-112">uwpApp</span></span>|<span data-ttu-id="4ff82-113">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md);</span><span class="sxs-lookup"><span data-stu-id="4ff82-113">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)</span></span>|<span data-ttu-id="4ff82-114">Это единственный идентификатор пользовательской модели приложения (AUMID), который будет доступен для запуска в режиме киоска</span><span class="sxs-lookup"><span data-stu-id="4ff82-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ff82-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="4ff82-115">Relationships</span></span>
<span data-ttu-id="4ff82-116">Нет</span><span class="sxs-lookup"><span data-stu-id="4ff82-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ff82-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ff82-117">JSON Representation</span></span>
<span data-ttu-id="4ff82-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ff82-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```



