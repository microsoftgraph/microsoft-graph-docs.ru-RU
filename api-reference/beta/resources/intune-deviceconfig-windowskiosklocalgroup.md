---
title: Тип ресурса Виндовскиосклокалграуп
description: Класс, используемый для идентификации локальной группы для конфигурации киоска
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54a4686282e4c13f657adf010a3e0272025eb249
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789523"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="a4339-103">Тип ресурса Виндовскиосклокалграуп</span><span class="sxs-lookup"><span data-stu-id="a4339-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="a4339-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4339-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4339-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4339-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4339-106">Класс, используемый для идентификации локальной группы для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="a4339-106">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="a4339-107">НаСледуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="a4339-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a4339-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4339-108">Properties</span></span>
|<span data-ttu-id="a4339-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4339-109">Property</span></span>|<span data-ttu-id="a4339-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a4339-110">Type</span></span>|<span data-ttu-id="a4339-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a4339-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4339-112">groupName</span><span class="sxs-lookup"><span data-stu-id="a4339-112">groupName</span></span>|<span data-ttu-id="a4339-113">String</span><span class="sxs-lookup"><span data-stu-id="a4339-113">String</span></span>|<span data-ttu-id="a4339-114">Имя локальной группы, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="a4339-114">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4339-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="a4339-115">Relationships</span></span>
<span data-ttu-id="a4339-116">Нет</span><span class="sxs-lookup"><span data-stu-id="a4339-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4339-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4339-117">JSON Representation</span></span>
<span data-ttu-id="a4339-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4339-118">Here is a JSON representation of the resource.</span></span>
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





