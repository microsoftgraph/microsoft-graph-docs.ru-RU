---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 307421c7fa5bf15628fb6bb1e10d6ba36bef5705
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531226"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="69652-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="69652-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="69652-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69652-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69652-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69652-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69652-106">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="69652-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="69652-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="69652-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="69652-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="69652-108">Properties</span></span>
|<span data-ttu-id="69652-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="69652-109">Property</span></span>|<span data-ttu-id="69652-110">Тип</span><span class="sxs-lookup"><span data-stu-id="69652-110">Type</span></span>|<span data-ttu-id="69652-111">Описание</span><span class="sxs-lookup"><span data-stu-id="69652-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69652-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="69652-112">vpnConfigurationId</span></span>|<span data-ttu-id="69652-113">String</span><span class="sxs-lookup"><span data-stu-id="69652-113">String</span></span>|<span data-ttu-id="69652-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="69652-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69652-115">Связи</span><span class="sxs-lookup"><span data-stu-id="69652-115">Relationships</span></span>
<span data-ttu-id="69652-116">Нет</span><span class="sxs-lookup"><span data-stu-id="69652-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69652-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69652-117">JSON Representation</span></span>
<span data-ttu-id="69652-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69652-118">Here is a JSON representation of the resource.</span></span>
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




