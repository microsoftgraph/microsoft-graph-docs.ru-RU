---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
ms.openlocfilehash: 4e02cc4ee100fe9fa6be0eb116cff18e343fd8ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025125"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="a6520-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="a6520-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="a6520-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a6520-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6520-105">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="a6520-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="a6520-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6520-106">Properties</span></span>
|<span data-ttu-id="a6520-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6520-107">Property</span></span>|<span data-ttu-id="a6520-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a6520-108">Type</span></span>|<span data-ttu-id="a6520-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a6520-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6520-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="a6520-110">supportsUserLicensing</span></span>|<span data-ttu-id="a6520-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6520-111">Boolean</span></span>|<span data-ttu-id="a6520-112">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="a6520-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="a6520-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="a6520-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="a6520-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6520-114">Boolean</span></span>|<span data-ttu-id="a6520-115">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="a6520-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6520-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a6520-116">Relationships</span></span>
<span data-ttu-id="a6520-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a6520-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a6520-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6520-118">JSON Representation</span></span>
<span data-ttu-id="a6520-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6520-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



