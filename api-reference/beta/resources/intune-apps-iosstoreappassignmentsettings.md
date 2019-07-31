---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: afd310f3b49d7d0dfa2d5f2bbcbb836c09ab2bf2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005508"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="64334-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="64334-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="64334-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64334-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64334-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64334-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64334-106">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="64334-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="64334-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="64334-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64334-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="64334-108">Properties</span></span>
|<span data-ttu-id="64334-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="64334-109">Property</span></span>|<span data-ttu-id="64334-110">Тип</span><span class="sxs-lookup"><span data-stu-id="64334-110">Type</span></span>|<span data-ttu-id="64334-111">Описание</span><span class="sxs-lookup"><span data-stu-id="64334-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64334-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="64334-112">vpnConfigurationId</span></span>|<span data-ttu-id="64334-113">String</span><span class="sxs-lookup"><span data-stu-id="64334-113">String</span></span>|<span data-ttu-id="64334-114">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="64334-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64334-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="64334-115">Relationships</span></span>
<span data-ttu-id="64334-116">Нет</span><span class="sxs-lookup"><span data-stu-id="64334-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64334-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64334-117">JSON Representation</span></span>
<span data-ttu-id="64334-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64334-118">Here is a JSON representation of the resource.</span></span>
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





