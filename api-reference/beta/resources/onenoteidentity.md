---
title: Тип ресурса oneNoteIdentity
description: '**Поддержка готовится к выпуску**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 33cb7d63ab103723ae5bb8d24c19add4bb7ef5ac
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576880"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="45bd0-103">Тип ресурса oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="45bd0-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45bd0-104">**Поддержка готовится к выпуску**</span><span class="sxs-lookup"><span data-stu-id="45bd0-104">**Support coming soon**</span></span>

<span data-ttu-id="45bd0-105">Тип OneNoteIdentity представляет удостоверение _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="45bd0-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="45bd0-106">В будущем этого типа будут объединены с [удостоверением](identity.md)</span><span class="sxs-lookup"><span data-stu-id="45bd0-106">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="45bd0-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45bd0-107">JSON representation</span></span>

<span data-ttu-id="45bd0-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45bd0-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oneNoteIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="45bd0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="45bd0-109">Properties</span></span>
| <span data-ttu-id="45bd0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="45bd0-110">Property</span></span>     | <span data-ttu-id="45bd0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="45bd0-111">Type</span></span>   |<span data-ttu-id="45bd0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="45bd0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45bd0-113">displayName</span><span class="sxs-lookup"><span data-stu-id="45bd0-113">displayName</span></span>|<span data-ttu-id="45bd0-114">string</span><span class="sxs-lookup"><span data-stu-id="45bd0-114">string</span></span>|<span data-ttu-id="45bd0-115">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="45bd0-115">The identity's display name.</span></span>|
|<span data-ttu-id="45bd0-116">id</span><span class="sxs-lookup"><span data-stu-id="45bd0-116">id</span></span>|<span data-ttu-id="45bd0-117">string</span><span class="sxs-lookup"><span data-stu-id="45bd0-117">string</span></span>|<span data-ttu-id="45bd0-118">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="45bd0-118">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
