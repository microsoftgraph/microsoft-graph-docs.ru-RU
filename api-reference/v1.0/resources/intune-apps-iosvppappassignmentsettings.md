---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d35cd60b1e616f38b8c4c792f7bd766f550b62aa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029122"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="e73b0-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e73b0-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e73b0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e73b0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e73b0-105">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="e73b0-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="e73b0-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e73b0-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e73b0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e73b0-107">Properties</span></span>
|<span data-ttu-id="e73b0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e73b0-108">Property</span></span>|<span data-ttu-id="e73b0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e73b0-109">Type</span></span>|<span data-ttu-id="e73b0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e73b0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e73b0-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e73b0-111">useDeviceLicensing</span></span>|<span data-ttu-id="e73b0-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73b0-112">Boolean</span></span>|<span data-ttu-id="e73b0-113">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="e73b0-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="e73b0-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e73b0-114">vpnConfigurationId</span></span>|<span data-ttu-id="e73b0-115">String</span><span class="sxs-lookup"><span data-stu-id="e73b0-115">String</span></span>|<span data-ttu-id="e73b0-116">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="e73b0-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e73b0-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="e73b0-117">Relationships</span></span>
<span data-ttu-id="e73b0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e73b0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e73b0-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e73b0-119">JSON Representation</span></span>
<span data-ttu-id="e73b0-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e73b0-120">Here is a JSON representation of the resource.</span></span>
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



