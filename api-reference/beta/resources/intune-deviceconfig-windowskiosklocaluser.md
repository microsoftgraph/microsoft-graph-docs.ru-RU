---
title: Тип ресурса Виндовскиосклокалусер
description: Класс, используемый для определения локальной учетной записи для конфигурации киоска
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a84b1d3ce0a6e0f9de0bf60de314c79c0a7b329
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786378"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="eccb5-103">Тип ресурса Виндовскиосклокалусер</span><span class="sxs-lookup"><span data-stu-id="eccb5-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="eccb5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eccb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eccb5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eccb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eccb5-106">Класс, используемый для определения локальной учетной записи для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="eccb5-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="eccb5-107">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="eccb5-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eccb5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eccb5-108">Properties</span></span>
|<span data-ttu-id="eccb5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eccb5-109">Property</span></span>|<span data-ttu-id="eccb5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eccb5-110">Type</span></span>|<span data-ttu-id="eccb5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eccb5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eccb5-112">userName</span><span class="sxs-lookup"><span data-stu-id="eccb5-112">userName</span></span>|<span data-ttu-id="eccb5-113">String</span><span class="sxs-lookup"><span data-stu-id="eccb5-113">String</span></span>|<span data-ttu-id="eccb5-114">Локальный пользователь, который будет заблокирован для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="eccb5-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="eccb5-115">Связи</span><span class="sxs-lookup"><span data-stu-id="eccb5-115">Relationships</span></span>
<span data-ttu-id="eccb5-116">Нет</span><span class="sxs-lookup"><span data-stu-id="eccb5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eccb5-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eccb5-117">JSON Representation</span></span>
<span data-ttu-id="eccb5-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eccb5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```



