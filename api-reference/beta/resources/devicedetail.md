---
title: Тип ресурса deviceDetail
description: Указывает сведения об устройстве, связанные с устройством, используемым для регистрации.
localization_priority: Normal
author: spunukol
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3fb6b338793b77e3079922cd8c372e402488a22c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761130"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="d8d79-103">Тип ресурса deviceDetail</span><span class="sxs-lookup"><span data-stu-id="d8d79-103">deviceDetail resource type</span></span>

<span data-ttu-id="d8d79-104">Пространство имен: microsoft.graph указывает сведения об устройстве, связанном с устройством, используемым для регистрации.</span><span class="sxs-lookup"><span data-stu-id="d8d79-104">Namespace: microsoft.graph Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="d8d79-105">Включает сведения, такие как браузер устройства и сведения об ОС, если устройство управляется Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d8d79-105">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="d8d79-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8d79-106">Properties</span></span>
| <span data-ttu-id="d8d79-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8d79-107">Property</span></span>     | <span data-ttu-id="d8d79-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d8d79-108">Type</span></span>   |<span data-ttu-id="d8d79-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d8d79-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8d79-110">Обозреватель</span><span class="sxs-lookup"><span data-stu-id="d8d79-110">browser</span></span>|<span data-ttu-id="d8d79-111">String</span><span class="sxs-lookup"><span data-stu-id="d8d79-111">String</span></span>|<span data-ttu-id="d8d79-112">Указывает сведения браузера, используемые для регистрации.</span><span class="sxs-lookup"><span data-stu-id="d8d79-112">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="d8d79-113">deviceId</span><span class="sxs-lookup"><span data-stu-id="d8d79-113">deviceId</span></span>|<span data-ttu-id="d8d79-114">String</span><span class="sxs-lookup"><span data-stu-id="d8d79-114">String</span></span>|<span data-ttu-id="d8d79-115">Относится к UniqueID устройства, используемого для регистрации.</span><span class="sxs-lookup"><span data-stu-id="d8d79-115">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="d8d79-116">displayName</span><span class="sxs-lookup"><span data-stu-id="d8d79-116">displayName</span></span>|<span data-ttu-id="d8d79-117">String</span><span class="sxs-lookup"><span data-stu-id="d8d79-117">String</span></span>|<span data-ttu-id="d8d79-118">Ссылается на имя устройства, используемого для регистрации.</span><span class="sxs-lookup"><span data-stu-id="d8d79-118">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="d8d79-119">isCompliant</span><span class="sxs-lookup"><span data-stu-id="d8d79-119">isCompliant</span></span>|<span data-ttu-id="d8d79-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8d79-120">Boolean</span></span>|<span data-ttu-id="d8d79-121">Указывает, является ли устройство совместимым или нет.</span><span class="sxs-lookup"><span data-stu-id="d8d79-121">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="d8d79-122">isManaged</span><span class="sxs-lookup"><span data-stu-id="d8d79-122">isManaged</span></span>|<span data-ttu-id="d8d79-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8d79-123">Boolean</span></span>|<span data-ttu-id="d8d79-124">Указывает, управляется устройство или нет.</span><span class="sxs-lookup"><span data-stu-id="d8d79-124">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="d8d79-125">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="d8d79-125">operatingSystem</span></span>|<span data-ttu-id="d8d79-126">String</span><span class="sxs-lookup"><span data-stu-id="d8d79-126">String</span></span>|<span data-ttu-id="d8d79-127">Указывает имя и версию ОС, используемые для регистрации.</span><span class="sxs-lookup"><span data-stu-id="d8d79-127">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="d8d79-128">trustType</span><span class="sxs-lookup"><span data-stu-id="d8d79-128">trustType</span></span>|<span data-ttu-id="d8d79-129">String</span><span class="sxs-lookup"><span data-stu-id="d8d79-129">String</span></span>|<span data-ttu-id="d8d79-130">Указывает сведения о том, присоединилось ли устройство к рабочему месту, к AzureAD присоединились, к домену присоединились.</span><span class="sxs-lookup"><span data-stu-id="d8d79-130">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8d79-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8d79-131">JSON representation</span></span>

<span data-ttu-id="d8d79-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8d79-132">Here is a JSON representation of the resource.</span></span>

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


