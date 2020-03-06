---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: afbb1ecf250b67563f965aae6d5e7e39ebc9083d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531208"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="6e549-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6e549-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="6e549-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e549-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e549-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e549-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e549-106">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="6e549-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="6e549-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6e549-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6e549-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e549-108">Properties</span></span>
|<span data-ttu-id="6e549-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e549-109">Property</span></span>|<span data-ttu-id="6e549-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6e549-110">Type</span></span>|<span data-ttu-id="6e549-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6e549-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e549-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="6e549-112">vpnConfigurationId</span></span>|<span data-ttu-id="6e549-113">String</span><span class="sxs-lookup"><span data-stu-id="6e549-113">String</span></span>|<span data-ttu-id="6e549-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="6e549-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e549-115">Связи</span><span class="sxs-lookup"><span data-stu-id="6e549-115">Relationships</span></span>
<span data-ttu-id="6e549-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6e549-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e549-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e549-117">JSON Representation</span></span>
<span data-ttu-id="6e549-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e549-118">Here is a JSON representation of the resource.</span></span>
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




