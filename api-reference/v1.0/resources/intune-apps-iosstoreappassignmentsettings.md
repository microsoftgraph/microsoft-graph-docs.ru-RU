---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0b47c71f151e0cb83f9e682789fcde3a7b69ae4b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756073"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="92c1d-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="92c1d-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="92c1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92c1d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92c1d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92c1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92c1d-106">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="92c1d-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="92c1d-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="92c1d-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92c1d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="92c1d-108">Properties</span></span>
|<span data-ttu-id="92c1d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="92c1d-109">Property</span></span>|<span data-ttu-id="92c1d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="92c1d-110">Type</span></span>|<span data-ttu-id="92c1d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="92c1d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92c1d-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="92c1d-112">vpnConfigurationId</span></span>|<span data-ttu-id="92c1d-113">String</span><span class="sxs-lookup"><span data-stu-id="92c1d-113">String</span></span>|<span data-ttu-id="92c1d-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="92c1d-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92c1d-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="92c1d-115">Relationships</span></span>
<span data-ttu-id="92c1d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="92c1d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92c1d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92c1d-117">JSON Representation</span></span>
<span data-ttu-id="92c1d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92c1d-118">Here is a JSON representation of the resource.</span></span>
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




