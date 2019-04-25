---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b46c9bcd8680ffbd78c1cfc85cc6dec85126e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557931"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="4f6e3-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="4f6e3-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="4f6e3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f6e3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f6e3-105">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="4f6e3-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="4f6e3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f6e3-106">Properties</span></span>
|<span data-ttu-id="4f6e3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f6e3-107">Property</span></span>|<span data-ttu-id="4f6e3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4f6e3-108">Type</span></span>|<span data-ttu-id="4f6e3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6e3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f6e3-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="4f6e3-110">supportsUserLicensing</span></span>|<span data-ttu-id="4f6e3-111">Логический</span><span class="sxs-lookup"><span data-stu-id="4f6e3-111">Boolean</span></span>|<span data-ttu-id="4f6e3-112">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f6e3-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="4f6e3-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="4f6e3-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="4f6e3-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f6e3-114">Boolean</span></span>|<span data-ttu-id="4f6e3-115">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="4f6e3-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f6e3-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="4f6e3-116">Relationships</span></span>
<span data-ttu-id="4f6e3-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4f6e3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f6e3-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f6e3-118">JSON Representation</span></span>
<span data-ttu-id="4f6e3-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f6e3-119">Here is a JSON representation of the resource.</span></span>
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



