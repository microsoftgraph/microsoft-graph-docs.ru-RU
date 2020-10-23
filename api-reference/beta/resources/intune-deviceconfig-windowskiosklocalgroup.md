---
title: Тип ресурса Виндовскиосклокалграуп
description: Класс, используемый для идентификации локальной группы для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e7777245f9020de1db2ad3b89a41052739ccb98
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729527"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="4b982-103">Тип ресурса Виндовскиосклокалграуп</span><span class="sxs-lookup"><span data-stu-id="4b982-103">windowsKioskLocalGroup resource type</span></span>

<span data-ttu-id="4b982-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b982-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b982-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b982-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b982-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b982-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b982-107">Класс, используемый для идентификации локальной группы для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="4b982-107">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="4b982-108">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="4b982-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b982-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b982-109">Properties</span></span>
|<span data-ttu-id="4b982-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b982-110">Property</span></span>|<span data-ttu-id="4b982-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4b982-111">Type</span></span>|<span data-ttu-id="4b982-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4b982-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b982-113">groupName</span><span class="sxs-lookup"><span data-stu-id="4b982-113">groupName</span></span>|<span data-ttu-id="4b982-114">Строка</span><span class="sxs-lookup"><span data-stu-id="4b982-114">String</span></span>|<span data-ttu-id="4b982-115">Имя локальной группы, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="4b982-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b982-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4b982-116">Relationships</span></span>
<span data-ttu-id="4b982-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4b982-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b982-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b982-118">JSON Representation</span></span>
<span data-ttu-id="4b982-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b982-119">Here is a JSON representation of the resource.</span></span>
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





