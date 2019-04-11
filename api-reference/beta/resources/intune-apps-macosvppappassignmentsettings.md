---
title: Тип ресурса Макосвппаппассигнментсеттингс
description: Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b55e203e58197d4b3e29d4a6a8567769d9196e0c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803229"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="2395b-103">Тип ресурса Макосвппаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="2395b-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="2395b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2395b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2395b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2395b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2395b-106">Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.</span><span class="sxs-lookup"><span data-stu-id="2395b-106">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="2395b-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2395b-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2395b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2395b-108">Properties</span></span>
|<span data-ttu-id="2395b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2395b-109">Property</span></span>|<span data-ttu-id="2395b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2395b-110">Type</span></span>|<span data-ttu-id="2395b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2395b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2395b-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="2395b-112">useDeviceLicensing</span></span>|<span data-ttu-id="2395b-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="2395b-113">Boolean</span></span>|<span data-ttu-id="2395b-114">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="2395b-114">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2395b-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="2395b-115">Relationships</span></span>
<span data-ttu-id="2395b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="2395b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2395b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2395b-117">JSON Representation</span></span>
<span data-ttu-id="2395b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2395b-118">Here is a JSON representation of the resource.</span></span>
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





