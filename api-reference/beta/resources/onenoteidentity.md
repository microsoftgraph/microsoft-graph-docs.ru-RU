---
title: Тип ресурса oneNoteIdentity
description: '**Поддержка готовится к выпуску**'
ms.openlocfilehash: 09c4ee9882a420fb07c6a51be5f361b601573969
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081414"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="4b2c5-103">Тип ресурса oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="4b2c5-103">oneNoteIdentity resource type</span></span>

> <span data-ttu-id="4b2c5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b2c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b2c5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b2c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b2c5-106">**Поддержка готовится к выпуску**</span><span class="sxs-lookup"><span data-stu-id="4b2c5-106">**Support coming soon**</span></span>

<span data-ttu-id="4b2c5-107">Тип OneNoteIdentity представляет удостоверение _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="4b2c5-107">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="4b2c5-108">В будущем этого типа будут объединены с [удостоверением](identity.md)</span><span class="sxs-lookup"><span data-stu-id="4b2c5-108">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="4b2c5-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b2c5-109">JSON representation</span></span>

<span data-ttu-id="4b2c5-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b2c5-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="4b2c5-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b2c5-111">Properties</span></span>
| <span data-ttu-id="4b2c5-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b2c5-112">Property</span></span>     | <span data-ttu-id="4b2c5-113">Тип</span><span class="sxs-lookup"><span data-stu-id="4b2c5-113">Type</span></span>   |<span data-ttu-id="4b2c5-114">Описание</span><span class="sxs-lookup"><span data-stu-id="4b2c5-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b2c5-115">displayName</span><span class="sxs-lookup"><span data-stu-id="4b2c5-115">displayName</span></span>|<span data-ttu-id="4b2c5-116">строка</span><span class="sxs-lookup"><span data-stu-id="4b2c5-116">string</span></span>|<span data-ttu-id="4b2c5-117">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4b2c5-117">The identity's display name.</span></span>|
|<span data-ttu-id="4b2c5-118">id</span><span class="sxs-lookup"><span data-stu-id="4b2c5-118">id</span></span>|<span data-ttu-id="4b2c5-119">строка</span><span class="sxs-lookup"><span data-stu-id="4b2c5-119">string</span></span>|<span data-ttu-id="4b2c5-120">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4b2c5-120">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
