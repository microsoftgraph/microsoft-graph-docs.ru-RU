---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f96077d6231d1997effcff185f263f0724651ef9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071089"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="92a20-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="92a20-103">vppLicensingType resource type</span></span>

<span data-ttu-id="92a20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92a20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92a20-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92a20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92a20-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92a20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92a20-107">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="92a20-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="92a20-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="92a20-108">Properties</span></span>
|<span data-ttu-id="92a20-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="92a20-109">Property</span></span>|<span data-ttu-id="92a20-110">Тип</span><span class="sxs-lookup"><span data-stu-id="92a20-110">Type</span></span>|<span data-ttu-id="92a20-111">Описание</span><span class="sxs-lookup"><span data-stu-id="92a20-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92a20-112">суппортусерлиценсинг</span><span class="sxs-lookup"><span data-stu-id="92a20-112">supportUserLicensing</span></span>|<span data-ttu-id="92a20-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="92a20-113">Boolean</span></span>|<span data-ttu-id="92a20-114">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="92a20-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="92a20-115">суппортдевицелиценсинг</span><span class="sxs-lookup"><span data-stu-id="92a20-115">supportDeviceLicensing</span></span>|<span data-ttu-id="92a20-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="92a20-116">Boolean</span></span>|<span data-ttu-id="92a20-117">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="92a20-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="92a20-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="92a20-118">supportsUserLicensing</span></span>|<span data-ttu-id="92a20-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="92a20-119">Boolean</span></span>|<span data-ttu-id="92a20-120">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="92a20-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="92a20-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="92a20-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="92a20-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="92a20-122">Boolean</span></span>|<span data-ttu-id="92a20-123">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="92a20-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92a20-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="92a20-124">Relationships</span></span>
<span data-ttu-id="92a20-125">Нет</span><span class="sxs-lookup"><span data-stu-id="92a20-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92a20-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92a20-126">JSON Representation</span></span>
<span data-ttu-id="92a20-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92a20-127">Here is a JSON representation of the resource.</span></span>
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






