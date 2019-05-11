---
title: Тип ресурса Виндовскиосклокалграуп
description: Класс, используемый для идентификации локальной группы для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ab9875759c8610f976e4aaa7cc5fc8733b20ee0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943860"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="3f319-103">Тип ресурса Виндовскиосклокалграуп</span><span class="sxs-lookup"><span data-stu-id="3f319-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="3f319-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f319-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f319-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f319-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f319-106">Класс, используемый для идентификации локальной группы для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="3f319-106">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="3f319-107">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="3f319-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f319-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f319-108">Properties</span></span>
|<span data-ttu-id="3f319-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f319-109">Property</span></span>|<span data-ttu-id="3f319-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3f319-110">Type</span></span>|<span data-ttu-id="3f319-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3f319-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f319-112">groupName</span><span class="sxs-lookup"><span data-stu-id="3f319-112">groupName</span></span>|<span data-ttu-id="3f319-113">Строка</span><span class="sxs-lookup"><span data-stu-id="3f319-113">String</span></span>|<span data-ttu-id="3f319-114">Имя локальной группы, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="3f319-114">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f319-115">Связи</span><span class="sxs-lookup"><span data-stu-id="3f319-115">Relationships</span></span>
<span data-ttu-id="3f319-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3f319-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f319-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f319-117">JSON Representation</span></span>
<span data-ttu-id="3f319-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f319-118">Here is a JSON representation of the resource.</span></span>
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




