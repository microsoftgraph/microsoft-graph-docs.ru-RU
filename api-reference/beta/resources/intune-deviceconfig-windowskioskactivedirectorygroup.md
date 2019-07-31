---
title: Тип ресурса Виндовскиоскактиведиректориграуп
description: Класс, используемый для определения группы каталогов Azure для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c64fe517fd610bad07b7a029e120c7657b834f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969025"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="6880b-103">Тип ресурса Виндовскиоскактиведиректориграуп</span><span class="sxs-lookup"><span data-stu-id="6880b-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="6880b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6880b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6880b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6880b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6880b-106">Класс, используемый для определения группы каталогов Azure для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="6880b-106">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="6880b-107">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="6880b-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6880b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6880b-108">Properties</span></span>
|<span data-ttu-id="6880b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6880b-109">Property</span></span>|<span data-ttu-id="6880b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6880b-110">Type</span></span>|<span data-ttu-id="6880b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6880b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6880b-112">groupName</span><span class="sxs-lookup"><span data-stu-id="6880b-112">groupName</span></span>|<span data-ttu-id="6880b-113">String</span><span class="sxs-lookup"><span data-stu-id="6880b-113">String</span></span>|<span data-ttu-id="6880b-114">Имя группы Active Directory, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="6880b-114">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="6880b-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="6880b-115">Relationships</span></span>
<span data-ttu-id="6880b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6880b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6880b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6880b-117">JSON Representation</span></span>
<span data-ttu-id="6880b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6880b-118">Here is a JSON representation of the resource.</span></span>
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





