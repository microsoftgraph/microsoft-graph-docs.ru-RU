---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 883f81ab29dd2258d57753b792f0a4f1f434ed43
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360211"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="dff19-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="dff19-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="dff19-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dff19-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dff19-105">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="dff19-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="dff19-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="dff19-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dff19-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dff19-107">Properties</span></span>
|<span data-ttu-id="dff19-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dff19-108">Property</span></span>|<span data-ttu-id="dff19-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dff19-109">Type</span></span>|<span data-ttu-id="dff19-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dff19-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dff19-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="dff19-111">useDeviceLicensing</span></span>|<span data-ttu-id="dff19-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="dff19-112">Boolean</span></span>|<span data-ttu-id="dff19-113">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="dff19-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="dff19-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="dff19-114">vpnConfigurationId</span></span>|<span data-ttu-id="dff19-115">String</span><span class="sxs-lookup"><span data-stu-id="dff19-115">String</span></span>|<span data-ttu-id="dff19-116">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="dff19-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dff19-117">Связи</span><span class="sxs-lookup"><span data-stu-id="dff19-117">Relationships</span></span>
<span data-ttu-id="dff19-118">Нет</span><span class="sxs-lookup"><span data-stu-id="dff19-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dff19-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dff19-119">JSON Representation</span></span>
<span data-ttu-id="dff19-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dff19-120">Here is a JSON representation of the resource.</span></span>
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




