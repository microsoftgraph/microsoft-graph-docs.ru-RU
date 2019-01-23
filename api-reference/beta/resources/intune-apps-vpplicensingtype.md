---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 42bb678077781309b9e06c339112537bc2e48bde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399677"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="bd470-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="bd470-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="bd470-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd470-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd470-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd470-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd470-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd470-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd470-107">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="bd470-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="bd470-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd470-108">Properties</span></span>
|<span data-ttu-id="bd470-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd470-109">Property</span></span>|<span data-ttu-id="bd470-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bd470-110">Type</span></span>|<span data-ttu-id="bd470-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd470-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd470-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="bd470-112">supportUserLicensing</span></span>|<span data-ttu-id="bd470-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd470-113">Boolean</span></span>|<span data-ttu-id="bd470-114">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd470-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="bd470-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="bd470-115">supportDeviceLicensing</span></span>|<span data-ttu-id="bd470-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd470-116">Boolean</span></span>|<span data-ttu-id="bd470-117">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="bd470-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="bd470-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="bd470-118">supportsUserLicensing</span></span>|<span data-ttu-id="bd470-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd470-119">Boolean</span></span>|<span data-ttu-id="bd470-120">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd470-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="bd470-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="bd470-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="bd470-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd470-122">Boolean</span></span>|<span data-ttu-id="bd470-123">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="bd470-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd470-124">Связи</span><span class="sxs-lookup"><span data-stu-id="bd470-124">Relationships</span></span>
<span data-ttu-id="bd470-125">Нет</span><span class="sxs-lookup"><span data-stu-id="bd470-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd470-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd470-126">JSON Representation</span></span>
<span data-ttu-id="bd470-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd470-127">Here is a JSON representation of the resource.</span></span>
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




