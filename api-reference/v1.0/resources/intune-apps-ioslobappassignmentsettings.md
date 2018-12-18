---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: tfitzmac
ms.openlocfilehash: 78de511bdbdf2e4a8b16d9ce32a790329d2eb3c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306092"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="c7ca1-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="c7ca1-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c7ca1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c7ca1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7ca1-105">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="c7ca1-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="c7ca1-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c7ca1-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7ca1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7ca1-107">Properties</span></span>
|<span data-ttu-id="c7ca1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7ca1-108">Property</span></span>|<span data-ttu-id="c7ca1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c7ca1-109">Type</span></span>|<span data-ttu-id="c7ca1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ca1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ca1-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="c7ca1-111">vpnConfigurationId</span></span>|<span data-ttu-id="c7ca1-112">String</span><span class="sxs-lookup"><span data-stu-id="c7ca1-112">String</span></span>|<span data-ttu-id="c7ca1-113">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="c7ca1-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7ca1-114">Связи</span><span class="sxs-lookup"><span data-stu-id="c7ca1-114">Relationships</span></span>
<span data-ttu-id="c7ca1-115">Нет</span><span class="sxs-lookup"><span data-stu-id="c7ca1-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7ca1-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7ca1-116">JSON Representation</span></span>
<span data-ttu-id="c7ca1-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7ca1-117">Here is a JSON representation of the resource.</span></span>
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



