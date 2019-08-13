---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb4fd7e4a2cded97bdd5d61921cd1819908a4d77
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366779"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="9eef2-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="9eef2-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="9eef2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eef2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9eef2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9eef2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9eef2-106">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="9eef2-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="9eef2-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9eef2-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9eef2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9eef2-108">Properties</span></span>
|<span data-ttu-id="9eef2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9eef2-109">Property</span></span>|<span data-ttu-id="9eef2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9eef2-110">Type</span></span>|<span data-ttu-id="9eef2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9eef2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eef2-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="9eef2-112">useDeviceLicensing</span></span>|<span data-ttu-id="9eef2-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="9eef2-113">Boolean</span></span>|<span data-ttu-id="9eef2-114">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="9eef2-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="9eef2-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="9eef2-115">vpnConfigurationId</span></span>|<span data-ttu-id="9eef2-116">String</span><span class="sxs-lookup"><span data-stu-id="9eef2-116">String</span></span>|<span data-ttu-id="9eef2-117">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="9eef2-117">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="9eef2-118">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="9eef2-118">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="9eef2-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="9eef2-119">Boolean</span></span>|<span data-ttu-id="9eef2-120">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="9eef2-120">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9eef2-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="9eef2-121">Relationships</span></span>
<span data-ttu-id="9eef2-122">Нет</span><span class="sxs-lookup"><span data-stu-id="9eef2-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9eef2-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9eef2-123">JSON Representation</span></span>
<span data-ttu-id="9eef2-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9eef2-124">Here is a JSON representation of the resource.</span></span>
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



