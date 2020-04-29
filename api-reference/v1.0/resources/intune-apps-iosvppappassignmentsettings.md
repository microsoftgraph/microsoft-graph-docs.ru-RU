---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 22f41ee393dea59b6773b822daa156a6a13bb9c9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474268"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="d2cf9-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="d2cf9-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="d2cf9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2cf9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2cf9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2cf9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2cf9-106">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="d2cf9-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="d2cf9-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d2cf9-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d2cf9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2cf9-108">Properties</span></span>
|<span data-ttu-id="d2cf9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2cf9-109">Property</span></span>|<span data-ttu-id="d2cf9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d2cf9-110">Type</span></span>|<span data-ttu-id="d2cf9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d2cf9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2cf9-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="d2cf9-112">useDeviceLicensing</span></span>|<span data-ttu-id="d2cf9-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2cf9-113">Boolean</span></span>|<span data-ttu-id="d2cf9-114">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="d2cf9-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="d2cf9-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="d2cf9-115">vpnConfigurationId</span></span>|<span data-ttu-id="d2cf9-116">String</span><span class="sxs-lookup"><span data-stu-id="d2cf9-116">String</span></span>|<span data-ttu-id="d2cf9-117">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="d2cf9-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2cf9-118">Связи</span><span class="sxs-lookup"><span data-stu-id="d2cf9-118">Relationships</span></span>
<span data-ttu-id="d2cf9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d2cf9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2cf9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2cf9-120">JSON Representation</span></span>
<span data-ttu-id="d2cf9-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2cf9-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```







