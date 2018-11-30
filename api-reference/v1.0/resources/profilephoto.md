---
title: Тип ресурса profilePhoto
description: Фотография профиля пользователя, группы или контакта Outlook из Exchange Online. Это двоичные данные, не представленные в кодировке base-64.
ms.openlocfilehash: c5f74e1dcd48e42a2e17d5a64e6ed4b9e9cca5e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028385"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="8e7b6-104">Тип ресурса profilePhoto</span><span class="sxs-lookup"><span data-stu-id="8e7b6-104">profilePhoto resource type</span></span>
<span data-ttu-id="8e7b6-p102">Фотография профиля пользователя, группы или контакта Outlook из Exchange Online. Это двоичные данные, не представленные в кодировке base-64.</span><span class="sxs-lookup"><span data-stu-id="8e7b6-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="8e7b6-107">Поддерживаемые размеры фотографий в формате HD для Exchange Online: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 и 648x648.</span><span class="sxs-lookup"><span data-stu-id="8e7b6-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="8e7b6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8e7b6-108">Methods</span></span>

| <span data-ttu-id="8e7b6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8e7b6-109">Method</span></span>       | <span data-ttu-id="8e7b6-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e7b6-110">Return Type</span></span>  |<span data-ttu-id="8e7b6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8e7b6-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8e7b6-112">Получение объекта profilePhoto</span><span class="sxs-lookup"><span data-stu-id="8e7b6-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="8e7b6-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="8e7b6-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="8e7b6-114">Получение указанного объекта **profilePhoto** или его метаданных (свойств profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="8e7b6-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="8e7b6-115">Обновление</span><span class="sxs-lookup"><span data-stu-id="8e7b6-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="8e7b6-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="8e7b6-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="8e7b6-p103">Назначение фотографии указанному пользователю, группе или контакту. Фотография должна быть представлена в двоичном формате. Она заменяет текущую фотографию (если она существует).</span><span class="sxs-lookup"><span data-stu-id="8e7b6-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e7b6-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e7b6-120">Properties</span></span>
| <span data-ttu-id="8e7b6-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e7b6-121">Property</span></span>     | <span data-ttu-id="8e7b6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8e7b6-122">Type</span></span>   |<span data-ttu-id="8e7b6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8e7b6-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e7b6-124">id</span><span class="sxs-lookup"><span data-stu-id="8e7b6-124">id</span></span>|<span data-ttu-id="8e7b6-125">строка</span><span class="sxs-lookup"><span data-stu-id="8e7b6-125">string</span></span>|<span data-ttu-id="8e7b6-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e7b6-126">Read-only.</span></span>|
|<span data-ttu-id="8e7b6-127">height</span><span class="sxs-lookup"><span data-stu-id="8e7b6-127">height</span></span>|<span data-ttu-id="8e7b6-128">int32</span><span class="sxs-lookup"><span data-stu-id="8e7b6-128">int32</span></span>|<span data-ttu-id="8e7b6-p104">Высота фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e7b6-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="8e7b6-131">width</span><span class="sxs-lookup"><span data-stu-id="8e7b6-131">width</span></span>|<span data-ttu-id="8e7b6-132">int32</span><span class="sxs-lookup"><span data-stu-id="8e7b6-132">int32</span></span>|<span data-ttu-id="8e7b6-p105">Ширина фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e7b6-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e7b6-135">Связи</span><span class="sxs-lookup"><span data-stu-id="8e7b6-135">Relationships</span></span>
<span data-ttu-id="8e7b6-136">Нет</span><span class="sxs-lookup"><span data-stu-id="8e7b6-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8e7b6-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e7b6-137">JSON representation</span></span>

<span data-ttu-id="8e7b6-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e7b6-138">Here is a JSON representation of the resource.</span></span>

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
