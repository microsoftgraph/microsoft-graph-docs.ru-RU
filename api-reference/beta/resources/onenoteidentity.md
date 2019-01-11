---
title: Тип ресурса oneNoteIdentity
description: '**Поддержка готовится к выпуску**'
localization_priority: Normal
ms.openlocfilehash: 80d0719bd2770b715902b5c600fe65012e0064d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883890"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="a9740-103">Тип ресурса oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="a9740-103">oneNoteIdentity resource type</span></span>

> <span data-ttu-id="a9740-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a9740-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9740-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9740-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9740-106">**Поддержка готовится к выпуску**</span><span class="sxs-lookup"><span data-stu-id="a9740-106">**Support coming soon**</span></span>

<span data-ttu-id="a9740-107">Тип OneNoteIdentity представляет удостоверение _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="a9740-107">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="a9740-108">В будущем этого типа будут объединены с [удостоверением](identity.md)</span><span class="sxs-lookup"><span data-stu-id="a9740-108">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="a9740-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9740-109">JSON representation</span></span>

<span data-ttu-id="a9740-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9740-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="a9740-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9740-111">Properties</span></span>
| <span data-ttu-id="a9740-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9740-112">Property</span></span>     | <span data-ttu-id="a9740-113">Тип</span><span class="sxs-lookup"><span data-stu-id="a9740-113">Type</span></span>   |<span data-ttu-id="a9740-114">Описание</span><span class="sxs-lookup"><span data-stu-id="a9740-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9740-115">displayName</span><span class="sxs-lookup"><span data-stu-id="a9740-115">displayName</span></span>|<span data-ttu-id="a9740-116">строка</span><span class="sxs-lookup"><span data-stu-id="a9740-116">string</span></span>|<span data-ttu-id="a9740-117">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a9740-117">The identity's display name.</span></span>|
|<span data-ttu-id="a9740-118">id</span><span class="sxs-lookup"><span data-stu-id="a9740-118">id</span></span>|<span data-ttu-id="a9740-119">строка</span><span class="sxs-lookup"><span data-stu-id="a9740-119">string</span></span>|<span data-ttu-id="a9740-120">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a9740-120">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
