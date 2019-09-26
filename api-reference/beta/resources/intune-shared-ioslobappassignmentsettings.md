---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a379e7467fb7e76a1043d73f766dace5b28a27d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201228"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="23daf-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="23daf-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="23daf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23daf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23daf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23daf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23daf-106">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="23daf-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="23daf-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="23daf-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23daf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="23daf-108">Properties</span></span>
|<span data-ttu-id="23daf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="23daf-109">Property</span></span>|<span data-ttu-id="23daf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="23daf-110">Type</span></span>|<span data-ttu-id="23daf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="23daf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23daf-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="23daf-112">vpnConfigurationId</span></span>|<span data-ttu-id="23daf-113">String</span><span class="sxs-lookup"><span data-stu-id="23daf-113">String</span></span>|<span data-ttu-id="23daf-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="23daf-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="23daf-115">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="23daf-115">**Apps**</span></span>|
|<span data-ttu-id="23daf-116">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="23daf-116">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="23daf-117">Boolean.</span><span class="sxs-lookup"><span data-stu-id="23daf-117">Boolean</span></span>|<span data-ttu-id="23daf-118">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="23daf-118">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23daf-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="23daf-119">Relationships</span></span>
<span data-ttu-id="23daf-120">Нет</span><span class="sxs-lookup"><span data-stu-id="23daf-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23daf-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23daf-121">JSON Representation</span></span>
<span data-ttu-id="23daf-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23daf-122">Here is a JSON representation of the resource.</span></span>
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



