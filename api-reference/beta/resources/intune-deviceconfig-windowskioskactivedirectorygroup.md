---
title: Тип ресурса Виндовскиоскактиведиректориграуп
description: Класс, используемый для определения группы каталогов Azure для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4c0810cfeda4f620f6733a5b824cde8d0234f38
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943965"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="eb7aa-103">Тип ресурса Виндовскиоскактиведиректориграуп</span><span class="sxs-lookup"><span data-stu-id="eb7aa-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="eb7aa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb7aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb7aa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb7aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb7aa-106">Класс, используемый для определения группы каталогов Azure для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="eb7aa-106">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="eb7aa-107">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="eb7aa-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb7aa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb7aa-108">Properties</span></span>
|<span data-ttu-id="eb7aa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb7aa-109">Property</span></span>|<span data-ttu-id="eb7aa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eb7aa-110">Type</span></span>|<span data-ttu-id="eb7aa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eb7aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb7aa-112">groupName</span><span class="sxs-lookup"><span data-stu-id="eb7aa-112">groupName</span></span>|<span data-ttu-id="eb7aa-113">Строка</span><span class="sxs-lookup"><span data-stu-id="eb7aa-113">String</span></span>|<span data-ttu-id="eb7aa-114">Имя группы Active Directory, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="eb7aa-114">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb7aa-115">Связи</span><span class="sxs-lookup"><span data-stu-id="eb7aa-115">Relationships</span></span>
<span data-ttu-id="eb7aa-116">Нет</span><span class="sxs-lookup"><span data-stu-id="eb7aa-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb7aa-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb7aa-117">JSON Representation</span></span>
<span data-ttu-id="eb7aa-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb7aa-118">Here is a JSON representation of the resource.</span></span>
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




