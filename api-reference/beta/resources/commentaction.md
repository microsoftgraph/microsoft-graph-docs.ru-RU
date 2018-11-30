---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
ms.openlocfilehash: 92dc26945cd591de2ba107907a593159f1e128c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082497"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="c3a69-102">Тип ресурса CommentAction</span><span class="sxs-lookup"><span data-stu-id="c3a69-102">CommentAction resource type</span></span>

> <span data-ttu-id="c3a69-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3a69-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3a69-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a69-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3a69-105">В ресурсе **CommentAction** содержатся сведения о [действии][] добавления комментария, выполненном над элементом.</span><span class="sxs-lookup"><span data-stu-id="c3a69-105">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c3a69-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c3a69-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c3a69-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3a69-108">Properties</span></span>

| <span data-ttu-id="c3a69-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c3a69-109">Property name</span></span>    | <span data-ttu-id="c3a69-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c3a69-110">Type</span></span>                       | <span data-ttu-id="c3a69-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3a69-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="c3a69-112">isReply</span><span class="sxs-lookup"><span data-stu-id="c3a69-112">isReply</span></span>          | <span data-ttu-id="c3a69-113">boolean</span><span class="sxs-lookup"><span data-stu-id="c3a69-113">boolean</span></span>                    | <span data-ttu-id="c3a69-114">Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.</span><span class="sxs-lookup"><span data-stu-id="c3a69-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="c3a69-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="c3a69-115">parentAuthor</span></span>     | <span data-ttu-id="c3a69-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c3a69-116">[identitySet][]</span></span>            | <span data-ttu-id="c3a69-117">Удостоверение пользователя, начавшего ветвь комментариев.</span><span class="sxs-lookup"><span data-stu-id="c3a69-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="c3a69-118">participants</span><span class="sxs-lookup"><span data-stu-id="c3a69-118">participants</span></span>     | <span data-ttu-id="c3a69-119">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c3a69-119">[identitySet][] collection</span></span> | <span data-ttu-id="c3a69-120">Удостоверения пользователей, участвующих в ветви комментариев.</span><span class="sxs-lookup"><span data-stu-id="c3a69-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="c3a69-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="c3a69-122">Remarks</span></span>

<span data-ttu-id="c3a69-123">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c3a69-123">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction"
} -->
