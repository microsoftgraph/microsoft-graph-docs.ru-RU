---
title: Тип ресурса profilePhoto
description: Фотография профиля пользователя, группы или контакта Outlook, доступ к которым осуществляется с помощью Exchange Online или Azure Active Directory (AAD). Это двоичные данные, не представленные в кодировке base-64.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: eee47378343aef1b0a471ac186099d4598124862
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965679"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="9363a-104">Тип ресурса profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9363a-104">profilePhoto resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9363a-105">Фотография профиля пользователя, группы или контакта Outlook, доступ к которым осуществляется с помощью Exchange Online или Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="9363a-105">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="9363a-106">Это двоичные данные, не представленные в кодировке base-64.</span><span class="sxs-lookup"><span data-stu-id="9363a-106">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="9363a-107">Поддерживаемые размеры фотографий в формате HD для Exchange Online: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 и 648x648.</span><span class="sxs-lookup"><span data-stu-id="9363a-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="9363a-108">В AAD фотографии могут быть любыми измерениями.</span><span class="sxs-lookup"><span data-stu-id="9363a-108">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="9363a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="9363a-109">Methods</span></span>

| <span data-ttu-id="9363a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="9363a-110">Method</span></span>       | <span data-ttu-id="9363a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9363a-111">Return Type</span></span>  |<span data-ttu-id="9363a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9363a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9363a-113">Получение объекта profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9363a-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="9363a-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9363a-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="9363a-115">Получение указанного объекта **profilePhoto** или его метаданных (свойств **profilePhoto**).</span><span class="sxs-lookup"><span data-stu-id="9363a-115">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="9363a-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="9363a-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="9363a-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9363a-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="9363a-p104">Назначение фотографии указанному пользователю, группе или контакту. Фотография должна быть представлена в двоичном формате. Она заменяет текущую фотографию (если она существует).</span><span class="sxs-lookup"><span data-stu-id="9363a-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="9363a-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="9363a-121">Properties</span></span>
| <span data-ttu-id="9363a-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="9363a-122">Property</span></span>     | <span data-ttu-id="9363a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9363a-123">Type</span></span>   |<span data-ttu-id="9363a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9363a-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9363a-125">id</span><span class="sxs-lookup"><span data-stu-id="9363a-125">id</span></span>|<span data-ttu-id="9363a-126">string</span><span class="sxs-lookup"><span data-stu-id="9363a-126">string</span></span>|<span data-ttu-id="9363a-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9363a-127">Read-only.</span></span>|
|<span data-ttu-id="9363a-128">height</span><span class="sxs-lookup"><span data-stu-id="9363a-128">height</span></span>|<span data-ttu-id="9363a-129">int32</span><span class="sxs-lookup"><span data-stu-id="9363a-129">int32</span></span>|<span data-ttu-id="9363a-p105">Высота фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9363a-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="9363a-132">width</span><span class="sxs-lookup"><span data-stu-id="9363a-132">width</span></span>|<span data-ttu-id="9363a-133">int32</span><span class="sxs-lookup"><span data-stu-id="9363a-133">int32</span></span>|<span data-ttu-id="9363a-p106">Ширина фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9363a-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9363a-136">Связи</span><span class="sxs-lookup"><span data-stu-id="9363a-136">Relationships</span></span>
<span data-ttu-id="9363a-137">Нет</span><span class="sxs-lookup"><span data-stu-id="9363a-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9363a-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9363a-138">JSON representation</span></span>

<span data-ttu-id="9363a-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9363a-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
