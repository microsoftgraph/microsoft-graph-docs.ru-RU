---
title: Тип ресурса Виндовскиоскактиведиректориграуп
description: Класс, используемый для определения группы каталогов Azure для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c9975317c49562efbae19c290ca0aa34792be28d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272530"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="18e98-103">Тип ресурса Виндовскиоскактиведиректориграуп</span><span class="sxs-lookup"><span data-stu-id="18e98-103">windowsKioskActiveDirectoryGroup resource type</span></span>

<span data-ttu-id="18e98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18e98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18e98-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18e98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18e98-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18e98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18e98-107">Класс, используемый для определения группы каталогов Azure для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="18e98-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="18e98-108">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="18e98-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="18e98-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="18e98-109">Properties</span></span>
|<span data-ttu-id="18e98-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="18e98-110">Property</span></span>|<span data-ttu-id="18e98-111">Тип</span><span class="sxs-lookup"><span data-stu-id="18e98-111">Type</span></span>|<span data-ttu-id="18e98-112">Описание</span><span class="sxs-lookup"><span data-stu-id="18e98-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18e98-113">groupName</span><span class="sxs-lookup"><span data-stu-id="18e98-113">groupName</span></span>|<span data-ttu-id="18e98-114">String</span><span class="sxs-lookup"><span data-stu-id="18e98-114">String</span></span>|<span data-ttu-id="18e98-115">Имя группы Active Directory, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="18e98-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="18e98-116">Связи</span><span class="sxs-lookup"><span data-stu-id="18e98-116">Relationships</span></span>
<span data-ttu-id="18e98-117">Нет</span><span class="sxs-lookup"><span data-stu-id="18e98-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18e98-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18e98-118">JSON Representation</span></span>
<span data-ttu-id="18e98-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18e98-119">Here is a JSON representation of the resource.</span></span>
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




