---
title: Тип ресурса macOsVppAppAssignmentSettings
description: Содержит свойства, используемые для назначения Mac VPP мобильного приложения в группу.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0927277b11416da001ad826200bf4ec841341118
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431762"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="d35ea-103">Тип ресурса macOsVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="d35ea-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d35ea-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d35ea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d35ea-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d35ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d35ea-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d35ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d35ea-107">Содержит свойства, используемые для назначения Mac VPP мобильного приложения в группу.</span><span class="sxs-lookup"><span data-stu-id="d35ea-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="d35ea-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d35ea-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d35ea-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d35ea-109">Properties</span></span>
|<span data-ttu-id="d35ea-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d35ea-110">Property</span></span>|<span data-ttu-id="d35ea-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d35ea-111">Type</span></span>|<span data-ttu-id="d35ea-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d35ea-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d35ea-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="d35ea-113">useDeviceLicensing</span></span>|<span data-ttu-id="d35ea-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d35ea-114">Boolean</span></span>|<span data-ttu-id="d35ea-115">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="d35ea-115">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d35ea-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="d35ea-116">Relationships</span></span>
<span data-ttu-id="d35ea-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d35ea-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d35ea-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d35ea-118">JSON Representation</span></span>
<span data-ttu-id="d35ea-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d35ea-119">Here is a JSON representation of the resource.</span></span>
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




