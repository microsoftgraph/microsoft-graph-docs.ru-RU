---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef89526a928ed2f8edb9a8c1ce26f199bdfdec77
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950419"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="27ff9-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="27ff9-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="27ff9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27ff9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27ff9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27ff9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27ff9-106">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="27ff9-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="27ff9-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="27ff9-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27ff9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="27ff9-108">Properties</span></span>
|<span data-ttu-id="27ff9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="27ff9-109">Property</span></span>|<span data-ttu-id="27ff9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="27ff9-110">Type</span></span>|<span data-ttu-id="27ff9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="27ff9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27ff9-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="27ff9-112">vpnConfigurationId</span></span>|<span data-ttu-id="27ff9-113">String</span><span class="sxs-lookup"><span data-stu-id="27ff9-113">String</span></span>|<span data-ttu-id="27ff9-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="27ff9-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27ff9-115">Связи</span><span class="sxs-lookup"><span data-stu-id="27ff9-115">Relationships</span></span>
<span data-ttu-id="27ff9-116">Нет</span><span class="sxs-lookup"><span data-stu-id="27ff9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27ff9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27ff9-117">JSON Representation</span></span>
<span data-ttu-id="27ff9-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27ff9-118">Here is a JSON representation of the resource.</span></span>
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




