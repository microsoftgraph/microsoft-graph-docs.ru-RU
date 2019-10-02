---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ecd129c4b76ebe932a9b87abeda6d638b4bce23
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356268"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="e032f-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e032f-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e032f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e032f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e032f-105">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="e032f-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="e032f-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e032f-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e032f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e032f-107">Properties</span></span>
|<span data-ttu-id="e032f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e032f-108">Property</span></span>|<span data-ttu-id="e032f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e032f-109">Type</span></span>|<span data-ttu-id="e032f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e032f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e032f-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e032f-111">vpnConfigurationId</span></span>|<span data-ttu-id="e032f-112">String</span><span class="sxs-lookup"><span data-stu-id="e032f-112">String</span></span>|<span data-ttu-id="e032f-113">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="e032f-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e032f-114">Связи</span><span class="sxs-lookup"><span data-stu-id="e032f-114">Relationships</span></span>
<span data-ttu-id="e032f-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e032f-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e032f-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e032f-116">JSON Representation</span></span>
<span data-ttu-id="e032f-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e032f-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```




