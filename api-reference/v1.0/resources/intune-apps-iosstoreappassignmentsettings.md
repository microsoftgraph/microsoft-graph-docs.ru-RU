---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c427962565f7ecbe507e1eec8229e487885faf22
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360736"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="ee34a-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ee34a-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="ee34a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee34a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee34a-105">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="ee34a-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="ee34a-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ee34a-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee34a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee34a-107">Properties</span></span>
|<span data-ttu-id="ee34a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee34a-108">Property</span></span>|<span data-ttu-id="ee34a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ee34a-109">Type</span></span>|<span data-ttu-id="ee34a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ee34a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee34a-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="ee34a-111">vpnConfigurationId</span></span>|<span data-ttu-id="ee34a-112">String</span><span class="sxs-lookup"><span data-stu-id="ee34a-112">String</span></span>|<span data-ttu-id="ee34a-113">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="ee34a-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee34a-114">Связи</span><span class="sxs-lookup"><span data-stu-id="ee34a-114">Relationships</span></span>
<span data-ttu-id="ee34a-115">Нет</span><span class="sxs-lookup"><span data-stu-id="ee34a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee34a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee34a-116">JSON Representation</span></span>
<span data-ttu-id="ee34a-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee34a-117">Here is a JSON representation of the resource.</span></span>
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




