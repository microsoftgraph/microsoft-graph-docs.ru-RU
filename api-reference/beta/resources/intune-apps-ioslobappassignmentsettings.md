---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a91d6b1fcbc5fb8affdfadf9a60993f630a8e56c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950503"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="e8a6e-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e8a6e-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e8a6e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8a6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8a6e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8a6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8a6e-106">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="e8a6e-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="e8a6e-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e8a6e-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8a6e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8a6e-108">Properties</span></span>
|<span data-ttu-id="e8a6e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8a6e-109">Property</span></span>|<span data-ttu-id="e8a6e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e8a6e-110">Type</span></span>|<span data-ttu-id="e8a6e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e8a6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8a6e-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e8a6e-112">vpnConfigurationId</span></span>|<span data-ttu-id="e8a6e-113">String</span><span class="sxs-lookup"><span data-stu-id="e8a6e-113">String</span></span>|<span data-ttu-id="e8a6e-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="e8a6e-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8a6e-115">Связи</span><span class="sxs-lookup"><span data-stu-id="e8a6e-115">Relationships</span></span>
<span data-ttu-id="e8a6e-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e8a6e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8a6e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8a6e-117">JSON Representation</span></span>
<span data-ttu-id="e8a6e-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8a6e-118">Here is a JSON representation of the resource.</span></span>
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




