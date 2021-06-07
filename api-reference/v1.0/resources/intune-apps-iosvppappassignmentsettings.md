---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 342f773d48b4918693b6062aba161ce72c82d743
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756066"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="14d2c-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="14d2c-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="14d2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14d2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14d2c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14d2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14d2c-106">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="14d2c-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="14d2c-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="14d2c-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14d2c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="14d2c-108">Properties</span></span>
|<span data-ttu-id="14d2c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="14d2c-109">Property</span></span>|<span data-ttu-id="14d2c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="14d2c-110">Type</span></span>|<span data-ttu-id="14d2c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="14d2c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14d2c-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="14d2c-112">useDeviceLicensing</span></span>|<span data-ttu-id="14d2c-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="14d2c-113">Boolean</span></span>|<span data-ttu-id="14d2c-114">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="14d2c-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="14d2c-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="14d2c-115">vpnConfigurationId</span></span>|<span data-ttu-id="14d2c-116">String</span><span class="sxs-lookup"><span data-stu-id="14d2c-116">String</span></span>|<span data-ttu-id="14d2c-117">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="14d2c-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14d2c-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="14d2c-118">Relationships</span></span>
<span data-ttu-id="14d2c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="14d2c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14d2c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14d2c-120">JSON Representation</span></span>
<span data-ttu-id="14d2c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14d2c-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```




