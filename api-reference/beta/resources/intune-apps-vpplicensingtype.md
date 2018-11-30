---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
ms.openlocfilehash: 5608fc8c621f28aef5ed3220404cf51118db0b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076631"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="6f501-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="6f501-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="6f501-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f501-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f501-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f501-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f501-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f501-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f501-107">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="6f501-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="6f501-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f501-108">Properties</span></span>
|<span data-ttu-id="6f501-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f501-109">Property</span></span>|<span data-ttu-id="6f501-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6f501-110">Type</span></span>|<span data-ttu-id="6f501-111">Description</span><span class="sxs-lookup"><span data-stu-id="6f501-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f501-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="6f501-112">supportUserLicensing</span></span>|<span data-ttu-id="6f501-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f501-113">Boolean</span></span>|<span data-ttu-id="6f501-114">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f501-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="6f501-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="6f501-115">supportDeviceLicensing</span></span>|<span data-ttu-id="6f501-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f501-116">Boolean</span></span>|<span data-ttu-id="6f501-117">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="6f501-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="6f501-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="6f501-118">supportsUserLicensing</span></span>|<span data-ttu-id="6f501-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f501-119">Boolean</span></span>|<span data-ttu-id="6f501-120">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f501-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="6f501-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="6f501-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="6f501-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f501-122">Boolean</span></span>|<span data-ttu-id="6f501-123">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="6f501-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f501-124">Связи</span><span class="sxs-lookup"><span data-stu-id="6f501-124">Relationships</span></span>
<span data-ttu-id="6f501-125">Нет</span><span class="sxs-lookup"><span data-stu-id="6f501-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6f501-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f501-126">JSON Representation</span></span>
<span data-ttu-id="6f501-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f501-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```





