---
title: Тип ресурса profilePhoto
description: Фотографий профиля пользователя, группы или контакта Outlook доступ из Exchange Online или Azure Active Directory (AAD). Это не кодируются в-64 двоичных данных.
ms.openlocfilehash: 61123542ce66c1e999fb6d90c154a78dbb77df50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075907"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="ac6fb-104">Тип ресурса profilePhoto</span><span class="sxs-lookup"><span data-stu-id="ac6fb-104">profilePhoto resource type</span></span>

> <span data-ttu-id="ac6fb-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ac6fb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac6fb-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac6fb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac6fb-107">Фотографий профиля пользователя, группы или контакта Outlook доступ из Exchange Online или Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="ac6fb-107">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="ac6fb-108">Это не кодируются в-64 двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="ac6fb-108">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="ac6fb-109">Поддерживаемые размеры фотографий в формате HD для Exchange Online: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 и 648x648.</span><span class="sxs-lookup"><span data-stu-id="ac6fb-109">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="ac6fb-110">На AAD фотографии может быть любой измерения.</span><span class="sxs-lookup"><span data-stu-id="ac6fb-110">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="ac6fb-111">Методы</span><span class="sxs-lookup"><span data-stu-id="ac6fb-111">Methods</span></span>

| <span data-ttu-id="ac6fb-112">Метод</span><span class="sxs-lookup"><span data-stu-id="ac6fb-112">Method</span></span>       | <span data-ttu-id="ac6fb-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ac6fb-113">Return Type</span></span>  |<span data-ttu-id="ac6fb-114">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6fb-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac6fb-115">Получение объекта profilePhoto</span><span class="sxs-lookup"><span data-stu-id="ac6fb-115">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="ac6fb-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="ac6fb-116">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="ac6fb-117">Получите указанный **profilePhoto** или метаданных (**profilePhoto** свойства).</span><span class="sxs-lookup"><span data-stu-id="ac6fb-117">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="ac6fb-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="ac6fb-118">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="ac6fb-119">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="ac6fb-119">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="ac6fb-p105">Назначение фотографии указанному пользователю, группе или контакту. Фотография должна быть представлена в двоичном формате. Она заменяет текущую фотографию (если она существует).</span><span class="sxs-lookup"><span data-stu-id="ac6fb-p105">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="ac6fb-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac6fb-123">Properties</span></span>
| <span data-ttu-id="ac6fb-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac6fb-124">Property</span></span>     | <span data-ttu-id="ac6fb-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ac6fb-125">Type</span></span>   |<span data-ttu-id="ac6fb-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6fb-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac6fb-127">id</span><span class="sxs-lookup"><span data-stu-id="ac6fb-127">id</span></span>|<span data-ttu-id="ac6fb-128">строка</span><span class="sxs-lookup"><span data-stu-id="ac6fb-128">string</span></span>|<span data-ttu-id="ac6fb-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac6fb-129">Read-only.</span></span>|
|<span data-ttu-id="ac6fb-130">height</span><span class="sxs-lookup"><span data-stu-id="ac6fb-130">height</span></span>|<span data-ttu-id="ac6fb-131">int32</span><span class="sxs-lookup"><span data-stu-id="ac6fb-131">int32</span></span>|<span data-ttu-id="ac6fb-p106">Высота фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac6fb-p106">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="ac6fb-134">width</span><span class="sxs-lookup"><span data-stu-id="ac6fb-134">width</span></span>|<span data-ttu-id="ac6fb-135">int32</span><span class="sxs-lookup"><span data-stu-id="ac6fb-135">int32</span></span>|<span data-ttu-id="ac6fb-p107">Ширина фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac6fb-p107">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac6fb-138">Связи</span><span class="sxs-lookup"><span data-stu-id="ac6fb-138">Relationships</span></span>
<span data-ttu-id="ac6fb-139">Нет</span><span class="sxs-lookup"><span data-stu-id="ac6fb-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ac6fb-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac6fb-140">JSON representation</span></span>

<span data-ttu-id="ac6fb-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac6fb-141">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
