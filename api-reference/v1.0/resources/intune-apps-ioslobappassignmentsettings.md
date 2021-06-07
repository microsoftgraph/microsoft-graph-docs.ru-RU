---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e364ae3ef38bd01376d937c6538ce00c39ba6172
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755156"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="dfc60-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="dfc60-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="dfc60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfc60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfc60-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfc60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfc60-106">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="dfc60-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="dfc60-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="dfc60-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dfc60-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfc60-108">Properties</span></span>
|<span data-ttu-id="dfc60-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfc60-109">Property</span></span>|<span data-ttu-id="dfc60-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dfc60-110">Type</span></span>|<span data-ttu-id="dfc60-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dfc60-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfc60-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="dfc60-112">vpnConfigurationId</span></span>|<span data-ttu-id="dfc60-113">String</span><span class="sxs-lookup"><span data-stu-id="dfc60-113">String</span></span>|<span data-ttu-id="dfc60-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="dfc60-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfc60-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="dfc60-115">Relationships</span></span>
<span data-ttu-id="dfc60-116">Нет</span><span class="sxs-lookup"><span data-stu-id="dfc60-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfc60-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfc60-117">JSON Representation</span></span>
<span data-ttu-id="dfc60-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfc60-118">Here is a JSON representation of the resource.</span></span>
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




