---
title: Тип ресурса Виндовскиоскактиведиректориграуп
description: Класс, используемый для определения группы каталогов Azure для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 35446a816b8fd14e6258e4f205ca4aaa3745053b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039919"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="ba05b-103">Тип ресурса Виндовскиоскактиведиректориграуп</span><span class="sxs-lookup"><span data-stu-id="ba05b-103">windowsKioskActiveDirectoryGroup resource type</span></span>

<span data-ttu-id="ba05b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba05b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba05b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba05b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba05b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba05b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba05b-107">Класс, используемый для определения группы каталогов Azure для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="ba05b-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="ba05b-108">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="ba05b-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ba05b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba05b-109">Properties</span></span>
|<span data-ttu-id="ba05b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba05b-110">Property</span></span>|<span data-ttu-id="ba05b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ba05b-111">Type</span></span>|<span data-ttu-id="ba05b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ba05b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba05b-113">groupName</span><span class="sxs-lookup"><span data-stu-id="ba05b-113">groupName</span></span>|<span data-ttu-id="ba05b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ba05b-114">String</span></span>|<span data-ttu-id="ba05b-115">Имя группы Active Directory, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="ba05b-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba05b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ba05b-116">Relationships</span></span>
<span data-ttu-id="ba05b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ba05b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba05b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba05b-118">JSON Representation</span></span>
<span data-ttu-id="ba05b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba05b-119">Here is a JSON representation of the resource.</span></span>
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






