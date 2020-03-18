---
title: Тип ресурса Макосвппаппассигнментсеттингс
description: Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1b4ecb5f2dbbca6d3f9fe8eebc3771347739e77
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769068"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="9dac0-103">Тип ресурса Макосвппаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="9dac0-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="9dac0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dac0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9dac0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9dac0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dac0-106">Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.</span><span class="sxs-lookup"><span data-stu-id="9dac0-106">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="9dac0-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9dac0-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9dac0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9dac0-108">Properties</span></span>
|<span data-ttu-id="9dac0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dac0-109">Property</span></span>|<span data-ttu-id="9dac0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9dac0-110">Type</span></span>|<span data-ttu-id="9dac0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9dac0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dac0-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="9dac0-112">useDeviceLicensing</span></span>|<span data-ttu-id="9dac0-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dac0-113">Boolean</span></span>|<span data-ttu-id="9dac0-114">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="9dac0-114">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dac0-115">Связи</span><span class="sxs-lookup"><span data-stu-id="9dac0-115">Relationships</span></span>
<span data-ttu-id="9dac0-116">Нет</span><span class="sxs-lookup"><span data-stu-id="9dac0-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dac0-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9dac0-117">JSON Representation</span></span>
<span data-ttu-id="9dac0-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dac0-118">Here is a JSON representation of the resource.</span></span>
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



