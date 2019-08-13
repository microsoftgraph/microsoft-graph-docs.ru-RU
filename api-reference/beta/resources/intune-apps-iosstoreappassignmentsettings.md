---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da1d42d092c7a85831da6ae26b55b43db7ac7db7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365990"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="eb518-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="eb518-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="eb518-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb518-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb518-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb518-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb518-106">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="eb518-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="eb518-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="eb518-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb518-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb518-108">Properties</span></span>
|<span data-ttu-id="eb518-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb518-109">Property</span></span>|<span data-ttu-id="eb518-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eb518-110">Type</span></span>|<span data-ttu-id="eb518-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eb518-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb518-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="eb518-112">vpnConfigurationId</span></span>|<span data-ttu-id="eb518-113">String</span><span class="sxs-lookup"><span data-stu-id="eb518-113">String</span></span>|<span data-ttu-id="eb518-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="eb518-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="eb518-115">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="eb518-115">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="eb518-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb518-116">Boolean</span></span>|<span data-ttu-id="eb518-117">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="eb518-117">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb518-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="eb518-118">Relationships</span></span>
<span data-ttu-id="eb518-119">Нет</span><span class="sxs-lookup"><span data-stu-id="eb518-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb518-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb518-120">JSON Representation</span></span>
<span data-ttu-id="eb518-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb518-121">Here is a JSON representation of the resource.</span></span>
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



