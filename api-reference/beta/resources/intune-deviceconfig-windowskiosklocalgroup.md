---
title: Тип ресурса Виндовскиосклокалграуп
description: Класс, используемый для идентификации локальной группы для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 50ebc28381d1453fe7f178f9ede846a60f2dcf0f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226652"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="bfc4a-103">Тип ресурса Виндовскиосклокалграуп</span><span class="sxs-lookup"><span data-stu-id="bfc4a-103">windowsKioskLocalGroup resource type</span></span>

<span data-ttu-id="bfc4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfc4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bfc4a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfc4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfc4a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfc4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfc4a-107">Класс, используемый для идентификации локальной группы для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="bfc4a-107">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="bfc4a-108">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="bfc4a-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bfc4a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfc4a-109">Properties</span></span>
|<span data-ttu-id="bfc4a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfc4a-110">Property</span></span>|<span data-ttu-id="bfc4a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bfc4a-111">Type</span></span>|<span data-ttu-id="bfc4a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bfc4a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfc4a-113">groupName</span><span class="sxs-lookup"><span data-stu-id="bfc4a-113">groupName</span></span>|<span data-ttu-id="bfc4a-114">String</span><span class="sxs-lookup"><span data-stu-id="bfc4a-114">String</span></span>|<span data-ttu-id="bfc4a-115">Имя локальной группы, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="bfc4a-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfc4a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="bfc4a-116">Relationships</span></span>
<span data-ttu-id="bfc4a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="bfc4a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfc4a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfc4a-118">JSON Representation</span></span>
<span data-ttu-id="bfc4a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfc4a-119">Here is a JSON representation of the resource.</span></span>
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




