---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 39f007a88fc05504fc83b624a886c719ffe08ba3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962275"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="03a98-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="03a98-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="03a98-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03a98-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03a98-105">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="03a98-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="03a98-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="03a98-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="03a98-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="03a98-107">Properties</span></span>
|<span data-ttu-id="03a98-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="03a98-108">Property</span></span>|<span data-ttu-id="03a98-109">Тип</span><span class="sxs-lookup"><span data-stu-id="03a98-109">Type</span></span>|<span data-ttu-id="03a98-110">Описание</span><span class="sxs-lookup"><span data-stu-id="03a98-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03a98-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="03a98-111">vpnConfigurationId</span></span>|<span data-ttu-id="03a98-112">String</span><span class="sxs-lookup"><span data-stu-id="03a98-112">String</span></span>|<span data-ttu-id="03a98-113">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="03a98-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03a98-114">Связи</span><span class="sxs-lookup"><span data-stu-id="03a98-114">Relationships</span></span>
<span data-ttu-id="03a98-115">Нет</span><span class="sxs-lookup"><span data-stu-id="03a98-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03a98-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03a98-116">JSON Representation</span></span>
<span data-ttu-id="03a98-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03a98-117">Here is a JSON representation of the resource.</span></span>
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



