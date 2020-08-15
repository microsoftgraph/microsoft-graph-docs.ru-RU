---
title: Тип ресурса profilePhoto
description: Фотография профиля пользователя, группы или контакта Outlook из Exchange Online. Это двоичные данные, не представленные в кодировке base-64.
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ef54be828c9094c76c215c66c79fd2c1453503dc
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757232"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="30955-104">Тип ресурса profilePhoto</span><span class="sxs-lookup"><span data-stu-id="30955-104">profilePhoto resource type</span></span>

<span data-ttu-id="30955-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30955-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="30955-p102">Фотография профиля пользователя, группы или контакта Outlook из Exchange Online. Это двоичные данные, не представленные в кодировке base-64.</span><span class="sxs-lookup"><span data-stu-id="30955-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="30955-108">Поддерживаемые размеры фотографий в формате HD для Exchange Online: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 и 648x648.</span><span class="sxs-lookup"><span data-stu-id="30955-108">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="30955-109">Методы</span><span class="sxs-lookup"><span data-stu-id="30955-109">Methods</span></span>

| <span data-ttu-id="30955-110">Метод</span><span class="sxs-lookup"><span data-stu-id="30955-110">Method</span></span>       | <span data-ttu-id="30955-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="30955-111">Return Type</span></span>  |<span data-ttu-id="30955-112">Описание</span><span class="sxs-lookup"><span data-stu-id="30955-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30955-113">Получение объекта profilePhoto</span><span class="sxs-lookup"><span data-stu-id="30955-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="30955-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="30955-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="30955-115">Получение указанного объекта **profilePhoto** или его метаданных (свойств profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="30955-115">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="30955-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="30955-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="30955-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="30955-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="30955-p103">Назначение фотографии указанному пользователю, группе или контакту. Фотография должна быть представлена в двоичном формате. Она заменяет текущую фотографию (если она существует).</span><span class="sxs-lookup"><span data-stu-id="30955-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="30955-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="30955-121">Properties</span></span>
| <span data-ttu-id="30955-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="30955-122">Property</span></span>     | <span data-ttu-id="30955-123">Тип</span><span class="sxs-lookup"><span data-stu-id="30955-123">Type</span></span>   |<span data-ttu-id="30955-124">Описание</span><span class="sxs-lookup"><span data-stu-id="30955-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30955-125">id</span><span class="sxs-lookup"><span data-stu-id="30955-125">id</span></span>|<span data-ttu-id="30955-126">string</span><span class="sxs-lookup"><span data-stu-id="30955-126">string</span></span>|<span data-ttu-id="30955-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30955-127">Read-only.</span></span>|
|<span data-ttu-id="30955-128">height</span><span class="sxs-lookup"><span data-stu-id="30955-128">height</span></span>|<span data-ttu-id="30955-129">int32</span><span class="sxs-lookup"><span data-stu-id="30955-129">int32</span></span>|<span data-ttu-id="30955-p104">Высота фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30955-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="30955-132">width</span><span class="sxs-lookup"><span data-stu-id="30955-132">width</span></span>|<span data-ttu-id="30955-133">int32</span><span class="sxs-lookup"><span data-stu-id="30955-133">int32</span></span>|<span data-ttu-id="30955-p105">Ширина фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30955-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30955-136">Связи</span><span class="sxs-lookup"><span data-stu-id="30955-136">Relationships</span></span>
<span data-ttu-id="30955-137">Нет</span><span class="sxs-lookup"><span data-stu-id="30955-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="30955-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30955-138">JSON representation</span></span>

<span data-ttu-id="30955-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30955-139">Here is a JSON representation of the resource.</span></span>

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
