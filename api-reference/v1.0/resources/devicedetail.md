---
title: Тип ресурса Девицедетаил
description: Показывает сведения о устройствах, связанных с устройством, используемом для входа. Сюда входят такие сведения, как браузер устройств и операционная система, а также, является ли устройство управляемым Azure AD.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a6ea50eeea3a906346b69466d2686a2de101792a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629301"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="7c756-104">Тип ресурса Девицедетаил</span><span class="sxs-lookup"><span data-stu-id="7c756-104">deviceDetail resource type</span></span>

<span data-ttu-id="7c756-105">Показывает сведения о устройствах, связанных с устройством, используемом для входа.</span><span class="sxs-lookup"><span data-stu-id="7c756-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="7c756-106">Сюда входят такие сведения, как браузер устройств и операционная система, а также, является ли устройство управляемым Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7c756-106">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="7c756-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c756-107">Properties</span></span>

| <span data-ttu-id="7c756-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c756-108">Property</span></span>     | <span data-ttu-id="7c756-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7c756-109">Type</span></span>   |<span data-ttu-id="7c756-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7c756-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c756-111">Обозреватель</span><span class="sxs-lookup"><span data-stu-id="7c756-111">browser</span></span>|<span data-ttu-id="7c756-112">String</span><span class="sxs-lookup"><span data-stu-id="7c756-112">String</span></span>|<span data-ttu-id="7c756-113">Указывает сведения о браузере, используемом для входа.</span><span class="sxs-lookup"><span data-stu-id="7c756-113">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="7c756-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="7c756-114">deviceId</span></span>|<span data-ttu-id="7c756-115">String</span><span class="sxs-lookup"><span data-stu-id="7c756-115">String</span></span>|<span data-ttu-id="7c756-116">Указывает уникальный идентификатор устройства, используемого для входа.</span><span class="sxs-lookup"><span data-stu-id="7c756-116">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="7c756-117">displayName</span><span class="sxs-lookup"><span data-stu-id="7c756-117">displayName</span></span>|<span data-ttu-id="7c756-118">String</span><span class="sxs-lookup"><span data-stu-id="7c756-118">String</span></span>|<span data-ttu-id="7c756-119">Указывает на имя устройства, используемого для входа.</span><span class="sxs-lookup"><span data-stu-id="7c756-119">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="7c756-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="7c756-120">isCompliant</span></span>|<span data-ttu-id="7c756-121">Логический</span><span class="sxs-lookup"><span data-stu-id="7c756-121">Boolean</span></span>|<span data-ttu-id="7c756-122">Указывает, является ли устройство совместимым.</span><span class="sxs-lookup"><span data-stu-id="7c756-122">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="7c756-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="7c756-123">isManaged</span></span>|<span data-ttu-id="7c756-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c756-124">Boolean</span></span>|<span data-ttu-id="7c756-125">Указывает, является ли устройство управляемым.</span><span class="sxs-lookup"><span data-stu-id="7c756-125">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="7c756-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="7c756-126">operatingSystem</span></span>|<span data-ttu-id="7c756-127">String</span><span class="sxs-lookup"><span data-stu-id="7c756-127">String</span></span>|<span data-ttu-id="7c756-128">Указывает имя и версию операционной системы, используемую для входа.</span><span class="sxs-lookup"><span data-stu-id="7c756-128">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="7c756-129">trustType</span><span class="sxs-lookup"><span data-stu-id="7c756-129">trustType</span></span>|<span data-ttu-id="7c756-130">String</span><span class="sxs-lookup"><span data-stu-id="7c756-130">String</span></span>|<span data-ttu-id="7c756-131">Сведения о том, является ли устройство, на котором выполнен вход, присоединено к рабочему месту, AzureAD присоединено к домену.</span><span class="sxs-lookup"><span data-stu-id="7c756-131">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7c756-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7c756-132">JSON representation</span></span>

<span data-ttu-id="7c756-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c756-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
