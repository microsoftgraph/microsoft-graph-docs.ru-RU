---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1148336c5fa868cea90f223e66bf3868775647c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423680"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="91d30-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="91d30-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="91d30-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91d30-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="91d30-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91d30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91d30-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91d30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91d30-107">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="91d30-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="91d30-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="91d30-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91d30-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="91d30-109">Properties</span></span>
|<span data-ttu-id="91d30-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="91d30-110">Property</span></span>|<span data-ttu-id="91d30-111">Тип</span><span class="sxs-lookup"><span data-stu-id="91d30-111">Type</span></span>|<span data-ttu-id="91d30-112">Описание</span><span class="sxs-lookup"><span data-stu-id="91d30-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91d30-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="91d30-113">useDeviceLicensing</span></span>|<span data-ttu-id="91d30-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="91d30-114">Boolean</span></span>|<span data-ttu-id="91d30-115">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="91d30-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="91d30-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="91d30-116">vpnConfigurationId</span></span>|<span data-ttu-id="91d30-117">String</span><span class="sxs-lookup"><span data-stu-id="91d30-117">String</span></span>|<span data-ttu-id="91d30-118">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="91d30-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91d30-119">Связи</span><span class="sxs-lookup"><span data-stu-id="91d30-119">Relationships</span></span>
<span data-ttu-id="91d30-120">Нет</span><span class="sxs-lookup"><span data-stu-id="91d30-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91d30-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91d30-121">JSON Representation</span></span>
<span data-ttu-id="91d30-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91d30-122">Here is a JSON representation of the resource.</span></span>
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




