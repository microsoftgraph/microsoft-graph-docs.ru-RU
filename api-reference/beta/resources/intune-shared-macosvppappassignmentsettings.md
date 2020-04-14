---
title: Тип ресурса Макосвппаппассигнментсеттингс
description: Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ddd69a94880c97ad389150eb66a429496d36335
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466259"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="8ac50-103">Тип ресурса Макосвппаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="8ac50-103">macOsVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="8ac50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ac50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ac50-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ac50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ac50-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ac50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ac50-107">Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.</span><span class="sxs-lookup"><span data-stu-id="8ac50-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="8ac50-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8ac50-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8ac50-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ac50-109">Properties</span></span>
|<span data-ttu-id="8ac50-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ac50-110">Property</span></span>|<span data-ttu-id="8ac50-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8ac50-111">Type</span></span>|<span data-ttu-id="8ac50-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8ac50-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ac50-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8ac50-113">useDeviceLicensing</span></span>|<span data-ttu-id="8ac50-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ac50-114">Boolean</span></span>|<span data-ttu-id="8ac50-115">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="8ac50-115">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ac50-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="8ac50-116">Relationships</span></span>
<span data-ttu-id="8ac50-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8ac50-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ac50-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ac50-118">JSON Representation</span></span>
<span data-ttu-id="8ac50-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ac50-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true
}
```



