---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f815b0530a87dd937a7ff9e88c8ff928865378ef
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684465"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="a6427-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a6427-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="a6427-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6427-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6427-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6427-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6427-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6427-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6427-107">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="a6427-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="a6427-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a6427-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a6427-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6427-109">Properties</span></span>
|<span data-ttu-id="a6427-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6427-110">Property</span></span>|<span data-ttu-id="a6427-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a6427-111">Type</span></span>|<span data-ttu-id="a6427-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a6427-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6427-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="a6427-113">useDeviceLicensing</span></span>|<span data-ttu-id="a6427-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6427-114">Boolean</span></span>|<span data-ttu-id="a6427-115">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="a6427-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="a6427-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a6427-116">vpnConfigurationId</span></span>|<span data-ttu-id="a6427-117">String</span><span class="sxs-lookup"><span data-stu-id="a6427-117">String</span></span>|<span data-ttu-id="a6427-118">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="a6427-118">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="a6427-119">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="a6427-119">**Apps**</span></span>|
|<span data-ttu-id="a6427-120">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="a6427-120">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="a6427-121">Логический</span><span class="sxs-lookup"><span data-stu-id="a6427-121">Boolean</span></span>|<span data-ttu-id="a6427-122">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="a6427-122">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6427-123">Связи</span><span class="sxs-lookup"><span data-stu-id="a6427-123">Relationships</span></span>
<span data-ttu-id="a6427-124">Нет</span><span class="sxs-lookup"><span data-stu-id="a6427-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6427-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6427-125">JSON Representation</span></span>
<span data-ttu-id="a6427-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6427-126">Here is a JSON representation of the resource.</span></span>
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





