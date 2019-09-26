---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04e2bedc18d16b1f882835eabdc32b87a9cff5a4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201219"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="e68bd-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e68bd-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e68bd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e68bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e68bd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e68bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e68bd-106">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="e68bd-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="e68bd-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e68bd-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e68bd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e68bd-108">Properties</span></span>
|<span data-ttu-id="e68bd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e68bd-109">Property</span></span>|<span data-ttu-id="e68bd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e68bd-110">Type</span></span>|<span data-ttu-id="e68bd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e68bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e68bd-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e68bd-112">useDeviceLicensing</span></span>|<span data-ttu-id="e68bd-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="e68bd-113">Boolean</span></span>|<span data-ttu-id="e68bd-114">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="e68bd-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="e68bd-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e68bd-115">vpnConfigurationId</span></span>|<span data-ttu-id="e68bd-116">String</span><span class="sxs-lookup"><span data-stu-id="e68bd-116">String</span></span>|<span data-ttu-id="e68bd-117">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="e68bd-117">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="e68bd-118">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="e68bd-118">**Apps**</span></span>|
|<span data-ttu-id="e68bd-119">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="e68bd-119">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="e68bd-120">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e68bd-120">Boolean</span></span>|<span data-ttu-id="e68bd-121">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="e68bd-121">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e68bd-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="e68bd-122">Relationships</span></span>
<span data-ttu-id="e68bd-123">Нет</span><span class="sxs-lookup"><span data-stu-id="e68bd-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e68bd-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e68bd-124">JSON Representation</span></span>
<span data-ttu-id="e68bd-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e68bd-125">Here is a JSON representation of the resource.</span></span>
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



