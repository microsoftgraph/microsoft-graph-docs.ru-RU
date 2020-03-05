---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff94d7ddbec70b40b59dc4b1dbfc1b4a5985be3b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491017"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="94fc5-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="94fc5-103">vppLicensingType resource type</span></span>

<span data-ttu-id="94fc5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="94fc5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94fc5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94fc5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94fc5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94fc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94fc5-107">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="94fc5-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="94fc5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="94fc5-108">Properties</span></span>
|<span data-ttu-id="94fc5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="94fc5-109">Property</span></span>|<span data-ttu-id="94fc5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="94fc5-110">Type</span></span>|<span data-ttu-id="94fc5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="94fc5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94fc5-112">суппортусерлиценсинг</span><span class="sxs-lookup"><span data-stu-id="94fc5-112">supportUserLicensing</span></span>|<span data-ttu-id="94fc5-113">Логический</span><span class="sxs-lookup"><span data-stu-id="94fc5-113">Boolean</span></span>|<span data-ttu-id="94fc5-114">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="94fc5-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="94fc5-115">суппортдевицелиценсинг</span><span class="sxs-lookup"><span data-stu-id="94fc5-115">supportDeviceLicensing</span></span>|<span data-ttu-id="94fc5-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="94fc5-116">Boolean</span></span>|<span data-ttu-id="94fc5-117">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="94fc5-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="94fc5-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="94fc5-118">supportsUserLicensing</span></span>|<span data-ttu-id="94fc5-119">Логический</span><span class="sxs-lookup"><span data-stu-id="94fc5-119">Boolean</span></span>|<span data-ttu-id="94fc5-120">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="94fc5-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="94fc5-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="94fc5-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="94fc5-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="94fc5-122">Boolean</span></span>|<span data-ttu-id="94fc5-123">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="94fc5-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94fc5-124">Связи</span><span class="sxs-lookup"><span data-stu-id="94fc5-124">Relationships</span></span>
<span data-ttu-id="94fc5-125">Нет</span><span class="sxs-lookup"><span data-stu-id="94fc5-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94fc5-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94fc5-126">JSON Representation</span></span>
<span data-ttu-id="94fc5-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94fc5-127">Here is a JSON representation of the resource.</span></span>
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



