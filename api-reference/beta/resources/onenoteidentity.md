---
title: Тип ресурса Оненотеидентити
description: '**Поддержка скоро**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f1b03ad907a0b8f6f3cf2674d74f1ee8722357ea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525028"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="7d7f6-103">Тип ресурса Оненотеидентити</span><span class="sxs-lookup"><span data-stu-id="7d7f6-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d7f6-104">**Поддержка скоро**</span><span class="sxs-lookup"><span data-stu-id="7d7f6-104">**Support coming soon**</span></span>

<span data-ttu-id="7d7f6-105">Тип Оненотеидентити представляет идентификатор _пользователя_.</span><span class="sxs-lookup"><span data-stu-id="7d7f6-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="7d7f6-106">В дальнейшем этот тип будет объединен с удостоверением [](identity.md)</span><span class="sxs-lookup"><span data-stu-id="7d7f6-106">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="7d7f6-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7d7f6-107">JSON representation</span></span>

<span data-ttu-id="7d7f6-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d7f6-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7d7f6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d7f6-109">Properties</span></span>
| <span data-ttu-id="7d7f6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d7f6-110">Property</span></span>     | <span data-ttu-id="7d7f6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7d7f6-111">Type</span></span>   |<span data-ttu-id="7d7f6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7d7f6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d7f6-113">displayName</span><span class="sxs-lookup"><span data-stu-id="7d7f6-113">displayName</span></span>|<span data-ttu-id="7d7f6-114">string</span><span class="sxs-lookup"><span data-stu-id="7d7f6-114">string</span></span>|<span data-ttu-id="7d7f6-115">Отображаемое имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7d7f6-115">The identity's display name.</span></span>|
|<span data-ttu-id="7d7f6-116">id</span><span class="sxs-lookup"><span data-stu-id="7d7f6-116">id</span></span>|<span data-ttu-id="7d7f6-117">строка</span><span class="sxs-lookup"><span data-stu-id="7d7f6-117">string</span></span>|<span data-ttu-id="7d7f6-118">Уникальный идентификатор удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7d7f6-118">Unique identifier for the identity.</span></span>|

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
