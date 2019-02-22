---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f09ca9a8f891b90563ebad2cff74775f4c6fb7c2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168399"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="481d7-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="481d7-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="481d7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="481d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="481d7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="481d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="481d7-106">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="481d7-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="481d7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="481d7-107">Properties</span></span>
|<span data-ttu-id="481d7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="481d7-108">Property</span></span>|<span data-ttu-id="481d7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="481d7-109">Type</span></span>|<span data-ttu-id="481d7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="481d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="481d7-111">Суппортусерлиценсинг</span><span class="sxs-lookup"><span data-stu-id="481d7-111">supportUserLicensing</span></span>|<span data-ttu-id="481d7-112">Логический</span><span class="sxs-lookup"><span data-stu-id="481d7-112">Boolean</span></span>|<span data-ttu-id="481d7-113">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="481d7-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="481d7-114">Суппортдевицелиценсинг</span><span class="sxs-lookup"><span data-stu-id="481d7-114">supportDeviceLicensing</span></span>|<span data-ttu-id="481d7-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="481d7-115">Boolean</span></span>|<span data-ttu-id="481d7-116">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="481d7-116">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="481d7-117">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="481d7-117">supportsUserLicensing</span></span>|<span data-ttu-id="481d7-118">Логический</span><span class="sxs-lookup"><span data-stu-id="481d7-118">Boolean</span></span>|<span data-ttu-id="481d7-119">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="481d7-119">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="481d7-120">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="481d7-120">supportsDeviceLicensing</span></span>|<span data-ttu-id="481d7-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="481d7-121">Boolean</span></span>|<span data-ttu-id="481d7-122">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="481d7-122">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="481d7-123">Связи</span><span class="sxs-lookup"><span data-stu-id="481d7-123">Relationships</span></span>
<span data-ttu-id="481d7-124">Нет</span><span class="sxs-lookup"><span data-stu-id="481d7-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="481d7-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="481d7-125">JSON Representation</span></span>
<span data-ttu-id="481d7-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="481d7-126">Here is a JSON representation of the resource.</span></span>
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




