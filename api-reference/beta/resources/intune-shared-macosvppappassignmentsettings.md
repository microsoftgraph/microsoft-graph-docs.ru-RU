---
title: Тип ресурса Макосвппаппассигнментсеттингс
description: Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 15db6cf48925767ab66ad98204a7283a72a294b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527382"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="ff39b-103">Тип ресурса Макосвппаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="ff39b-103">macOsVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="ff39b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ff39b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff39b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff39b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff39b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff39b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff39b-107">Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.</span><span class="sxs-lookup"><span data-stu-id="ff39b-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="ff39b-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ff39b-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff39b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff39b-109">Properties</span></span>
|<span data-ttu-id="ff39b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff39b-110">Property</span></span>|<span data-ttu-id="ff39b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ff39b-111">Type</span></span>|<span data-ttu-id="ff39b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ff39b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff39b-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="ff39b-113">useDeviceLicensing</span></span>|<span data-ttu-id="ff39b-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff39b-114">Boolean</span></span>|<span data-ttu-id="ff39b-115">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="ff39b-115">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff39b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ff39b-116">Relationships</span></span>
<span data-ttu-id="ff39b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ff39b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff39b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff39b-118">JSON Representation</span></span>
<span data-ttu-id="ff39b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff39b-119">Here is a JSON representation of the resource.</span></span>
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



