---
title: Тип ресурса Макосвппаппассигнментсеттингс
description: Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a8b63edf4e470e3418693fe299dc07a22175e09
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989149"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="ea5db-103">Тип ресурса Макосвппаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="ea5db-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="ea5db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea5db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea5db-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea5db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea5db-106">Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.</span><span class="sxs-lookup"><span data-stu-id="ea5db-106">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="ea5db-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ea5db-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea5db-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea5db-108">Properties</span></span>
|<span data-ttu-id="ea5db-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea5db-109">Property</span></span>|<span data-ttu-id="ea5db-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ea5db-110">Type</span></span>|<span data-ttu-id="ea5db-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea5db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea5db-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="ea5db-112">useDeviceLicensing</span></span>|<span data-ttu-id="ea5db-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea5db-113">Boolean</span></span>|<span data-ttu-id="ea5db-114">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="ea5db-114">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea5db-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="ea5db-115">Relationships</span></span>
<span data-ttu-id="ea5db-116">Нет</span><span class="sxs-lookup"><span data-stu-id="ea5db-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea5db-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea5db-117">JSON Representation</span></span>
<span data-ttu-id="ea5db-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea5db-118">Here is a JSON representation of the resource.</span></span>
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





