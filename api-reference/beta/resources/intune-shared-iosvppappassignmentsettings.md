---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 56e19bb10115faaf7386e6f54dc5ca2dc368ee33
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866092"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="e9736-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e9736-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="e9736-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9736-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9736-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9736-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9736-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9736-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9736-107">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="e9736-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="e9736-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e9736-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9736-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9736-109">Properties</span></span>
|<span data-ttu-id="e9736-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9736-110">Property</span></span>|<span data-ttu-id="e9736-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e9736-111">Type</span></span>|<span data-ttu-id="e9736-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e9736-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9736-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e9736-113">useDeviceLicensing</span></span>|<span data-ttu-id="e9736-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9736-114">Boolean</span></span>|<span data-ttu-id="e9736-115">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="e9736-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="e9736-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e9736-116">vpnConfigurationId</span></span>|<span data-ttu-id="e9736-117">String</span><span class="sxs-lookup"><span data-stu-id="e9736-117">String</span></span>|<span data-ttu-id="e9736-118">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="e9736-118">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="e9736-119">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="e9736-119">**Apps**</span></span>|
|<span data-ttu-id="e9736-120">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="e9736-120">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="e9736-121">Логический</span><span class="sxs-lookup"><span data-stu-id="e9736-121">Boolean</span></span>|<span data-ttu-id="e9736-122">Следует ли удалить приложение при удалении устройства из Intune.</span><span class="sxs-lookup"><span data-stu-id="e9736-122">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9736-123">Связи</span><span class="sxs-lookup"><span data-stu-id="e9736-123">Relationships</span></span>
<span data-ttu-id="e9736-124">Нет</span><span class="sxs-lookup"><span data-stu-id="e9736-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9736-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9736-125">JSON Representation</span></span>
<span data-ttu-id="e9736-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9736-126">Here is a JSON representation of the resource.</span></span>
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




