---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: tfitzmac
ms.openlocfilehash: 9e1233c9d5a33876da64ab3c75419c322ee83931
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321331"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="c5159-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="c5159-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c5159-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5159-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5159-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5159-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5159-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5159-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5159-107">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="c5159-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="c5159-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c5159-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5159-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5159-109">Properties</span></span>
|<span data-ttu-id="c5159-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5159-110">Property</span></span>|<span data-ttu-id="c5159-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c5159-111">Type</span></span>|<span data-ttu-id="c5159-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c5159-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5159-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="c5159-113">useDeviceLicensing</span></span>|<span data-ttu-id="c5159-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5159-114">Boolean</span></span>|<span data-ttu-id="c5159-115">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="c5159-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="c5159-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="c5159-116">vpnConfigurationId</span></span>|<span data-ttu-id="c5159-117">String</span><span class="sxs-lookup"><span data-stu-id="c5159-117">String</span></span>|<span data-ttu-id="c5159-118">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="c5159-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5159-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c5159-119">Relationships</span></span>
<span data-ttu-id="c5159-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c5159-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c5159-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5159-121">JSON Representation</span></span>
<span data-ttu-id="c5159-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5159-122">Here is a JSON representation of the resource.</span></span>
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





