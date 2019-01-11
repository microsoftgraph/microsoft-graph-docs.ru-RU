---
title: Тип ресурса deviceDetail
description: Указывает, связанные с устройства, используемый для подписи сведений об устройстве. Включает в себя данные о браузере устройства и сведения о операционной системы, если устройство является управляемым Azure AD.
localization_priority: Normal
ms.openlocfilehash: ca4679a8c484b6dc5b36ef39d3d6d039537cbdbb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884842"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="eb25b-104">Тип ресурса deviceDetail</span><span class="sxs-lookup"><span data-stu-id="eb25b-104">deviceDetail resource type</span></span>
<span data-ttu-id="eb25b-105">Указывает, связанные с устройства, используемый для подписи сведений об устройстве.</span><span class="sxs-lookup"><span data-stu-id="eb25b-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="eb25b-106">Включает в себя данные о браузере устройства и сведения о операционной системы, если устройство является управляемым Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eb25b-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="eb25b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb25b-107">Properties</span></span>
| <span data-ttu-id="eb25b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb25b-108">Property</span></span>     | <span data-ttu-id="eb25b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eb25b-109">Type</span></span>   |<span data-ttu-id="eb25b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eb25b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb25b-111">Обозреватель</span><span class="sxs-lookup"><span data-stu-id="eb25b-111">browser</span></span>|<span data-ttu-id="eb25b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="eb25b-112">String</span></span>|<span data-ttu-id="eb25b-113">Указывает информацию браузеров, используемых для вход в систему.</span><span class="sxs-lookup"><span data-stu-id="eb25b-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="eb25b-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="eb25b-114">deviceId</span></span>|<span data-ttu-id="eb25b-115">String</span><span class="sxs-lookup"><span data-stu-id="eb25b-115">String</span></span>|<span data-ttu-id="eb25b-116">Ссылается на уникальный идентификатор устройства, используемого для подписи в.</span><span class="sxs-lookup"><span data-stu-id="eb25b-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="eb25b-117">displayName</span><span class="sxs-lookup"><span data-stu-id="eb25b-117">displayName</span></span>|<span data-ttu-id="eb25b-118">Строка</span><span class="sxs-lookup"><span data-stu-id="eb25b-118">String</span></span>|<span data-ttu-id="eb25b-119">— Имя устройства, используемый для подписи в.</span><span class="sxs-lookup"><span data-stu-id="eb25b-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="eb25b-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="eb25b-120">isCompliant</span></span>|<span data-ttu-id="eb25b-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb25b-121">Boolean</span></span>|<span data-ttu-id="eb25b-122">Указывает, является ли устройство совместимым.</span><span class="sxs-lookup"><span data-stu-id="eb25b-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="eb25b-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="eb25b-123">isManaged</span></span>|<span data-ttu-id="eb25b-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb25b-124">Boolean</span></span>|<span data-ttu-id="eb25b-125">Указывает, если устройство является управляемым или нет.</span><span class="sxs-lookup"><span data-stu-id="eb25b-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="eb25b-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="eb25b-126">operatingSystem</span></span>|<span data-ttu-id="eb25b-127">String</span><span class="sxs-lookup"><span data-stu-id="eb25b-127">String</span></span>|<span data-ttu-id="eb25b-128">Указывает имя операционная система и версия, используемый для подписи в.</span><span class="sxs-lookup"><span data-stu-id="eb25b-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="eb25b-129">trustType</span><span class="sxs-lookup"><span data-stu-id="eb25b-129">trustType</span></span>|<span data-ttu-id="eb25b-130">String</span><span class="sxs-lookup"><span data-stu-id="eb25b-130">String</span></span>|<span data-ttu-id="eb25b-131">Указывает сведения о того, является ли устройство выполнил вход присоединился к месту в состав AzureAD, присоединенный к домену.</span><span class="sxs-lookup"><span data-stu-id="eb25b-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eb25b-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb25b-132">JSON representation</span></span>

<span data-ttu-id="eb25b-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb25b-133">Here is a JSON representation of the resource.</span></span>

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
