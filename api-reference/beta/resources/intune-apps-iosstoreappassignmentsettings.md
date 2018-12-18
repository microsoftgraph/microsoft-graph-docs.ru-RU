---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
author: tfitzmac
ms.openlocfilehash: 19a9ba760a0e375d6afa4c504fd57e6ecac4d2ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303950"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="fc10e-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="fc10e-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="fc10e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc10e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc10e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc10e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc10e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc10e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc10e-107">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="fc10e-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="fc10e-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="fc10e-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc10e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc10e-109">Properties</span></span>
|<span data-ttu-id="fc10e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc10e-110">Property</span></span>|<span data-ttu-id="fc10e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fc10e-111">Type</span></span>|<span data-ttu-id="fc10e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fc10e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc10e-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="fc10e-113">vpnConfigurationId</span></span>|<span data-ttu-id="fc10e-114">String</span><span class="sxs-lookup"><span data-stu-id="fc10e-114">String</span></span>|<span data-ttu-id="fc10e-115">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="fc10e-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc10e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="fc10e-116">Relationships</span></span>
<span data-ttu-id="fc10e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="fc10e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc10e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc10e-118">JSON Representation</span></span>
<span data-ttu-id="fc10e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc10e-119">Here is a JSON representation of the resource.</span></span>
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





