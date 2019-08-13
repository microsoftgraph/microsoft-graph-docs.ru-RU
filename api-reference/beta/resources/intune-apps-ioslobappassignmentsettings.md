---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3cb8c437d5cb943ef4d6f76ed515b917f8a3e10a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366065"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="66d10-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="66d10-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="66d10-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66d10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66d10-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66d10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d10-106">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="66d10-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="66d10-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="66d10-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="66d10-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="66d10-108">Properties</span></span>
|<span data-ttu-id="66d10-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="66d10-109">Property</span></span>|<span data-ttu-id="66d10-110">Тип</span><span class="sxs-lookup"><span data-stu-id="66d10-110">Type</span></span>|<span data-ttu-id="66d10-111">Описание</span><span class="sxs-lookup"><span data-stu-id="66d10-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d10-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="66d10-112">vpnConfigurationId</span></span>|<span data-ttu-id="66d10-113">String</span><span class="sxs-lookup"><span data-stu-id="66d10-113">String</span></span>|<span data-ttu-id="66d10-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="66d10-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="66d10-115">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="66d10-115">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="66d10-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="66d10-116">Boolean</span></span>|<span data-ttu-id="66d10-117">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="66d10-117">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66d10-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="66d10-118">Relationships</span></span>
<span data-ttu-id="66d10-119">Нет</span><span class="sxs-lookup"><span data-stu-id="66d10-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66d10-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66d10-120">JSON Representation</span></span>
<span data-ttu-id="66d10-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66d10-121">Here is a JSON representation of the resource.</span></span>
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



