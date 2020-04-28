---
title: Тип ресурса Виндовскиоскактиведиректориграуп
description: Класс, используемый для определения группы каталогов Azure для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c46d3b44c28c7f07b5d0478acc3f82547b3819ee
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466862"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="4dfb4-103">Тип ресурса Виндовскиоскактиведиректориграуп</span><span class="sxs-lookup"><span data-stu-id="4dfb4-103">windowsKioskActiveDirectoryGroup resource type</span></span>

<span data-ttu-id="4dfb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dfb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4dfb4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dfb4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dfb4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dfb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dfb4-107">Класс, используемый для определения группы каталогов Azure для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="4dfb4-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="4dfb4-108">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="4dfb4-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4dfb4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dfb4-109">Properties</span></span>
|<span data-ttu-id="4dfb4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dfb4-110">Property</span></span>|<span data-ttu-id="4dfb4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4dfb4-111">Type</span></span>|<span data-ttu-id="4dfb4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4dfb4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dfb4-113">groupName</span><span class="sxs-lookup"><span data-stu-id="4dfb4-113">groupName</span></span>|<span data-ttu-id="4dfb4-114">String</span><span class="sxs-lookup"><span data-stu-id="4dfb4-114">String</span></span>|<span data-ttu-id="4dfb4-115">Имя группы Active Directory, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="4dfb4-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dfb4-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4dfb4-116">Relationships</span></span>
<span data-ttu-id="4dfb4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4dfb4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dfb4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dfb4-118">JSON Representation</span></span>
<span data-ttu-id="4dfb4-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dfb4-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```



