---
title: Тип ресурса profilePhoto
description: Фотографий профиля пользователя, группы или контакта Outlook доступ из Exchange Online или Azure Active Directory (AAD). Это не кодируются в-64 двоичных данных.
localization_priority: Normal
ms.openlocfilehash: 2a831abd098fb9a0dfa95f6d6dd3a9cd5de128cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513657"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="0bdb4-104">Тип ресурса profilePhoto</span><span class="sxs-lookup"><span data-stu-id="0bdb4-104">profilePhoto resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bdb4-105">Фотографий профиля пользователя, группы или контакта Outlook доступ из Exchange Online или Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="0bdb4-105">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="0bdb4-106">Это не кодируются в-64 двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="0bdb4-106">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="0bdb4-107">Поддерживаемые размеры фотографий в формате HD для Exchange Online: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 и 648x648.</span><span class="sxs-lookup"><span data-stu-id="0bdb4-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="0bdb4-108">На AAD фотографии может быть любой измерения.</span><span class="sxs-lookup"><span data-stu-id="0bdb4-108">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="0bdb4-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0bdb4-109">Methods</span></span>

| <span data-ttu-id="0bdb4-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0bdb4-110">Method</span></span>       | <span data-ttu-id="0bdb4-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0bdb4-111">Return Type</span></span>  |<span data-ttu-id="0bdb4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0bdb4-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0bdb4-113">Получение объекта profilePhoto</span><span class="sxs-lookup"><span data-stu-id="0bdb4-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="0bdb4-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="0bdb4-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="0bdb4-115">Получите указанный **profilePhoto** или метаданных (**profilePhoto** свойства).</span><span class="sxs-lookup"><span data-stu-id="0bdb4-115">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="0bdb4-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="0bdb4-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="0bdb4-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="0bdb4-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="0bdb4-p104">Назначение фотографии указанному пользователю, группе или контакту. Фотография должна быть представлена в двоичном формате. Она заменяет текущую фотографию (если она существует).</span><span class="sxs-lookup"><span data-stu-id="0bdb4-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="0bdb4-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bdb4-121">Properties</span></span>
| <span data-ttu-id="0bdb4-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bdb4-122">Property</span></span>     | <span data-ttu-id="0bdb4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0bdb4-123">Type</span></span>   |<span data-ttu-id="0bdb4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0bdb4-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bdb4-125">id</span><span class="sxs-lookup"><span data-stu-id="0bdb4-125">id</span></span>|<span data-ttu-id="0bdb4-126">string</span><span class="sxs-lookup"><span data-stu-id="0bdb4-126">string</span></span>|<span data-ttu-id="0bdb4-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bdb4-127">Read-only.</span></span>|
|<span data-ttu-id="0bdb4-128">height</span><span class="sxs-lookup"><span data-stu-id="0bdb4-128">height</span></span>|<span data-ttu-id="0bdb4-129">int32</span><span class="sxs-lookup"><span data-stu-id="0bdb4-129">int32</span></span>|<span data-ttu-id="0bdb4-p105">Высота фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bdb4-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="0bdb4-132">width</span><span class="sxs-lookup"><span data-stu-id="0bdb4-132">width</span></span>|<span data-ttu-id="0bdb4-133">int32</span><span class="sxs-lookup"><span data-stu-id="0bdb4-133">int32</span></span>|<span data-ttu-id="0bdb4-p106">Ширина фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bdb4-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bdb4-136">Связи</span><span class="sxs-lookup"><span data-stu-id="0bdb4-136">Relationships</span></span>
<span data-ttu-id="0bdb4-137">Нет</span><span class="sxs-lookup"><span data-stu-id="0bdb4-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0bdb4-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0bdb4-138">JSON representation</span></span>

<span data-ttu-id="0bdb4-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bdb4-139">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/profilephoto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
