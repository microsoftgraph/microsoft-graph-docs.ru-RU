---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 539c1974505e248bc700a9d804d06c6f8bc4b257
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005536"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="c099b-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="c099b-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c099b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c099b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c099b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c099b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c099b-106">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="c099b-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="c099b-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c099b-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c099b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c099b-108">Properties</span></span>
|<span data-ttu-id="c099b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c099b-109">Property</span></span>|<span data-ttu-id="c099b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c099b-110">Type</span></span>|<span data-ttu-id="c099b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c099b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c099b-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="c099b-112">vpnConfigurationId</span></span>|<span data-ttu-id="c099b-113">String</span><span class="sxs-lookup"><span data-stu-id="c099b-113">String</span></span>|<span data-ttu-id="c099b-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="c099b-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c099b-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="c099b-115">Relationships</span></span>
<span data-ttu-id="c099b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c099b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c099b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c099b-117">JSON Representation</span></span>
<span data-ttu-id="c099b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c099b-118">Here is a JSON representation of the resource.</span></span>
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





