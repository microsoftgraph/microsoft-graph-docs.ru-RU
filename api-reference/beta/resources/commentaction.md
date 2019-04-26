---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: c472a0b1b992c91b60174859e4900ffcee04c007
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341484"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="b6851-102">Тип ресурса CommentAction</span><span class="sxs-lookup"><span data-stu-id="b6851-102">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6851-103">В ресурсе **CommentAction** содержатся сведения о [действии][] добавления комментария, выполненном над элементом.</span><span class="sxs-lookup"><span data-stu-id="b6851-103">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b6851-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b6851-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b6851-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6851-106">Properties</span></span>

| <span data-ttu-id="b6851-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b6851-107">Property name</span></span>    | <span data-ttu-id="b6851-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b6851-108">Type</span></span>                       | <span data-ttu-id="b6851-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b6851-109">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="b6851-110">isReply</span><span class="sxs-lookup"><span data-stu-id="b6851-110">isReply</span></span>          | <span data-ttu-id="b6851-111">boolean</span><span class="sxs-lookup"><span data-stu-id="b6851-111">boolean</span></span>                    | <span data-ttu-id="b6851-112">Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.</span><span class="sxs-lookup"><span data-stu-id="b6851-112">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="b6851-113">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="b6851-113">parentAuthor</span></span>     | <span data-ttu-id="b6851-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b6851-114">[identitySet][]</span></span>            | <span data-ttu-id="b6851-115">Удостоверение пользователя, начавшего ветвь комментариев.</span><span class="sxs-lookup"><span data-stu-id="b6851-115">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="b6851-116">participants</span><span class="sxs-lookup"><span data-stu-id="b6851-116">participants</span></span>     | <span data-ttu-id="b6851-117">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b6851-117">[identitySet][] collection</span></span> | <span data-ttu-id="b6851-118">Удостоверения пользователей, участвующих в ветви комментариев.</span><span class="sxs-lookup"><span data-stu-id="b6851-118">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="b6851-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="b6851-120">Remarks</span></span>

<span data-ttu-id="b6851-121">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b6851-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": []
}
-->
