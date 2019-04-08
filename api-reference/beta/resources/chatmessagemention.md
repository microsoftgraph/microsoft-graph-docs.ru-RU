---
title: Тип ресурса Чатмессажементион
description: 'Представляет упоминание в объекте chatMessage. Упоминание может быть у пользователя, группы, ленты или канала. '
localization_priority: Normal
ms.openlocfilehash: 45b4c60e22f727210150a64078935741dfb71640
ms.sourcegitcommit: 953895b28b6bae6e17eead938565fde289c49ef7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2019
ms.locfileid: "31481372"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="a2924-104">Тип ресурса Чатмессажементион</span><span class="sxs-lookup"><span data-stu-id="a2924-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2924-105">Представляет упоминание в объекте [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="a2924-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="a2924-106">Упоминание может быть у пользователя, группы, ленты или канала.</span><span class="sxs-lookup"><span data-stu-id="a2924-106">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="a2924-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2924-107">Properties</span></span>
| <span data-ttu-id="a2924-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2924-108">Property</span></span>     | <span data-ttu-id="a2924-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a2924-109">Type</span></span>   |<span data-ttu-id="a2924-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a2924-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2924-111">id</span><span class="sxs-lookup"><span data-stu-id="a2924-111">id</span></span>|<span data-ttu-id="a2924-112">string</span><span class="sxs-lookup"><span data-stu-id="a2924-112">string</span></span>|<span data-ttu-id="a2924-113">Идентификатор упоминаемого объекта</span><span class="sxs-lookup"><span data-stu-id="a2924-113">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="a2924-114">Ментионтекст</span><span class="sxs-lookup"><span data-stu-id="a2924-114">mentionText</span></span>|<span data-ttu-id="a2924-115">string</span><span class="sxs-lookup"><span data-stu-id="a2924-115">string</span></span>|<span data-ttu-id="a2924-116">Строка, представляющая упоминание ex: отображаемое имя пользователя, имя группы и т. д.</span><span class="sxs-lookup"><span data-stu-id="a2924-116">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="a2924-117">котором</span><span class="sxs-lookup"><span data-stu-id="a2924-117">mentioned</span></span>|[<span data-ttu-id="a2924-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="a2924-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="a2924-119">Пользователь, который упоминал</span><span class="sxs-lookup"><span data-stu-id="a2924-119">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2924-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a2924-120">JSON representation</span></span>

<span data-ttu-id="a2924-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2924-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessagemention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
