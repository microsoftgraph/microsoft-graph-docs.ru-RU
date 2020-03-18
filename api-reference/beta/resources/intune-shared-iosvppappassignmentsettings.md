---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a72f1876d0d0dcd181aee7a9b0322f372838377
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769572"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="9bcae-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="9bcae-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="9bcae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bcae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bcae-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bcae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bcae-106">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="9bcae-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="9bcae-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9bcae-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9bcae-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9bcae-108">Properties</span></span>
|<span data-ttu-id="9bcae-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bcae-109">Property</span></span>|<span data-ttu-id="9bcae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9bcae-110">Type</span></span>|<span data-ttu-id="9bcae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9bcae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bcae-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="9bcae-112">useDeviceLicensing</span></span>|<span data-ttu-id="9bcae-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bcae-113">Boolean</span></span>|<span data-ttu-id="9bcae-114">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="9bcae-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="9bcae-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="9bcae-115">vpnConfigurationId</span></span>|<span data-ttu-id="9bcae-116">String</span><span class="sxs-lookup"><span data-stu-id="9bcae-116">String</span></span>|<span data-ttu-id="9bcae-117">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="9bcae-117">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="9bcae-118">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="9bcae-118">**Apps**</span></span>|
|<span data-ttu-id="9bcae-119">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="9bcae-119">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="9bcae-120">Логический</span><span class="sxs-lookup"><span data-stu-id="9bcae-120">Boolean</span></span>|<span data-ttu-id="9bcae-121">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="9bcae-121">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bcae-122">Связи</span><span class="sxs-lookup"><span data-stu-id="9bcae-122">Relationships</span></span>
<span data-ttu-id="9bcae-123">Нет</span><span class="sxs-lookup"><span data-stu-id="9bcae-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bcae-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9bcae-124">JSON Representation</span></span>
<span data-ttu-id="9bcae-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bcae-125">Here is a JSON representation of the resource.</span></span>
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



