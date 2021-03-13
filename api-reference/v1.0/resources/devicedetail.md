---
title: Тип ресурса deviceDetail
description: Указывает сведения об устройстве, связанные с устройством, используемым для регистрации. Это включает сведения о браузере устройства и операционной системе, а также об управляемом устройстве Azure AD.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1c48724a12f7cb29de74a965c1cbb06a44498d26
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761214"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="7a003-104">Тип ресурса deviceDetail</span><span class="sxs-lookup"><span data-stu-id="7a003-104">deviceDetail resource type</span></span>

<span data-ttu-id="7a003-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a003-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7a003-106">Указывает сведения об устройстве, связанные с устройством, используемым для регистрации.</span><span class="sxs-lookup"><span data-stu-id="7a003-106">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="7a003-107">Это включает сведения о браузере устройства и операционной системе, а также об управляемом устройстве Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7a003-107">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="7a003-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a003-108">Properties</span></span>

| <span data-ttu-id="7a003-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a003-109">Property</span></span>     | <span data-ttu-id="7a003-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7a003-110">Type</span></span>   |<span data-ttu-id="7a003-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7a003-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a003-112">Обозреватель</span><span class="sxs-lookup"><span data-stu-id="7a003-112">browser</span></span>|<span data-ttu-id="7a003-113">String</span><span class="sxs-lookup"><span data-stu-id="7a003-113">String</span></span>|<span data-ttu-id="7a003-114">Указывает сведения браузера, используемые для регистрации.</span><span class="sxs-lookup"><span data-stu-id="7a003-114">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="7a003-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="7a003-115">deviceId</span></span>|<span data-ttu-id="7a003-116">String</span><span class="sxs-lookup"><span data-stu-id="7a003-116">String</span></span>|<span data-ttu-id="7a003-117">Ссылается на UniqueID устройства, используемого для регистрации.</span><span class="sxs-lookup"><span data-stu-id="7a003-117">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="7a003-118">displayName</span><span class="sxs-lookup"><span data-stu-id="7a003-118">displayName</span></span>|<span data-ttu-id="7a003-119">String</span><span class="sxs-lookup"><span data-stu-id="7a003-119">String</span></span>|<span data-ttu-id="7a003-120">Ссылается на имя устройства, используемого для регистрации.</span><span class="sxs-lookup"><span data-stu-id="7a003-120">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="7a003-121">isCompliant</span><span class="sxs-lookup"><span data-stu-id="7a003-121">isCompliant</span></span>|<span data-ttu-id="7a003-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a003-122">Boolean</span></span>|<span data-ttu-id="7a003-123">Указывает, соответствует ли устройство.</span><span class="sxs-lookup"><span data-stu-id="7a003-123">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="7a003-124">isManaged</span><span class="sxs-lookup"><span data-stu-id="7a003-124">isManaged</span></span>|<span data-ttu-id="7a003-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a003-125">Boolean</span></span>|<span data-ttu-id="7a003-126">Указывает, управляется ли устройство.</span><span class="sxs-lookup"><span data-stu-id="7a003-126">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="7a003-127">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="7a003-127">operatingSystem</span></span>|<span data-ttu-id="7a003-128">String</span><span class="sxs-lookup"><span data-stu-id="7a003-128">String</span></span>|<span data-ttu-id="7a003-129">Указывает имя операционной системы и версию, используемую для регистрации.</span><span class="sxs-lookup"><span data-stu-id="7a003-129">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="7a003-130">trustType</span><span class="sxs-lookup"><span data-stu-id="7a003-130">trustType</span></span>|<span data-ttu-id="7a003-131">String</span><span class="sxs-lookup"><span data-stu-id="7a003-131">String</span></span>|<span data-ttu-id="7a003-132">Предоставляет сведения о том, является ли подписанное устройство рабочим местом, AzureAD Joined, Domain Joined.</span><span class="sxs-lookup"><span data-stu-id="7a003-132">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a003-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a003-133">JSON representation</span></span>

<span data-ttu-id="7a003-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a003-134">Here is a JSON representation of the resource.</span></span>

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

