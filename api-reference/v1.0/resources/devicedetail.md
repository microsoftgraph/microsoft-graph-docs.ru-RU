---
title: Тип ресурса Девицедетаил
description: Показывает сведения о устройствах, связанных с устройством, используемом для входа. Сюда входят такие сведения, как браузер устройств и операционная система, а также, является ли устройство управляемым Azure AD.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cf5de980f28768fdd92ed4b052e0c678be1cdac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029500"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="169c3-104">Тип ресурса Девицедетаил</span><span class="sxs-lookup"><span data-stu-id="169c3-104">deviceDetail resource type</span></span>

<span data-ttu-id="169c3-105">Показывает сведения о устройствах, связанных с устройством, используемом для входа.</span><span class="sxs-lookup"><span data-stu-id="169c3-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="169c3-106">Сюда входят такие сведения, как браузер устройств и операционная система, а также, является ли устройство управляемым Azure AD.</span><span class="sxs-lookup"><span data-stu-id="169c3-106">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="169c3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="169c3-107">Properties</span></span>

| <span data-ttu-id="169c3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="169c3-108">Property</span></span>     | <span data-ttu-id="169c3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="169c3-109">Type</span></span>   |<span data-ttu-id="169c3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="169c3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="169c3-111">Обозреватель</span><span class="sxs-lookup"><span data-stu-id="169c3-111">browser</span></span>|<span data-ttu-id="169c3-112">String</span><span class="sxs-lookup"><span data-stu-id="169c3-112">String</span></span>|<span data-ttu-id="169c3-113">Указывает сведения о браузере, используемом для входа.</span><span class="sxs-lookup"><span data-stu-id="169c3-113">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="169c3-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="169c3-114">deviceId</span></span>|<span data-ttu-id="169c3-115">String</span><span class="sxs-lookup"><span data-stu-id="169c3-115">String</span></span>|<span data-ttu-id="169c3-116">Указывает уникальный идентификатор устройства, используемого для входа.</span><span class="sxs-lookup"><span data-stu-id="169c3-116">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="169c3-117">displayName</span><span class="sxs-lookup"><span data-stu-id="169c3-117">displayName</span></span>|<span data-ttu-id="169c3-118">String</span><span class="sxs-lookup"><span data-stu-id="169c3-118">String</span></span>|<span data-ttu-id="169c3-119">Указывает на имя устройства, используемого для входа.</span><span class="sxs-lookup"><span data-stu-id="169c3-119">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="169c3-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="169c3-120">isCompliant</span></span>|<span data-ttu-id="169c3-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="169c3-121">Boolean</span></span>|<span data-ttu-id="169c3-122">Указывает, является ли устройство совместимым.</span><span class="sxs-lookup"><span data-stu-id="169c3-122">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="169c3-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="169c3-123">isManaged</span></span>|<span data-ttu-id="169c3-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="169c3-124">Boolean</span></span>|<span data-ttu-id="169c3-125">Указывает, является ли устройство управляемым.</span><span class="sxs-lookup"><span data-stu-id="169c3-125">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="169c3-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="169c3-126">operatingSystem</span></span>|<span data-ttu-id="169c3-127">String</span><span class="sxs-lookup"><span data-stu-id="169c3-127">String</span></span>|<span data-ttu-id="169c3-128">Указывает имя и версию операционной системы, используемую для входа.</span><span class="sxs-lookup"><span data-stu-id="169c3-128">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="169c3-129">trustType</span><span class="sxs-lookup"><span data-stu-id="169c3-129">trustType</span></span>|<span data-ttu-id="169c3-130">String</span><span class="sxs-lookup"><span data-stu-id="169c3-130">String</span></span>|<span data-ttu-id="169c3-131">Сведения о том, является ли устройство, на котором выполнен вход, присоединено к рабочему месту, AzureAD присоединено к домену.</span><span class="sxs-lookup"><span data-stu-id="169c3-131">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="169c3-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="169c3-132">JSON representation</span></span>

<span data-ttu-id="169c3-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="169c3-133">Here is a JSON representation of the resource.</span></span>

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
