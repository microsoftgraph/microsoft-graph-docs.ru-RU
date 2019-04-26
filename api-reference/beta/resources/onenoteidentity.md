---
title: Тип ресурса Оненотеидентити
description: '**Поддержка скоро**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ee5eb0db40516e1069fe8e40a8711cf97ae18eaa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341500"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="f481f-103">Тип ресурса Оненотеидентити</span><span class="sxs-lookup"><span data-stu-id="f481f-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f481f-104">**Поддержка скоро**</span><span class="sxs-lookup"><span data-stu-id="f481f-104">**Support coming soon**</span></span>

<span data-ttu-id="f481f-105">Тип Оненотеидентити представляет идентификатор _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="f481f-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="f481f-106">В дальнейшем этот тип будет объединен с удостоверением [](identity.md)</span><span class="sxs-lookup"><span data-stu-id="f481f-106">In future, this type will be merged with [identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="f481f-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f481f-107">JSON representation</span></span>

<span data-ttu-id="f481f-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f481f-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f481f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f481f-109">Properties</span></span>
| <span data-ttu-id="f481f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f481f-110">Property</span></span>     | <span data-ttu-id="f481f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f481f-111">Type</span></span>   |<span data-ttu-id="f481f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f481f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f481f-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f481f-113">displayName</span></span>|<span data-ttu-id="f481f-114">string</span><span class="sxs-lookup"><span data-stu-id="f481f-114">string</span></span>|<span data-ttu-id="f481f-115">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f481f-115">The identity's display name.</span></span>|
|<span data-ttu-id="f481f-116">id</span><span class="sxs-lookup"><span data-stu-id="f481f-116">id</span></span>|<span data-ttu-id="f481f-117">строка</span><span class="sxs-lookup"><span data-stu-id="f481f-117">string</span></span>|<span data-ttu-id="f481f-118">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f481f-118">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
