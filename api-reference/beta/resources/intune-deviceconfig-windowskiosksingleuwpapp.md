---
title: Тип ресурса Виндовскиосксинглеувпапп
description: Класс, используемый для определения сведений о приложении UWP для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 276cbe4c231425540037dcc9a9e0afe977220bc0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944014"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="bd86b-103">Тип ресурса Виндовскиосксинглеувпапп</span><span class="sxs-lookup"><span data-stu-id="bd86b-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="bd86b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd86b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd86b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd86b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd86b-106">Класс, используемый для определения сведений о приложении UWP для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="bd86b-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="bd86b-107">Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd86b-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd86b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd86b-108">Properties</span></span>
|<span data-ttu-id="bd86b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd86b-109">Property</span></span>|<span data-ttu-id="bd86b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bd86b-110">Type</span></span>|<span data-ttu-id="bd86b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd86b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd86b-112">Увпапп</span><span class="sxs-lookup"><span data-stu-id="bd86b-112">uwpApp</span></span>|<span data-ttu-id="bd86b-113">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md);</span><span class="sxs-lookup"><span data-stu-id="bd86b-113">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)</span></span>|<span data-ttu-id="bd86b-114">Это единственный идентификатор пользовательской модели приложения (AUMID), который будет доступен для запуска в режиме киоска</span><span class="sxs-lookup"><span data-stu-id="bd86b-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd86b-115">Связи</span><span class="sxs-lookup"><span data-stu-id="bd86b-115">Relationships</span></span>
<span data-ttu-id="bd86b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="bd86b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd86b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd86b-117">JSON Representation</span></span>
<span data-ttu-id="bd86b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd86b-118">Here is a JSON representation of the resource.</span></span>
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




