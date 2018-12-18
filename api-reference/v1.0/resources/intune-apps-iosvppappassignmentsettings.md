---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: tfitzmac
ms.openlocfilehash: 65a143c1f6cc9eed4dfdc6dabeb6f9379517277c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310250"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="c5a11-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="c5a11-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c5a11-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5a11-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5a11-105">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="c5a11-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="c5a11-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c5a11-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5a11-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5a11-107">Properties</span></span>
|<span data-ttu-id="c5a11-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5a11-108">Property</span></span>|<span data-ttu-id="c5a11-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c5a11-109">Type</span></span>|<span data-ttu-id="c5a11-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c5a11-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a11-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="c5a11-111">useDeviceLicensing</span></span>|<span data-ttu-id="c5a11-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a11-112">Boolean</span></span>|<span data-ttu-id="c5a11-113">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="c5a11-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="c5a11-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="c5a11-114">vpnConfigurationId</span></span>|<span data-ttu-id="c5a11-115">String</span><span class="sxs-lookup"><span data-stu-id="c5a11-115">String</span></span>|<span data-ttu-id="c5a11-116">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="c5a11-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5a11-117">Связи</span><span class="sxs-lookup"><span data-stu-id="c5a11-117">Relationships</span></span>
<span data-ttu-id="c5a11-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c5a11-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c5a11-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5a11-119">JSON Representation</span></span>
<span data-ttu-id="c5a11-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5a11-120">Here is a JSON representation of the resource.</span></span>
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



