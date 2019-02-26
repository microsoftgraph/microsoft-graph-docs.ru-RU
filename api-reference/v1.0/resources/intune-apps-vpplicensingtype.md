---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b46c9bcd8680ffbd78c1cfc85cc6dec85126e6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256121"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="dc5e4-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="dc5e4-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="dc5e4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc5e4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc5e4-105">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="dc5e4-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="dc5e4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc5e4-106">Properties</span></span>
|<span data-ttu-id="dc5e4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc5e4-107">Property</span></span>|<span data-ttu-id="dc5e4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dc5e4-108">Type</span></span>|<span data-ttu-id="dc5e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dc5e4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc5e4-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="dc5e4-110">supportsUserLicensing</span></span>|<span data-ttu-id="dc5e4-111">Логический</span><span class="sxs-lookup"><span data-stu-id="dc5e4-111">Boolean</span></span>|<span data-ttu-id="dc5e4-112">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="dc5e4-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="dc5e4-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="dc5e4-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="dc5e4-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc5e4-114">Boolean</span></span>|<span data-ttu-id="dc5e4-115">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="dc5e4-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc5e4-116">Связи</span><span class="sxs-lookup"><span data-stu-id="dc5e4-116">Relationships</span></span>
<span data-ttu-id="dc5e4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="dc5e4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc5e4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc5e4-118">JSON Representation</span></span>
<span data-ttu-id="dc5e4-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc5e4-119">Here is a JSON representation of the resource.</span></span>
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



