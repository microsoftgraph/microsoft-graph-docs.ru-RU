---
author: daspek
description: В ресурсе CommentAction содержатся сведения о действии добавления комментария, выполненном над элементом.
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7782c6e4dd30b503a9be88737ef6bd2dbad109b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973260"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="126cb-103">Тип ресурса CommentAction</span><span class="sxs-lookup"><span data-stu-id="126cb-103">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="126cb-104">В ресурсе **CommentAction** содержатся сведения о [действии][] добавления комментария, выполненном над элементом.</span><span class="sxs-lookup"><span data-stu-id="126cb-104">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="126cb-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="126cb-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="126cb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="126cb-107">Properties</span></span>

| <span data-ttu-id="126cb-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="126cb-108">Property name</span></span>    | <span data-ttu-id="126cb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="126cb-109">Type</span></span>                       | <span data-ttu-id="126cb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="126cb-110">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="126cb-111">isReply</span><span class="sxs-lookup"><span data-stu-id="126cb-111">isReply</span></span>          | <span data-ttu-id="126cb-112">boolean</span><span class="sxs-lookup"><span data-stu-id="126cb-112">boolean</span></span>                    | <span data-ttu-id="126cb-113">Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.</span><span class="sxs-lookup"><span data-stu-id="126cb-113">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="126cb-114">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="126cb-114">parentAuthor</span></span>     | <span data-ttu-id="126cb-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="126cb-115">[identitySet][]</span></span>            | <span data-ttu-id="126cb-116">Удостоверение пользователя, начавшего ветвь комментариев.</span><span class="sxs-lookup"><span data-stu-id="126cb-116">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="126cb-117">participants</span><span class="sxs-lookup"><span data-stu-id="126cb-117">participants</span></span>     | <span data-ttu-id="126cb-118">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="126cb-118">[identitySet][] collection</span></span> | <span data-ttu-id="126cb-119">Удостоверения пользователей, участвующих в ветви комментариев.</span><span class="sxs-lookup"><span data-stu-id="126cb-119">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="126cb-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="126cb-121">Remarks</span></span>

<span data-ttu-id="126cb-122">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="126cb-122">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
