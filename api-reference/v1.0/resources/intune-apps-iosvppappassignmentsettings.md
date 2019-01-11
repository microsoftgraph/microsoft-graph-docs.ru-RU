---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4c9a5196be760204af682c1a7318318920284a40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886116"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="aed71-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="aed71-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="aed71-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aed71-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aed71-105">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="aed71-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="aed71-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="aed71-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aed71-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aed71-107">Properties</span></span>
|<span data-ttu-id="aed71-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="aed71-108">Property</span></span>|<span data-ttu-id="aed71-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aed71-109">Type</span></span>|<span data-ttu-id="aed71-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aed71-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aed71-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="aed71-111">useDeviceLicensing</span></span>|<span data-ttu-id="aed71-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="aed71-112">Boolean</span></span>|<span data-ttu-id="aed71-113">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="aed71-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="aed71-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="aed71-114">vpnConfigurationId</span></span>|<span data-ttu-id="aed71-115">String</span><span class="sxs-lookup"><span data-stu-id="aed71-115">String</span></span>|<span data-ttu-id="aed71-116">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="aed71-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aed71-117">Связи</span><span class="sxs-lookup"><span data-stu-id="aed71-117">Relationships</span></span>
<span data-ttu-id="aed71-118">Нет</span><span class="sxs-lookup"><span data-stu-id="aed71-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aed71-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aed71-119">JSON Representation</span></span>
<span data-ttu-id="aed71-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aed71-120">Here is a JSON representation of the resource.</span></span>
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



