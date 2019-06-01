---
title: Тип ресурса Девицедетаил
description: Показывает сведения о устройствах, связанных с устройством, используемом для входа. Содержит такие сведения, как браузер устройств и сведения о ОС, если устройство управляется службой Azure AD.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f3a0d7f141723beb5194860b025fe6fa349eb95a
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657702"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="4ab0b-104">Тип ресурса Девицедетаил</span><span class="sxs-lookup"><span data-stu-id="4ab0b-104">deviceDetail resource type</span></span>
<span data-ttu-id="4ab0b-105">Показывает сведения о устройствах, связанных с устройством, используемом для входа.</span><span class="sxs-lookup"><span data-stu-id="4ab0b-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="4ab0b-106">Содержит такие сведения, как браузер устройств и сведения о ОС, если устройство управляется службой Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4ab0b-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="4ab0b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ab0b-107">Properties</span></span>
| <span data-ttu-id="4ab0b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ab0b-108">Property</span></span>     | <span data-ttu-id="4ab0b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4ab0b-109">Type</span></span>   |<span data-ttu-id="4ab0b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ab0b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ab0b-111">Обозреватель</span><span class="sxs-lookup"><span data-stu-id="4ab0b-111">browser</span></span>|<span data-ttu-id="4ab0b-112">String</span><span class="sxs-lookup"><span data-stu-id="4ab0b-112">String</span></span>|<span data-ttu-id="4ab0b-113">Указывает сведения, используемые для входа в браузер.</span><span class="sxs-lookup"><span data-stu-id="4ab0b-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="4ab0b-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="4ab0b-114">deviceId</span></span>|<span data-ttu-id="4ab0b-115">String</span><span class="sxs-lookup"><span data-stu-id="4ab0b-115">String</span></span>|<span data-ttu-id="4ab0b-116">Уникальный идентификатор устройства, используемого для входа.</span><span class="sxs-lookup"><span data-stu-id="4ab0b-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="4ab0b-117">displayName</span><span class="sxs-lookup"><span data-stu-id="4ab0b-117">displayName</span></span>|<span data-ttu-id="4ab0b-118">String</span><span class="sxs-lookup"><span data-stu-id="4ab0b-118">String</span></span>|<span data-ttu-id="4ab0b-119">Указывает имя устройства, используемого для входа.</span><span class="sxs-lookup"><span data-stu-id="4ab0b-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="4ab0b-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="4ab0b-120">isCompliant</span></span>|<span data-ttu-id="4ab0b-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab0b-121">Boolean</span></span>|<span data-ttu-id="4ab0b-122">Указывает, является ли устройство совместимым.</span><span class="sxs-lookup"><span data-stu-id="4ab0b-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="4ab0b-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="4ab0b-123">isManaged</span></span>|<span data-ttu-id="4ab0b-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab0b-124">Boolean</span></span>|<span data-ttu-id="4ab0b-125">Указывает, является ли устройство управляемым.</span><span class="sxs-lookup"><span data-stu-id="4ab0b-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="4ab0b-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="4ab0b-126">operatingSystem</span></span>|<span data-ttu-id="4ab0b-127">String</span><span class="sxs-lookup"><span data-stu-id="4ab0b-127">String</span></span>|<span data-ttu-id="4ab0b-128">Указывает имя и версию операционной системы, которые используются для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="4ab0b-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="4ab0b-129">trustType</span><span class="sxs-lookup"><span data-stu-id="4ab0b-129">trustType</span></span>|<span data-ttu-id="4ab0b-130">String</span><span class="sxs-lookup"><span data-stu-id="4ab0b-130">String</span></span>|<span data-ttu-id="4ab0b-131">Указывает, является ли устройство, на который выполнен вход, подключен к рабочему месту, AzureAD присоединен, присоединен к домену.</span><span class="sxs-lookup"><span data-stu-id="4ab0b-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4ab0b-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ab0b-132">JSON representation</span></span>

<span data-ttu-id="4ab0b-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ab0b-133">Here is a JSON representation of the resource.</span></span>

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
