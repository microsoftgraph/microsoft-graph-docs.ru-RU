---
title: Тип ресурса Девицедетаил
description: Показывает сведения о устройствах, связанных с устройством, используемом для входа. Сюда входят такие сведения, как браузер устройств и операционная система, а также, является ли устройство управляемым Azure AD.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8730c6fefebadbd2c64937366c7b7de41537b11c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531674"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="31334-104">Тип ресурса Девицедетаил</span><span class="sxs-lookup"><span data-stu-id="31334-104">deviceDetail resource type</span></span>

<span data-ttu-id="31334-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31334-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31334-106">Показывает сведения о устройствах, связанных с устройством, используемом для входа.</span><span class="sxs-lookup"><span data-stu-id="31334-106">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="31334-107">Сюда входят такие сведения, как браузер устройств и операционная система, а также, является ли устройство управляемым Azure AD.</span><span class="sxs-lookup"><span data-stu-id="31334-107">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="31334-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="31334-108">Properties</span></span>

| <span data-ttu-id="31334-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="31334-109">Property</span></span>     | <span data-ttu-id="31334-110">Тип</span><span class="sxs-lookup"><span data-stu-id="31334-110">Type</span></span>   |<span data-ttu-id="31334-111">Описание</span><span class="sxs-lookup"><span data-stu-id="31334-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31334-112">Обозреватель</span><span class="sxs-lookup"><span data-stu-id="31334-112">browser</span></span>|<span data-ttu-id="31334-113">Строка</span><span class="sxs-lookup"><span data-stu-id="31334-113">String</span></span>|<span data-ttu-id="31334-114">Указывает сведения о браузере, используемом для входа.</span><span class="sxs-lookup"><span data-stu-id="31334-114">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="31334-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="31334-115">deviceId</span></span>|<span data-ttu-id="31334-116">String</span><span class="sxs-lookup"><span data-stu-id="31334-116">String</span></span>|<span data-ttu-id="31334-117">Указывает уникальный идентификатор устройства, используемого для входа.</span><span class="sxs-lookup"><span data-stu-id="31334-117">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="31334-118">displayName</span><span class="sxs-lookup"><span data-stu-id="31334-118">displayName</span></span>|<span data-ttu-id="31334-119">Строка</span><span class="sxs-lookup"><span data-stu-id="31334-119">String</span></span>|<span data-ttu-id="31334-120">Указывает на имя устройства, используемого для входа.</span><span class="sxs-lookup"><span data-stu-id="31334-120">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="31334-121">isCompliant</span><span class="sxs-lookup"><span data-stu-id="31334-121">isCompliant</span></span>|<span data-ttu-id="31334-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="31334-122">Boolean</span></span>|<span data-ttu-id="31334-123">Указывает, является ли устройство совместимым.</span><span class="sxs-lookup"><span data-stu-id="31334-123">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="31334-124">isManaged</span><span class="sxs-lookup"><span data-stu-id="31334-124">isManaged</span></span>|<span data-ttu-id="31334-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="31334-125">Boolean</span></span>|<span data-ttu-id="31334-126">Указывает, является ли устройство управляемым.</span><span class="sxs-lookup"><span data-stu-id="31334-126">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="31334-127">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="31334-127">operatingSystem</span></span>|<span data-ttu-id="31334-128">Строка</span><span class="sxs-lookup"><span data-stu-id="31334-128">String</span></span>|<span data-ttu-id="31334-129">Указывает имя и версию операционной системы, используемую для входа.</span><span class="sxs-lookup"><span data-stu-id="31334-129">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="31334-130">trustType</span><span class="sxs-lookup"><span data-stu-id="31334-130">trustType</span></span>|<span data-ttu-id="31334-131">Строка</span><span class="sxs-lookup"><span data-stu-id="31334-131">String</span></span>|<span data-ttu-id="31334-132">Сведения о том, является ли устройство, на котором выполнен вход, присоединено к рабочему месту, AzureAD присоединено к домену.</span><span class="sxs-lookup"><span data-stu-id="31334-132">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31334-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31334-133">JSON representation</span></span>

<span data-ttu-id="31334-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31334-134">Here is a JSON representation of the resource.</span></span>

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
