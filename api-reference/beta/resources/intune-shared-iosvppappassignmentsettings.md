---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a8393b4da0b4c31f2e0bfd455f6eeb6f1b51dea8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460596"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="f6e18-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f6e18-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="f6e18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6e18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6e18-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6e18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6e18-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6e18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6e18-107">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="f6e18-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="f6e18-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f6e18-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f6e18-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6e18-109">Properties</span></span>
|<span data-ttu-id="f6e18-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6e18-110">Property</span></span>|<span data-ttu-id="f6e18-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f6e18-111">Type</span></span>|<span data-ttu-id="f6e18-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f6e18-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6e18-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="f6e18-113">useDeviceLicensing</span></span>|<span data-ttu-id="f6e18-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6e18-114">Boolean</span></span>|<span data-ttu-id="f6e18-115">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="f6e18-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="f6e18-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f6e18-116">vpnConfigurationId</span></span>|<span data-ttu-id="f6e18-117">String</span><span class="sxs-lookup"><span data-stu-id="f6e18-117">String</span></span>|<span data-ttu-id="f6e18-118">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="f6e18-118">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="f6e18-119">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="f6e18-119">**Apps**</span></span>|
|<span data-ttu-id="f6e18-120">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="f6e18-120">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="f6e18-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6e18-121">Boolean</span></span>|<span data-ttu-id="f6e18-122">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="f6e18-122">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6e18-123">Связи</span><span class="sxs-lookup"><span data-stu-id="f6e18-123">Relationships</span></span>
<span data-ttu-id="f6e18-124">Нет</span><span class="sxs-lookup"><span data-stu-id="f6e18-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6e18-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6e18-125">JSON Representation</span></span>
<span data-ttu-id="f6e18-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6e18-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



