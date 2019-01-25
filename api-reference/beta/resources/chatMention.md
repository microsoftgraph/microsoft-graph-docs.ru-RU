---
title: Тип ресурса chatMessageMention
description: 'Представляет упоминаются в сущности chatMessage. Упоминание может быть пользователь, группа, программа-робот или канала. '
localization_priority: Normal
ms.openlocfilehash: f37374a9793000ba641ed772e5dbfca5c0f1bd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515351"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="06a28-104">Тип ресурса chatMessageMention</span><span class="sxs-lookup"><span data-stu-id="06a28-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06a28-105">Представляет упоминаются в сущности [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="06a28-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="06a28-106">Упоминание может быть пользователь, группа, программа-робот или канала.</span><span class="sxs-lookup"><span data-stu-id="06a28-106">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="06a28-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="06a28-107">Properties</span></span>
| <span data-ttu-id="06a28-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="06a28-108">Property</span></span>     | <span data-ttu-id="06a28-109">Тип</span><span class="sxs-lookup"><span data-stu-id="06a28-109">Type</span></span>   |<span data-ttu-id="06a28-110">Описание</span><span class="sxs-lookup"><span data-stu-id="06a28-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06a28-111">id</span><span class="sxs-lookup"><span data-stu-id="06a28-111">id</span></span>|<span data-ttu-id="06a28-112">string</span><span class="sxs-lookup"><span data-stu-id="06a28-112">string</span></span>|<span data-ttu-id="06a28-113">Идентификатор сущности упоминаемые</span><span class="sxs-lookup"><span data-stu-id="06a28-113">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="06a28-114">mentionText</span><span class="sxs-lookup"><span data-stu-id="06a28-114">mentionText</span></span>|<span data-ttu-id="06a28-115">string</span><span class="sxs-lookup"><span data-stu-id="06a28-115">string</span></span>|<span data-ttu-id="06a28-116">Строка, используемая для представления упоминание Ex: отображаемое имя пользователя, имя группы и т.д.</span><span class="sxs-lookup"><span data-stu-id="06a28-116">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="06a28-117">упомянутые</span><span class="sxs-lookup"><span data-stu-id="06a28-117">mentioned</span></span>|[<span data-ttu-id="06a28-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="06a28-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="06a28-119">Пользователь, который был упомянут</span><span class="sxs-lookup"><span data-stu-id="06a28-119">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06a28-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06a28-120">JSON representation</span></span>

<span data-ttu-id="06a28-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06a28-121">The following is a JSON representation of the resource.</span></span>

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
    "Error: /api-reference/beta/resources/chatMention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
