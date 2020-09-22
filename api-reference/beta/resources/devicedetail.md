---
title: Тип ресурса Девицедетаил
description: Показывает сведения о устройствах, связанных с устройством, используемом для входа.
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 69d8d1e2314021752a5f1a0ab3650d8176ecc8dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049851"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="036ec-103">Тип ресурса Девицедетаил</span><span class="sxs-lookup"><span data-stu-id="036ec-103">deviceDetail resource type</span></span>

<span data-ttu-id="036ec-104">Пространство имен: Microsoft. Graph указывает сведения о устройстве, связанные с устройством, используемом для входа.</span><span class="sxs-lookup"><span data-stu-id="036ec-104">Namespace: microsoft.graph Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="036ec-105">Содержит такие сведения, как браузер устройств и сведения о ОС, если устройство управляется службой Azure AD.</span><span class="sxs-lookup"><span data-stu-id="036ec-105">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="036ec-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="036ec-106">Properties</span></span>
| <span data-ttu-id="036ec-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="036ec-107">Property</span></span>     | <span data-ttu-id="036ec-108">Тип</span><span class="sxs-lookup"><span data-stu-id="036ec-108">Type</span></span>   |<span data-ttu-id="036ec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="036ec-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="036ec-110">Обозреватель</span><span class="sxs-lookup"><span data-stu-id="036ec-110">browser</span></span>|<span data-ttu-id="036ec-111">Строка</span><span class="sxs-lookup"><span data-stu-id="036ec-111">String</span></span>|<span data-ttu-id="036ec-112">Указывает сведения, используемые для входа в браузер.</span><span class="sxs-lookup"><span data-stu-id="036ec-112">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="036ec-113">deviceId</span><span class="sxs-lookup"><span data-stu-id="036ec-113">deviceId</span></span>|<span data-ttu-id="036ec-114">String</span><span class="sxs-lookup"><span data-stu-id="036ec-114">String</span></span>|<span data-ttu-id="036ec-115">Уникальный идентификатор устройства, используемого для входа.</span><span class="sxs-lookup"><span data-stu-id="036ec-115">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="036ec-116">displayName</span><span class="sxs-lookup"><span data-stu-id="036ec-116">displayName</span></span>|<span data-ttu-id="036ec-117">Строка</span><span class="sxs-lookup"><span data-stu-id="036ec-117">String</span></span>|<span data-ttu-id="036ec-118">Указывает имя устройства, используемого для входа.</span><span class="sxs-lookup"><span data-stu-id="036ec-118">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="036ec-119">isCompliant</span><span class="sxs-lookup"><span data-stu-id="036ec-119">isCompliant</span></span>|<span data-ttu-id="036ec-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="036ec-120">Boolean</span></span>|<span data-ttu-id="036ec-121">Указывает, является ли устройство совместимым.</span><span class="sxs-lookup"><span data-stu-id="036ec-121">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="036ec-122">isManaged</span><span class="sxs-lookup"><span data-stu-id="036ec-122">isManaged</span></span>|<span data-ttu-id="036ec-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="036ec-123">Boolean</span></span>|<span data-ttu-id="036ec-124">Указывает, является ли устройство управляемым.</span><span class="sxs-lookup"><span data-stu-id="036ec-124">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="036ec-125">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="036ec-125">operatingSystem</span></span>|<span data-ttu-id="036ec-126">String</span><span class="sxs-lookup"><span data-stu-id="036ec-126">String</span></span>|<span data-ttu-id="036ec-127">Указывает имя и версию операционной системы, которые используются для входа в систему.</span><span class="sxs-lookup"><span data-stu-id="036ec-127">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="036ec-128">trustType</span><span class="sxs-lookup"><span data-stu-id="036ec-128">trustType</span></span>|<span data-ttu-id="036ec-129">String</span><span class="sxs-lookup"><span data-stu-id="036ec-129">String</span></span>|<span data-ttu-id="036ec-130">Указывает, является ли устройство, на который выполнен вход, подключен к рабочему месту, AzureAD присоединен, присоединен к домену.</span><span class="sxs-lookup"><span data-stu-id="036ec-130">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="036ec-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="036ec-131">JSON representation</span></span>

<span data-ttu-id="036ec-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="036ec-132">Here is a JSON representation of the resource.</span></span>

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


