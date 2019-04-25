---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36c6e2c60423038f2af10ccdbcfaf94ecd6ec3aa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552326"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="f9caf-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f9caf-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f9caf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9caf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9caf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9caf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9caf-106">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="f9caf-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="f9caf-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f9caf-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f9caf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9caf-108">Properties</span></span>
|<span data-ttu-id="f9caf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9caf-109">Property</span></span>|<span data-ttu-id="f9caf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f9caf-110">Type</span></span>|<span data-ttu-id="f9caf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9caf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9caf-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="f9caf-112">useDeviceLicensing</span></span>|<span data-ttu-id="f9caf-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9caf-113">Boolean</span></span>|<span data-ttu-id="f9caf-114">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="f9caf-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="f9caf-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f9caf-115">vpnConfigurationId</span></span>|<span data-ttu-id="f9caf-116">String</span><span class="sxs-lookup"><span data-stu-id="f9caf-116">String</span></span>|<span data-ttu-id="f9caf-117">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="f9caf-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9caf-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="f9caf-118">Relationships</span></span>
<span data-ttu-id="f9caf-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f9caf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9caf-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9caf-120">JSON Representation</span></span>
<span data-ttu-id="f9caf-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9caf-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```





