---
title: Тип ресурса Макосвппаппассигнментсеттингс
description: Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0c7b76b562a58e832c97cc03fb475a023247ee5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950321"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="fdeed-103">Тип ресурса Макосвппаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="fdeed-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="fdeed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdeed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdeed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdeed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdeed-106">Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.</span><span class="sxs-lookup"><span data-stu-id="fdeed-106">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="fdeed-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="fdeed-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fdeed-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdeed-108">Properties</span></span>
|<span data-ttu-id="fdeed-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdeed-109">Property</span></span>|<span data-ttu-id="fdeed-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fdeed-110">Type</span></span>|<span data-ttu-id="fdeed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fdeed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdeed-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="fdeed-112">useDeviceLicensing</span></span>|<span data-ttu-id="fdeed-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdeed-113">Boolean</span></span>|<span data-ttu-id="fdeed-114">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="fdeed-114">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdeed-115">Связи</span><span class="sxs-lookup"><span data-stu-id="fdeed-115">Relationships</span></span>
<span data-ttu-id="fdeed-116">Нет</span><span class="sxs-lookup"><span data-stu-id="fdeed-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdeed-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdeed-117">JSON Representation</span></span>
<span data-ttu-id="fdeed-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdeed-118">Here is a JSON representation of the resource.</span></span>
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




