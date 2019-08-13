---
title: Тип ресурса vppLicensingType
description: Содержит свойства для корпоративного лицензирования приложений iOS (VPP).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4303a77b2aa9a403c7d618e8b8cc07ddb7b3774f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335776"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="0bd9f-103">Тип ресурса vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="0bd9f-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="0bd9f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bd9f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bd9f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bd9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bd9f-106">Содержит свойства для корпоративного лицензирования приложений iOS (VPP).</span><span class="sxs-lookup"><span data-stu-id="0bd9f-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="0bd9f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bd9f-107">Properties</span></span>
|<span data-ttu-id="0bd9f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bd9f-108">Property</span></span>|<span data-ttu-id="0bd9f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0bd9f-109">Type</span></span>|<span data-ttu-id="0bd9f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0bd9f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bd9f-111">суппортусерлиценсинг</span><span class="sxs-lookup"><span data-stu-id="0bd9f-111">supportUserLicensing</span></span>|<span data-ttu-id="0bd9f-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bd9f-112">Boolean</span></span>|<span data-ttu-id="0bd9f-113">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="0bd9f-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="0bd9f-114">суппортдевицелиценсинг</span><span class="sxs-lookup"><span data-stu-id="0bd9f-114">supportDeviceLicensing</span></span>|<span data-ttu-id="0bd9f-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bd9f-115">Boolean</span></span>|<span data-ttu-id="0bd9f-116">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="0bd9f-116">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="0bd9f-117">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="0bd9f-117">supportsUserLicensing</span></span>|<span data-ttu-id="0bd9f-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bd9f-118">Boolean</span></span>|<span data-ttu-id="0bd9f-119">Указывает, поддерживает ли программа тип лицензирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="0bd9f-119">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="0bd9f-120">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="0bd9f-120">supportsDeviceLicensing</span></span>|<span data-ttu-id="0bd9f-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bd9f-121">Boolean</span></span>|<span data-ttu-id="0bd9f-122">Указывает, поддерживает ли программа тип лицензирования устройства.</span><span class="sxs-lookup"><span data-stu-id="0bd9f-122">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bd9f-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="0bd9f-123">Relationships</span></span>
<span data-ttu-id="0bd9f-124">Нет</span><span class="sxs-lookup"><span data-stu-id="0bd9f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bd9f-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0bd9f-125">JSON Representation</span></span>
<span data-ttu-id="0bd9f-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bd9f-126">Here is a JSON representation of the resource.</span></span>
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



