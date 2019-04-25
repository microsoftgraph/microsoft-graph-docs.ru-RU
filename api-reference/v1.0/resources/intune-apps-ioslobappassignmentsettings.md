---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5beacfd60eb2237ed85a95bca21c27a38f956d16
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583160"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="f1efa-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f1efa-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f1efa-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1efa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1efa-105">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="f1efa-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="f1efa-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f1efa-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f1efa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1efa-107">Properties</span></span>
|<span data-ttu-id="f1efa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1efa-108">Property</span></span>|<span data-ttu-id="f1efa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f1efa-109">Type</span></span>|<span data-ttu-id="f1efa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f1efa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1efa-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f1efa-111">vpnConfigurationId</span></span>|<span data-ttu-id="f1efa-112">String</span><span class="sxs-lookup"><span data-stu-id="f1efa-112">String</span></span>|<span data-ttu-id="f1efa-113">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="f1efa-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1efa-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="f1efa-114">Relationships</span></span>
<span data-ttu-id="f1efa-115">Нет</span><span class="sxs-lookup"><span data-stu-id="f1efa-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1efa-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1efa-116">JSON Representation</span></span>
<span data-ttu-id="f1efa-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1efa-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



