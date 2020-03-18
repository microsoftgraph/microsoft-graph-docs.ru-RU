---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 23cb5d484aaa813bfb1b3cd352cd0168e750713e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769677"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="b7b07-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b7b07-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b7b07-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7b07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7b07-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7b07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7b07-106">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="b7b07-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="b7b07-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b7b07-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b7b07-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7b07-108">Properties</span></span>
|<span data-ttu-id="b7b07-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7b07-109">Property</span></span>|<span data-ttu-id="b7b07-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b7b07-110">Type</span></span>|<span data-ttu-id="b7b07-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b7b07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7b07-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="b7b07-112">vpnConfigurationId</span></span>|<span data-ttu-id="b7b07-113">String</span><span class="sxs-lookup"><span data-stu-id="b7b07-113">String</span></span>|<span data-ttu-id="b7b07-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="b7b07-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="b7b07-115">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="b7b07-115">**Apps**</span></span>|
|<span data-ttu-id="b7b07-116">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="b7b07-116">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="b7b07-117">Логический</span><span class="sxs-lookup"><span data-stu-id="b7b07-117">Boolean</span></span>|<span data-ttu-id="b7b07-118">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="b7b07-118">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7b07-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b7b07-119">Relationships</span></span>
<span data-ttu-id="b7b07-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b7b07-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7b07-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7b07-121">JSON Representation</span></span>
<span data-ttu-id="b7b07-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7b07-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



