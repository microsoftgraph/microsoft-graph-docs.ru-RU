---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1adb547aaa1a1690c43ca0ed491e205c3c2585bd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971398"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="8abd7-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="8abd7-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="8abd7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8abd7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8abd7-105">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="8abd7-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="8abd7-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8abd7-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8abd7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8abd7-107">Properties</span></span>
|<span data-ttu-id="8abd7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8abd7-108">Property</span></span>|<span data-ttu-id="8abd7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8abd7-109">Type</span></span>|<span data-ttu-id="8abd7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8abd7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8abd7-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="8abd7-111">vpnConfigurationId</span></span>|<span data-ttu-id="8abd7-112">String</span><span class="sxs-lookup"><span data-stu-id="8abd7-112">String</span></span>|<span data-ttu-id="8abd7-113">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="8abd7-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8abd7-114">Связи</span><span class="sxs-lookup"><span data-stu-id="8abd7-114">Relationships</span></span>
<span data-ttu-id="8abd7-115">Нет</span><span class="sxs-lookup"><span data-stu-id="8abd7-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8abd7-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8abd7-116">JSON Representation</span></span>
<span data-ttu-id="8abd7-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8abd7-117">Here is a JSON representation of the resource.</span></span>
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



