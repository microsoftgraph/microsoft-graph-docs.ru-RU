---
title: Тип ресурса iosVppAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e221ceb67789f9d96195a31bd7eba8f37a9df6bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917646"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="b9cdb-103">Тип ресурса iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b9cdb-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b9cdb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b9cdb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9cdb-105">Содержит свойства, используемые при назначении мобильного приложения VPP для iOS группе.</span><span class="sxs-lookup"><span data-stu-id="b9cdb-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="b9cdb-106">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b9cdb-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b9cdb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9cdb-107">Properties</span></span>
|<span data-ttu-id="b9cdb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9cdb-108">Property</span></span>|<span data-ttu-id="b9cdb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b9cdb-109">Type</span></span>|<span data-ttu-id="b9cdb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9cdb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9cdb-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="b9cdb-111">useDeviceLicensing</span></span>|<span data-ttu-id="b9cdb-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9cdb-112">Boolean</span></span>|<span data-ttu-id="b9cdb-113">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="b9cdb-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="b9cdb-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="b9cdb-114">vpnConfigurationId</span></span>|<span data-ttu-id="b9cdb-115">String</span><span class="sxs-lookup"><span data-stu-id="b9cdb-115">String</span></span>|<span data-ttu-id="b9cdb-116">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="b9cdb-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9cdb-117">Связи</span><span class="sxs-lookup"><span data-stu-id="b9cdb-117">Relationships</span></span>
<span data-ttu-id="b9cdb-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b9cdb-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b9cdb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9cdb-119">JSON Representation</span></span>
<span data-ttu-id="b9cdb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9cdb-120">Here is a JSON representation of the resource.</span></span>
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



