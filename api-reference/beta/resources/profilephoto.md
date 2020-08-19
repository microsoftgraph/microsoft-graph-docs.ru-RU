---
title: Тип ресурса profilePhoto
description: Фотография профиля пользователя, группы или контакта Outlook, доступ к которым осуществляется с помощью Exchange Online или Azure Active Directory (AAD). Двоичные данные, не закодированные в Base – 64.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: dbaff3f61e7c430ae77ec10bea66a9c11dabaf05
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812038"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="c66da-104">Тип ресурса profilePhoto</span><span class="sxs-lookup"><span data-stu-id="c66da-104">profilePhoto resource type</span></span>

<span data-ttu-id="c66da-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c66da-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c66da-p102">Фотография профиля пользователя, группы или контакта Outlook, доступ к которым осуществляется с помощью Exchange Online или Azure Active Directory (AAD). Двоичные данные, не закодированные в Base – 64.</span><span class="sxs-lookup"><span data-stu-id="c66da-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD). It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="c66da-108">Поддерживаемые размеры фотографий в формате HD для Exchange Online: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 и 648x648.</span><span class="sxs-lookup"><span data-stu-id="c66da-108">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="c66da-109">В AAD фотографии могут быть любыми измерениями.</span><span class="sxs-lookup"><span data-stu-id="c66da-109">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="c66da-110">Методы</span><span class="sxs-lookup"><span data-stu-id="c66da-110">Methods</span></span>

| <span data-ttu-id="c66da-111">Метод</span><span class="sxs-lookup"><span data-stu-id="c66da-111">Method</span></span>       | <span data-ttu-id="c66da-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c66da-112">Return Type</span></span>  |<span data-ttu-id="c66da-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c66da-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c66da-114">Получение объекта profilePhoto</span><span class="sxs-lookup"><span data-stu-id="c66da-114">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="c66da-115">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="c66da-115">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="c66da-116">Получение указанного объекта **profilePhoto** или его метаданных (свойств **profilePhoto**).</span><span class="sxs-lookup"><span data-stu-id="c66da-116">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="c66da-117">Обновление</span><span class="sxs-lookup"><span data-stu-id="c66da-117">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="c66da-118">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="c66da-118">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="c66da-p104">Назначение фотографии указанному пользователю, группе или контакту. Фотография должна быть представлена в двоичном формате. Она заменяет текущую фотографию (если она существует).</span><span class="sxs-lookup"><span data-stu-id="c66da-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="c66da-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="c66da-122">Properties</span></span>
| <span data-ttu-id="c66da-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="c66da-123">Property</span></span>     | <span data-ttu-id="c66da-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c66da-124">Type</span></span>   |<span data-ttu-id="c66da-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c66da-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c66da-126">id</span><span class="sxs-lookup"><span data-stu-id="c66da-126">id</span></span>|<span data-ttu-id="c66da-127">string</span><span class="sxs-lookup"><span data-stu-id="c66da-127">string</span></span>|<span data-ttu-id="c66da-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c66da-128">Read-only.</span></span>|
|<span data-ttu-id="c66da-129">height</span><span class="sxs-lookup"><span data-stu-id="c66da-129">height</span></span>|<span data-ttu-id="c66da-130">int32</span><span class="sxs-lookup"><span data-stu-id="c66da-130">int32</span></span>|<span data-ttu-id="c66da-p105">Высота фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c66da-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="c66da-133">width</span><span class="sxs-lookup"><span data-stu-id="c66da-133">width</span></span>|<span data-ttu-id="c66da-134">int32</span><span class="sxs-lookup"><span data-stu-id="c66da-134">int32</span></span>|<span data-ttu-id="c66da-p106">Ширина фотографии. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c66da-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c66da-137">Связи</span><span class="sxs-lookup"><span data-stu-id="c66da-137">Relationships</span></span>
<span data-ttu-id="c66da-138">Нет</span><span class="sxs-lookup"><span data-stu-id="c66da-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c66da-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c66da-139">JSON representation</span></span>

<span data-ttu-id="c66da-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c66da-140">Here is a JSON representation of the resource.</span></span>

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
