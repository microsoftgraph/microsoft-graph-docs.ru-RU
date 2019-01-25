---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: e674c996002b3a54c92886dd1c5dca7a76c56b51
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526272"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="24f9b-102">Тип ресурса CommentAction</span><span class="sxs-lookup"><span data-stu-id="24f9b-102">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24f9b-103">В ресурсе **CommentAction** содержатся сведения о [действии][] добавления комментария, выполненном над элементом.</span><span class="sxs-lookup"><span data-stu-id="24f9b-103">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="24f9b-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="24f9b-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="24f9b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="24f9b-106">Properties</span></span>

| <span data-ttu-id="24f9b-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="24f9b-107">Property name</span></span>    | <span data-ttu-id="24f9b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="24f9b-108">Type</span></span>                       | <span data-ttu-id="24f9b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="24f9b-109">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="24f9b-110">isReply</span><span class="sxs-lookup"><span data-stu-id="24f9b-110">isReply</span></span>          | <span data-ttu-id="24f9b-111">boolean</span><span class="sxs-lookup"><span data-stu-id="24f9b-111">boolean</span></span>                    | <span data-ttu-id="24f9b-112">Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.</span><span class="sxs-lookup"><span data-stu-id="24f9b-112">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="24f9b-113">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="24f9b-113">parentAuthor</span></span>     | <span data-ttu-id="24f9b-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="24f9b-114">[identitySet][]</span></span>            | <span data-ttu-id="24f9b-115">Удостоверение пользователя, начавшего ветвь комментариев.</span><span class="sxs-lookup"><span data-stu-id="24f9b-115">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="24f9b-116">participants</span><span class="sxs-lookup"><span data-stu-id="24f9b-116">participants</span></span>     | <span data-ttu-id="24f9b-117">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="24f9b-117">[identitySet][] collection</span></span> | <span data-ttu-id="24f9b-118">Удостоверения пользователей, участвующих в ветви комментариев.</span><span class="sxs-lookup"><span data-stu-id="24f9b-118">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="24f9b-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="24f9b-120">Remarks</span></span>

<span data-ttu-id="24f9b-121">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="24f9b-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/commentaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
