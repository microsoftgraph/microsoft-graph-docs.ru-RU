---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf70ac8fe90307b6445006e3f197415ef5873379
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054751"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="21f5d-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="21f5d-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="21f5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21f5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21f5d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21f5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21f5d-106">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="21f5d-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="21f5d-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="21f5d-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21f5d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="21f5d-108">Properties</span></span>
|<span data-ttu-id="21f5d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="21f5d-109">Property</span></span>|<span data-ttu-id="21f5d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="21f5d-110">Type</span></span>|<span data-ttu-id="21f5d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21f5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21f5d-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="21f5d-112">vpnConfigurationId</span></span>|<span data-ttu-id="21f5d-113">String</span><span class="sxs-lookup"><span data-stu-id="21f5d-113">String</span></span>|<span data-ttu-id="21f5d-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="21f5d-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21f5d-115">Связи</span><span class="sxs-lookup"><span data-stu-id="21f5d-115">Relationships</span></span>
<span data-ttu-id="21f5d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="21f5d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21f5d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21f5d-117">JSON Representation</span></span>
<span data-ttu-id="21f5d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21f5d-118">Here is a JSON representation of the resource.</span></span>
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









