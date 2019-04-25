---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1ff346b9ae786fdc2158a5386625f808e04c181
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523912"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="023e9-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="023e9-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="023e9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="023e9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="023e9-105">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="023e9-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="023e9-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="023e9-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="023e9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="023e9-107">Properties</span></span>
|<span data-ttu-id="023e9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="023e9-108">Property</span></span>|<span data-ttu-id="023e9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="023e9-109">Type</span></span>|<span data-ttu-id="023e9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="023e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="023e9-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="023e9-111">useDeviceLicensing</span></span>|<span data-ttu-id="023e9-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="023e9-112">Boolean</span></span>|<span data-ttu-id="023e9-113">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="023e9-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="023e9-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="023e9-114">vpnConfigurationId</span></span>|<span data-ttu-id="023e9-115">String</span><span class="sxs-lookup"><span data-stu-id="023e9-115">String</span></span>|<span data-ttu-id="023e9-116">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="023e9-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="023e9-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="023e9-117">Relationships</span></span>
<span data-ttu-id="023e9-118">Нет</span><span class="sxs-lookup"><span data-stu-id="023e9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="023e9-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="023e9-119">JSON Representation</span></span>
<span data-ttu-id="023e9-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="023e9-120">Here is a JSON representation of the resource.</span></span>
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



