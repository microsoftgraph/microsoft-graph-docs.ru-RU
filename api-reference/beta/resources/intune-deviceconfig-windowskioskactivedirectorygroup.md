---
title: Тип ресурса Виндовскиоскактиведиректориграуп
description: Класс, используемый для определения группы каталогов Azure для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5451050bb70cb9cdbcc50738da0eb81c659f8e6f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371028"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="56bc9-103">Тип ресурса Виндовскиоскактиведиректориграуп</span><span class="sxs-lookup"><span data-stu-id="56bc9-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="56bc9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56bc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56bc9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56bc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56bc9-106">Класс, используемый для определения группы каталогов Azure для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="56bc9-106">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="56bc9-107">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="56bc9-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56bc9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="56bc9-108">Properties</span></span>
|<span data-ttu-id="56bc9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="56bc9-109">Property</span></span>|<span data-ttu-id="56bc9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="56bc9-110">Type</span></span>|<span data-ttu-id="56bc9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="56bc9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56bc9-112">groupName</span><span class="sxs-lookup"><span data-stu-id="56bc9-112">groupName</span></span>|<span data-ttu-id="56bc9-113">String</span><span class="sxs-lookup"><span data-stu-id="56bc9-113">String</span></span>|<span data-ttu-id="56bc9-114">Имя группы Active Directory, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="56bc9-114">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="56bc9-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="56bc9-115">Relationships</span></span>
<span data-ttu-id="56bc9-116">Нет</span><span class="sxs-lookup"><span data-stu-id="56bc9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56bc9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56bc9-117">JSON Representation</span></span>
<span data-ttu-id="56bc9-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56bc9-118">Here is a JSON representation of the resource.</span></span>
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



