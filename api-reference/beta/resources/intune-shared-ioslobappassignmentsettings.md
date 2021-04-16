---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 820ae9ce7ec4a76891962628086d4eade5ba04cd
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866131"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="f6fc3-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f6fc3-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="f6fc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6fc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6fc3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6fc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6fc3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6fc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6fc3-107">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="f6fc3-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="f6fc3-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f6fc3-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f6fc3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6fc3-109">Properties</span></span>
|<span data-ttu-id="f6fc3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6fc3-110">Property</span></span>|<span data-ttu-id="f6fc3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f6fc3-111">Type</span></span>|<span data-ttu-id="f6fc3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f6fc3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6fc3-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f6fc3-113">vpnConfigurationId</span></span>|<span data-ttu-id="f6fc3-114">String</span><span class="sxs-lookup"><span data-stu-id="f6fc3-114">String</span></span>|<span data-ttu-id="f6fc3-115">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="f6fc3-115">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="f6fc3-116">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="f6fc3-116">**Apps**</span></span>|
|<span data-ttu-id="f6fc3-117">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="f6fc3-117">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="f6fc3-118">Логический</span><span class="sxs-lookup"><span data-stu-id="f6fc3-118">Boolean</span></span>|<span data-ttu-id="f6fc3-119">Следует ли удалить приложение при удалении устройства из Intune.</span><span class="sxs-lookup"><span data-stu-id="f6fc3-119">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6fc3-120">Связи</span><span class="sxs-lookup"><span data-stu-id="f6fc3-120">Relationships</span></span>
<span data-ttu-id="f6fc3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="f6fc3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6fc3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6fc3-122">JSON Representation</span></span>
<span data-ttu-id="f6fc3-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6fc3-123">Here is a JSON representation of the resource.</span></span>
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




