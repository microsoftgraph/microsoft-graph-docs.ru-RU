---
title: Тип ресурса oneNoteIdentity
description: '**Поддержка готовится к выпуску**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7ce71775842cc6b7084b86e13e9e4715765567ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963215"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="e8450-103">Тип ресурса oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="e8450-103">oneNoteIdentity resource type</span></span>

> <span data-ttu-id="e8450-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8450-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8450-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8450-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8450-106">**Поддержка готовится к выпуску**</span><span class="sxs-lookup"><span data-stu-id="e8450-106">**Support coming soon**</span></span>

<span data-ttu-id="e8450-107">Тип OneNoteIdentity представляет удостоверение _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="e8450-107">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="e8450-108">В будущем этого типа будут объединены с [удостоверением](identity.md)</span><span class="sxs-lookup"><span data-stu-id="e8450-108">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="e8450-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8450-109">JSON representation</span></span>

<span data-ttu-id="e8450-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8450-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e8450-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8450-111">Properties</span></span>
| <span data-ttu-id="e8450-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8450-112">Property</span></span>     | <span data-ttu-id="e8450-113">Тип</span><span class="sxs-lookup"><span data-stu-id="e8450-113">Type</span></span>   |<span data-ttu-id="e8450-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e8450-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8450-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e8450-115">displayName</span></span>|<span data-ttu-id="e8450-116">строка</span><span class="sxs-lookup"><span data-stu-id="e8450-116">string</span></span>|<span data-ttu-id="e8450-117">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e8450-117">The identity's display name.</span></span>|
|<span data-ttu-id="e8450-118">id</span><span class="sxs-lookup"><span data-stu-id="e8450-118">id</span></span>|<span data-ttu-id="e8450-119">строка</span><span class="sxs-lookup"><span data-stu-id="e8450-119">string</span></span>|<span data-ttu-id="e8450-120">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e8450-120">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
