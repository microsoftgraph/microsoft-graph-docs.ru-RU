---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
ms.openlocfilehash: ec26e3367aabedfca009db003468164c468e9ecd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025577"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="e4b9a-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e4b9a-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e4b9a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e4b9a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4b9a-105">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="e4b9a-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="e4b9a-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e4b9a-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e4b9a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4b9a-107">Properties</span></span>
|<span data-ttu-id="e4b9a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4b9a-108">Property</span></span>|<span data-ttu-id="e4b9a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e4b9a-109">Type</span></span>|<span data-ttu-id="e4b9a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e4b9a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4b9a-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e4b9a-111">vpnConfigurationId</span></span>|<span data-ttu-id="e4b9a-112">String</span><span class="sxs-lookup"><span data-stu-id="e4b9a-112">String</span></span>|<span data-ttu-id="e4b9a-113">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="e4b9a-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4b9a-114">Связи</span><span class="sxs-lookup"><span data-stu-id="e4b9a-114">Relationships</span></span>
<span data-ttu-id="e4b9a-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e4b9a-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4b9a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4b9a-116">JSON Representation</span></span>
<span data-ttu-id="e4b9a-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4b9a-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



