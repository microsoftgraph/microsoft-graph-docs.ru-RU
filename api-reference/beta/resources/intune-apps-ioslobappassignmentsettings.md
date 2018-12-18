---
title: Тип ресурса iosLobAppAssignmentSettings
description: Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.
author: tfitzmac
ms.openlocfilehash: ca85fff558285ea52f14e359d17511a3e879e24a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361742"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="982d2-103">Тип ресурса iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="982d2-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="982d2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="982d2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="982d2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="982d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="982d2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="982d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="982d2-107">Содержит свойства, используемые при назначении бизнес-приложения для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="982d2-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="982d2-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="982d2-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="982d2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="982d2-109">Properties</span></span>
|<span data-ttu-id="982d2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="982d2-110">Property</span></span>|<span data-ttu-id="982d2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="982d2-111">Type</span></span>|<span data-ttu-id="982d2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="982d2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="982d2-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="982d2-113">vpnConfigurationId</span></span>|<span data-ttu-id="982d2-114">String</span><span class="sxs-lookup"><span data-stu-id="982d2-114">String</span></span>|<span data-ttu-id="982d2-115">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="982d2-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="982d2-116">Связи</span><span class="sxs-lookup"><span data-stu-id="982d2-116">Relationships</span></span>
<span data-ttu-id="982d2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="982d2-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="982d2-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="982d2-118">JSON Representation</span></span>
<span data-ttu-id="982d2-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="982d2-119">Here is a JSON representation of the resource.</span></span>
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





