---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c04e3fbc7da2a355dc8d5b1e69ad90a6f333a9cf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797698"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="4515d-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="4515d-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="4515d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4515d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4515d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4515d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4515d-106">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="4515d-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="4515d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4515d-107">Properties</span></span>
|<span data-ttu-id="4515d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4515d-108">Property</span></span>|<span data-ttu-id="4515d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4515d-109">Type</span></span>|<span data-ttu-id="4515d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4515d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4515d-111">суппортусерлиценсинг</span><span class="sxs-lookup"><span data-stu-id="4515d-111">supportUserLicensing</span></span>|<span data-ttu-id="4515d-112">Логический</span><span class="sxs-lookup"><span data-stu-id="4515d-112">Boolean</span></span>|<span data-ttu-id="4515d-113">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="4515d-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="4515d-114">суппортдевицелиценсинг</span><span class="sxs-lookup"><span data-stu-id="4515d-114">supportDeviceLicensing</span></span>|<span data-ttu-id="4515d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="4515d-115">Boolean</span></span>|<span data-ttu-id="4515d-116">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="4515d-116">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="4515d-117">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="4515d-117">supportsUserLicensing</span></span>|<span data-ttu-id="4515d-118">Логический</span><span class="sxs-lookup"><span data-stu-id="4515d-118">Boolean</span></span>|<span data-ttu-id="4515d-119">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="4515d-119">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="4515d-120">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="4515d-120">supportsDeviceLicensing</span></span>|<span data-ttu-id="4515d-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="4515d-121">Boolean</span></span>|<span data-ttu-id="4515d-122">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="4515d-122">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4515d-123">Связи</span><span class="sxs-lookup"><span data-stu-id="4515d-123">Relationships</span></span>
<span data-ttu-id="4515d-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4515d-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4515d-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4515d-125">JSON Representation</span></span>
<span data-ttu-id="4515d-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4515d-126">Here is a JSON representation of the resource.</span></span>
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



