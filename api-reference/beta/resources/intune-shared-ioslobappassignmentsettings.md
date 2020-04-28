---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fe57b72e2e656d3653cfb2c2d7b2f62361c29b5e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407594"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="2ebea-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="2ebea-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="2ebea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ebea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ebea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ebea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ebea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ebea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ebea-107">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="2ebea-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="2ebea-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2ebea-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ebea-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ebea-109">Properties</span></span>
|<span data-ttu-id="2ebea-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ebea-110">Property</span></span>|<span data-ttu-id="2ebea-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2ebea-111">Type</span></span>|<span data-ttu-id="2ebea-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2ebea-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ebea-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="2ebea-113">vpnConfigurationId</span></span>|<span data-ttu-id="2ebea-114">String</span><span class="sxs-lookup"><span data-stu-id="2ebea-114">String</span></span>|<span data-ttu-id="2ebea-115">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="2ebea-115">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="2ebea-116">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="2ebea-116">**Apps**</span></span>|
|<span data-ttu-id="2ebea-117">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="2ebea-117">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="2ebea-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ebea-118">Boolean</span></span>|<span data-ttu-id="2ebea-119">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="2ebea-119">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ebea-120">Связи</span><span class="sxs-lookup"><span data-stu-id="2ebea-120">Relationships</span></span>
<span data-ttu-id="2ebea-121">Нет</span><span class="sxs-lookup"><span data-stu-id="2ebea-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ebea-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ebea-122">JSON Representation</span></span>
<span data-ttu-id="2ebea-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ebea-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



