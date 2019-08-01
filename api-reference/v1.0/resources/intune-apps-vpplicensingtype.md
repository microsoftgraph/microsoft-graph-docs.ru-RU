---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 831961fd9e04bff577fe986a2e6309d1cdfbcca0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032132"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="8693e-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="8693e-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="8693e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8693e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8693e-105">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="8693e-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="8693e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8693e-106">Properties</span></span>
|<span data-ttu-id="8693e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8693e-107">Property</span></span>|<span data-ttu-id="8693e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8693e-108">Type</span></span>|<span data-ttu-id="8693e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8693e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8693e-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="8693e-110">supportsUserLicensing</span></span>|<span data-ttu-id="8693e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="8693e-111">Boolean</span></span>|<span data-ttu-id="8693e-112">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="8693e-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="8693e-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8693e-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="8693e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8693e-114">Boolean</span></span>|<span data-ttu-id="8693e-115">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="8693e-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8693e-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="8693e-116">Relationships</span></span>
<span data-ttu-id="8693e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8693e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8693e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8693e-118">JSON Representation</span></span>
<span data-ttu-id="8693e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8693e-119">Here is a JSON representation of the resource.</span></span>
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



