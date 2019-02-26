---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d58490e97aec48f664ab6882198e4c1da3511e8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250315"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="99938-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="99938-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="99938-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99938-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99938-105">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="99938-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="99938-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="99938-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="99938-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="99938-107">Properties</span></span>
|<span data-ttu-id="99938-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="99938-108">Property</span></span>|<span data-ttu-id="99938-109">Тип</span><span class="sxs-lookup"><span data-stu-id="99938-109">Type</span></span>|<span data-ttu-id="99938-110">Описание</span><span class="sxs-lookup"><span data-stu-id="99938-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99938-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="99938-111">vpnConfigurationId</span></span>|<span data-ttu-id="99938-112">String</span><span class="sxs-lookup"><span data-stu-id="99938-112">String</span></span>|<span data-ttu-id="99938-113">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="99938-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99938-114">Связи</span><span class="sxs-lookup"><span data-stu-id="99938-114">Relationships</span></span>
<span data-ttu-id="99938-115">Нет</span><span class="sxs-lookup"><span data-stu-id="99938-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99938-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99938-116">JSON Representation</span></span>
<span data-ttu-id="99938-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99938-117">Here is a JSON representation of the resource.</span></span>
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



