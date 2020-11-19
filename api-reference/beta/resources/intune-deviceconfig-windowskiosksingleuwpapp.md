---
title: Тип ресурса Виндовскиосксинглеувпапп
description: Класс, используемый для определения сведений о приложении UWP для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 957670eec5e73f56dff2518936e98d0dfb0fbc33
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268169"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="06e57-103">Тип ресурса Виндовскиосксинглеувпапп</span><span class="sxs-lookup"><span data-stu-id="06e57-103">windowsKioskSingleUWPApp resource type</span></span>

<span data-ttu-id="06e57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06e57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06e57-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06e57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06e57-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06e57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06e57-107">Класс, используемый для определения сведений о приложении UWP для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="06e57-107">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="06e57-108">Наследуется от [виндовскиоскаппконфигуратион](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06e57-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="06e57-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="06e57-109">Properties</span></span>
|<span data-ttu-id="06e57-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="06e57-110">Property</span></span>|<span data-ttu-id="06e57-111">Тип</span><span class="sxs-lookup"><span data-stu-id="06e57-111">Type</span></span>|<span data-ttu-id="06e57-112">Описание</span><span class="sxs-lookup"><span data-stu-id="06e57-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06e57-113">увпапп</span><span class="sxs-lookup"><span data-stu-id="06e57-113">uwpApp</span></span>|<span data-ttu-id="06e57-114">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md);</span><span class="sxs-lookup"><span data-stu-id="06e57-114">[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)</span></span>|<span data-ttu-id="06e57-115">Это единственный идентификатор пользовательской модели приложения (AUMID), который будет доступен для запуска в режиме киоска</span><span class="sxs-lookup"><span data-stu-id="06e57-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="06e57-116">Связи</span><span class="sxs-lookup"><span data-stu-id="06e57-116">Relationships</span></span>
<span data-ttu-id="06e57-117">Нет</span><span class="sxs-lookup"><span data-stu-id="06e57-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06e57-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06e57-118">JSON Representation</span></span>
<span data-ttu-id="06e57-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06e57-119">Here is a JSON representation of the resource.</span></span>
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




