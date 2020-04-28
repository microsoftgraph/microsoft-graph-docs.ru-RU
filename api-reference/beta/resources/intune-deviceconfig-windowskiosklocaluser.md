---
title: Тип ресурса Виндовскиосклокалусер
description: Класс, используемый для определения локальной учетной записи для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f614a1bc8a71515fb3b94cdba9ce8ce5548c79f7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460023"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="09438-103">Тип ресурса Виндовскиосклокалусер</span><span class="sxs-lookup"><span data-stu-id="09438-103">windowsKioskLocalUser resource type</span></span>

<span data-ttu-id="09438-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09438-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09438-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09438-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09438-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09438-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09438-107">Класс, используемый для определения локальной учетной записи для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="09438-107">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="09438-108">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="09438-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09438-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="09438-109">Properties</span></span>
|<span data-ttu-id="09438-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="09438-110">Property</span></span>|<span data-ttu-id="09438-111">Тип</span><span class="sxs-lookup"><span data-stu-id="09438-111">Type</span></span>|<span data-ttu-id="09438-112">Описание</span><span class="sxs-lookup"><span data-stu-id="09438-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09438-113">userName</span><span class="sxs-lookup"><span data-stu-id="09438-113">userName</span></span>|<span data-ttu-id="09438-114">String</span><span class="sxs-lookup"><span data-stu-id="09438-114">String</span></span>|<span data-ttu-id="09438-115">Локальный пользователь, который будет заблокирован для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="09438-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="09438-116">Связи</span><span class="sxs-lookup"><span data-stu-id="09438-116">Relationships</span></span>
<span data-ttu-id="09438-117">Нет</span><span class="sxs-lookup"><span data-stu-id="09438-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09438-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09438-118">JSON Representation</span></span>
<span data-ttu-id="09438-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09438-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```



