---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc764c68fb6ad872fba7a7e12e3a53f92b9ba2c1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451623"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="91bb7-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="91bb7-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="91bb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91bb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91bb7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91bb7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91bb7-106">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="91bb7-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="91bb7-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="91bb7-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91bb7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="91bb7-108">Properties</span></span>
|<span data-ttu-id="91bb7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="91bb7-109">Property</span></span>|<span data-ttu-id="91bb7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="91bb7-110">Type</span></span>|<span data-ttu-id="91bb7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="91bb7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91bb7-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="91bb7-112">vpnConfigurationId</span></span>|<span data-ttu-id="91bb7-113">String</span><span class="sxs-lookup"><span data-stu-id="91bb7-113">String</span></span>|<span data-ttu-id="91bb7-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="91bb7-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91bb7-115">Связи</span><span class="sxs-lookup"><span data-stu-id="91bb7-115">Relationships</span></span>
<span data-ttu-id="91bb7-116">Нет</span><span class="sxs-lookup"><span data-stu-id="91bb7-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91bb7-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91bb7-117">JSON Representation</span></span>
<span data-ttu-id="91bb7-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91bb7-118">Here is a JSON representation of the resource.</span></span>
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







