---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ea50a193467d684de052292b8113b6ae3c95d7fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527399"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="155d4-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="155d4-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="155d4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="155d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="155d4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="155d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="155d4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="155d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="155d4-107">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="155d4-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="155d4-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="155d4-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="155d4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="155d4-109">Properties</span></span>
|<span data-ttu-id="155d4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="155d4-110">Property</span></span>|<span data-ttu-id="155d4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="155d4-111">Type</span></span>|<span data-ttu-id="155d4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="155d4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="155d4-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="155d4-113">vpnConfigurationId</span></span>|<span data-ttu-id="155d4-114">String</span><span class="sxs-lookup"><span data-stu-id="155d4-114">String</span></span>|<span data-ttu-id="155d4-115">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="155d4-115">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="155d4-116">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="155d4-116">**Apps**</span></span>|
|<span data-ttu-id="155d4-117">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="155d4-117">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="155d4-118">Логический</span><span class="sxs-lookup"><span data-stu-id="155d4-118">Boolean</span></span>|<span data-ttu-id="155d4-119">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="155d4-119">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="155d4-120">Связи</span><span class="sxs-lookup"><span data-stu-id="155d4-120">Relationships</span></span>
<span data-ttu-id="155d4-121">Нет</span><span class="sxs-lookup"><span data-stu-id="155d4-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="155d4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="155d4-122">JSON Representation</span></span>
<span data-ttu-id="155d4-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="155d4-123">Here is a JSON representation of the resource.</span></span>
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



