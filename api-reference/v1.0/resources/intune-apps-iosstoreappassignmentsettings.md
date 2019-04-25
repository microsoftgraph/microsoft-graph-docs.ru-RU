---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d58490e97aec48f664ab6882198e4c1da3511e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523947"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="1c60b-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1c60b-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1c60b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c60b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c60b-105">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="1c60b-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="1c60b-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1c60b-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c60b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c60b-107">Properties</span></span>
|<span data-ttu-id="1c60b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c60b-108">Property</span></span>|<span data-ttu-id="1c60b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1c60b-109">Type</span></span>|<span data-ttu-id="1c60b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1c60b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c60b-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="1c60b-111">vpnConfigurationId</span></span>|<span data-ttu-id="1c60b-112">String</span><span class="sxs-lookup"><span data-stu-id="1c60b-112">String</span></span>|<span data-ttu-id="1c60b-113">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="1c60b-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c60b-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="1c60b-114">Relationships</span></span>
<span data-ttu-id="1c60b-115">Нет</span><span class="sxs-lookup"><span data-stu-id="1c60b-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c60b-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c60b-116">JSON Representation</span></span>
<span data-ttu-id="1c60b-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c60b-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



