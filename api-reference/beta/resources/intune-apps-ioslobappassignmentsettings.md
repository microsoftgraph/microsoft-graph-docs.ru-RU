---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48bac2fcc8dd8c7da65c3ee138aabaaf5649b356
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553073"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="ec072-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ec072-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="ec072-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec072-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec072-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec072-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec072-106">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="ec072-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="ec072-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ec072-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ec072-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec072-108">Properties</span></span>
|<span data-ttu-id="ec072-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec072-109">Property</span></span>|<span data-ttu-id="ec072-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ec072-110">Type</span></span>|<span data-ttu-id="ec072-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ec072-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec072-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="ec072-112">vpnConfigurationId</span></span>|<span data-ttu-id="ec072-113">String</span><span class="sxs-lookup"><span data-stu-id="ec072-113">String</span></span>|<span data-ttu-id="ec072-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="ec072-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec072-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="ec072-115">Relationships</span></span>
<span data-ttu-id="ec072-116">Нет</span><span class="sxs-lookup"><span data-stu-id="ec072-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec072-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec072-117">JSON Representation</span></span>
<span data-ttu-id="ec072-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec072-118">Here is a JSON representation of the resource.</span></span>
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





