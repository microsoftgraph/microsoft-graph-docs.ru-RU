---
title: Тип ресурса Виндовскиосксинглеувпапп
description: Класс, используемый для определения сведений о приложении UWP для конфигурации киоска
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0a3b56c7bc9856b98708b63c247479e6ccf9c9b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571160"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="0b6c4-103">Тип ресурса Виндовскиосксинглеувпапп</span><span class="sxs-lookup"><span data-stu-id="0b6c4-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="0b6c4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b6c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b6c4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b6c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b6c4-106">Класс, используемый для определения сведений о приложении UWP для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="0b6c4-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="0b6c4-107">НаСледуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b6c4-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0b6c4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b6c4-108">Properties</span></span>
|<span data-ttu-id="0b6c4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b6c4-109">Property</span></span>|<span data-ttu-id="0b6c4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0b6c4-110">Type</span></span>|<span data-ttu-id="0b6c4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0b6c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b6c4-112">Увпапп</span><span class="sxs-lookup"><span data-stu-id="0b6c4-112">uwpApp</span></span>|<span data-ttu-id="0b6c4-113">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md);</span><span class="sxs-lookup"><span data-stu-id="0b6c4-113">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)</span></span>|<span data-ttu-id="0b6c4-114">Это единственный идентификатор пользовательской модели приложения (AUMID), который будет доступен для запуска в режиме киоска</span><span class="sxs-lookup"><span data-stu-id="0b6c4-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b6c4-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="0b6c4-115">Relationships</span></span>
<span data-ttu-id="0b6c4-116">Нет</span><span class="sxs-lookup"><span data-stu-id="0b6c4-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b6c4-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b6c4-117">JSON Representation</span></span>
<span data-ttu-id="0b6c4-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b6c4-118">Here is a JSON representation of the resource.</span></span>
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




