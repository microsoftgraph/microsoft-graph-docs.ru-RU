---
title: Тип ресурса Виндовскиосклокалграуп
description: Класс, используемый для идентификации локальной группы для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7385fd0990fc7ac135a3ea9ba318e06571ecdd6d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444096"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="95dc0-103">Тип ресурса Виндовскиосклокалграуп</span><span class="sxs-lookup"><span data-stu-id="95dc0-103">windowsKioskLocalGroup resource type</span></span>

<span data-ttu-id="95dc0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95dc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95dc0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95dc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95dc0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95dc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95dc0-107">Класс, используемый для идентификации локальной группы для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="95dc0-107">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="95dc0-108">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="95dc0-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="95dc0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="95dc0-109">Properties</span></span>
|<span data-ttu-id="95dc0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="95dc0-110">Property</span></span>|<span data-ttu-id="95dc0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="95dc0-111">Type</span></span>|<span data-ttu-id="95dc0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="95dc0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95dc0-113">groupName</span><span class="sxs-lookup"><span data-stu-id="95dc0-113">groupName</span></span>|<span data-ttu-id="95dc0-114">String</span><span class="sxs-lookup"><span data-stu-id="95dc0-114">String</span></span>|<span data-ttu-id="95dc0-115">Имя локальной группы, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="95dc0-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="95dc0-116">Связи</span><span class="sxs-lookup"><span data-stu-id="95dc0-116">Relationships</span></span>
<span data-ttu-id="95dc0-117">Нет</span><span class="sxs-lookup"><span data-stu-id="95dc0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95dc0-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95dc0-118">JSON Representation</span></span>
<span data-ttu-id="95dc0-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95dc0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```



