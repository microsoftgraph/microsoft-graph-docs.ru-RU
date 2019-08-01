---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8cb033283c163a30dbedf7088001025c327dbae6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029171"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="ded78-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ded78-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="ded78-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ded78-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ded78-105">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="ded78-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="ded78-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ded78-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ded78-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ded78-107">Properties</span></span>
|<span data-ttu-id="ded78-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ded78-108">Property</span></span>|<span data-ttu-id="ded78-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ded78-109">Type</span></span>|<span data-ttu-id="ded78-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ded78-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ded78-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="ded78-111">vpnConfigurationId</span></span>|<span data-ttu-id="ded78-112">String</span><span class="sxs-lookup"><span data-stu-id="ded78-112">String</span></span>|<span data-ttu-id="ded78-113">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="ded78-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ded78-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="ded78-114">Relationships</span></span>
<span data-ttu-id="ded78-115">Нет</span><span class="sxs-lookup"><span data-stu-id="ded78-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ded78-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ded78-116">JSON Representation</span></span>
<span data-ttu-id="ded78-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ded78-117">Here is a JSON representation of the resource.</span></span>
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



