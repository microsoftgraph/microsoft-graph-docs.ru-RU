---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c7dbaded456e4f4df9874635a27b7f46d0ca7a2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094304"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="9a95e-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="9a95e-103">vppLicensingType resource type</span></span>

<span data-ttu-id="9a95e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a95e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a95e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a95e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a95e-106">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="9a95e-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="9a95e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a95e-107">Properties</span></span>
|<span data-ttu-id="9a95e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a95e-108">Property</span></span>|<span data-ttu-id="9a95e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9a95e-109">Type</span></span>|<span data-ttu-id="9a95e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9a95e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a95e-111">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="9a95e-111">supportsUserLicensing</span></span>|<span data-ttu-id="9a95e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a95e-112">Boolean</span></span>|<span data-ttu-id="9a95e-113">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="9a95e-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="9a95e-114">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="9a95e-114">supportsDeviceLicensing</span></span>|<span data-ttu-id="9a95e-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a95e-115">Boolean</span></span>|<span data-ttu-id="9a95e-116">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="9a95e-116">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a95e-117">Связи</span><span class="sxs-lookup"><span data-stu-id="9a95e-117">Relationships</span></span>
<span data-ttu-id="9a95e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9a95e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a95e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a95e-119">JSON Representation</span></span>
<span data-ttu-id="9a95e-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a95e-120">Here is a JSON representation of the resource.</span></span>
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









