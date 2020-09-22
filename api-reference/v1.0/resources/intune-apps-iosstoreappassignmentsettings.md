---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 111f7a1f1a5b48e46e00ee98f95eaa7397bf6ab4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075037"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="866d3-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="866d3-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="866d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="866d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="866d3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="866d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="866d3-106">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="866d3-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="866d3-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="866d3-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="866d3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="866d3-108">Properties</span></span>
|<span data-ttu-id="866d3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="866d3-109">Property</span></span>|<span data-ttu-id="866d3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="866d3-110">Type</span></span>|<span data-ttu-id="866d3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="866d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="866d3-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="866d3-112">vpnConfigurationId</span></span>|<span data-ttu-id="866d3-113">String</span><span class="sxs-lookup"><span data-stu-id="866d3-113">String</span></span>|<span data-ttu-id="866d3-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="866d3-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="866d3-115">Связи</span><span class="sxs-lookup"><span data-stu-id="866d3-115">Relationships</span></span>
<span data-ttu-id="866d3-116">Нет</span><span class="sxs-lookup"><span data-stu-id="866d3-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="866d3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="866d3-117">JSON Representation</span></span>
<span data-ttu-id="866d3-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="866d3-118">Here is a JSON representation of the resource.</span></span>
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









