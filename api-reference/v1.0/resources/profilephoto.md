---
title: Тип ресурса profilePhoto
description: Фотография профиля пользователя, группы или контакта Outlook из Exchange Online. Это двоичные данные, не представленные в кодировке base-64.
localization_priority: Priority
ms.openlocfilehash: b1901928a97356b2a9808a446d34981fd74bf456
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876568"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="35c9a-104">Тип ресурса profilePhoto</span><span class="sxs-lookup"><span data-stu-id="35c9a-104">profilePhoto resource type</span></span>
<span data-ttu-id="35c9a-p102">Фотография профиля пользователя, группы или контакта Outlook из Exchange Online. Это двоичные данные, не представленные в кодировке base-64.</span><span class="sxs-lookup"><span data-stu-id="35c9a-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="35c9a-107">Поддерживаемые размеры фотографий в формате HD для Exchange Online: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 и 648x648.</span><span class="sxs-lookup"><span data-stu-id="35c9a-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="35c9a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="35c9a-108">Methods</span></span>

| <span data-ttu-id="35c9a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="35c9a-109">Method</span></span>       | <span data-ttu-id="35c9a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="35c9a-110">Return Type</span></span>  |<span data-ttu-id="35c9a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35c9a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35c9a-112">Получение объекта profilePhoto</span><span class="sxs-lookup"><span data-stu-id="35c9a-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="35c9a-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="35c9a-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="35c9a-114">Получение указанного объекта **profilePhoto** или его метаданных (свойств profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="35c9a-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="35c9a-115">Обновление</span><span class="sxs-lookup"><span data-stu-id="35c9a-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="35c9a-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="35c9a-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="35c9a-p103">Назначение фотографии указанному пользователю, группе или контакту. Фотография должна быть представлена в двоичном формате. Она заменяет текущую фотографию (если она существует).</span><span class="sxs-lookup"><span data-stu-id="35c9a-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="35c9a-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="35c9a-120">Properties</span></span>
| <span data-ttu-id="35c9a-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="35c9a-121">Property</span></span>     | <span data-ttu-id="35c9a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="35c9a-122">Type</span></span>   |<span data-ttu-id="35c9a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="35c9a-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35c9a-124">id</span><span class="sxs-lookup"><span data-stu-id="35c9a-124">id</span></span>|<span data-ttu-id="35c9a-125">строка</span><span class="sxs-lookup"><span data-stu-id="35c9a-125">string</span></span>|<span data-ttu-id="35c9a-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35c9a-126">Read-only.</span></span>|
|<span data-ttu-id="35c9a-127">height</span><span class="sxs-lookup"><span data-stu-id="35c9a-127">height</span></span>|<span data-ttu-id="35c9a-128">int32</span><span class="sxs-lookup"><span data-stu-id="35c9a-128">int32</span></span>|<span data-ttu-id="35c9a-p104">Высота фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35c9a-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="35c9a-131">width</span><span class="sxs-lookup"><span data-stu-id="35c9a-131">width</span></span>|<span data-ttu-id="35c9a-132">int32</span><span class="sxs-lookup"><span data-stu-id="35c9a-132">int32</span></span>|<span data-ttu-id="35c9a-p105">Ширина фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35c9a-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35c9a-135">Связи</span><span class="sxs-lookup"><span data-stu-id="35c9a-135">Relationships</span></span>
<span data-ttu-id="35c9a-136">Нет</span><span class="sxs-lookup"><span data-stu-id="35c9a-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="35c9a-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35c9a-137">JSON representation</span></span>

<span data-ttu-id="35c9a-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35c9a-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
