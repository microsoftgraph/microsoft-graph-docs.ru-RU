---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2fd271222d6e44878bdbd5efd7f26e1a2d74dd1a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727176"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="24b4b-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="24b4b-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="24b4b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24b4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24b4b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24b4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24b4b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24b4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24b4b-107">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="24b4b-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="24b4b-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="24b4b-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24b4b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="24b4b-109">Properties</span></span>
|<span data-ttu-id="24b4b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="24b4b-110">Property</span></span>|<span data-ttu-id="24b4b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="24b4b-111">Type</span></span>|<span data-ttu-id="24b4b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="24b4b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24b4b-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="24b4b-113">vpnConfigurationId</span></span>|<span data-ttu-id="24b4b-114">String</span><span class="sxs-lookup"><span data-stu-id="24b4b-114">String</span></span>|<span data-ttu-id="24b4b-115">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="24b4b-115">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="24b4b-116">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="24b4b-116">**Apps**</span></span>|
|<span data-ttu-id="24b4b-117">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="24b4b-117">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="24b4b-118">Логический</span><span class="sxs-lookup"><span data-stu-id="24b4b-118">Boolean</span></span>|<span data-ttu-id="24b4b-119">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="24b4b-119">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24b4b-120">Связи</span><span class="sxs-lookup"><span data-stu-id="24b4b-120">Relationships</span></span>
<span data-ttu-id="24b4b-121">Нет</span><span class="sxs-lookup"><span data-stu-id="24b4b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24b4b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24b4b-122">JSON Representation</span></span>
<span data-ttu-id="24b4b-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24b4b-123">Here is a JSON representation of the resource.</span></span>
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





