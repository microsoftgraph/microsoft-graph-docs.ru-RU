---
author: daspek
description: В ресурсе CommentAction содержатся сведения о действии добавления комментария, выполненном над элементом.
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f09785ae438225aa109a3b6a30790546cf3f30c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033988"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="c8b2e-103">Тип ресурса CommentAction</span><span class="sxs-lookup"><span data-stu-id="c8b2e-103">CommentAction resource type</span></span>

<span data-ttu-id="c8b2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8b2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8b2e-105">В ресурсе **CommentAction** содержатся сведения о [действии][] добавления комментария, выполненном над элементом.</span><span class="sxs-lookup"><span data-stu-id="c8b2e-105">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c8b2e-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c8b2e-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c8b2e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8b2e-108">Properties</span></span>

| <span data-ttu-id="c8b2e-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c8b2e-109">Property name</span></span>    | <span data-ttu-id="c8b2e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c8b2e-110">Type</span></span>                       | <span data-ttu-id="c8b2e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c8b2e-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="c8b2e-112">isReply</span><span class="sxs-lookup"><span data-stu-id="c8b2e-112">isReply</span></span>          | <span data-ttu-id="c8b2e-113">boolean</span><span class="sxs-lookup"><span data-stu-id="c8b2e-113">boolean</span></span>                    | <span data-ttu-id="c8b2e-114">Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.</span><span class="sxs-lookup"><span data-stu-id="c8b2e-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="c8b2e-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="c8b2e-115">parentAuthor</span></span>     | <span data-ttu-id="c8b2e-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c8b2e-116">[identitySet][]</span></span>            | <span data-ttu-id="c8b2e-117">Удостоверение пользователя, начавшего ветвь комментариев.</span><span class="sxs-lookup"><span data-stu-id="c8b2e-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="c8b2e-118">participants</span><span class="sxs-lookup"><span data-stu-id="c8b2e-118">participants</span></span>     | <span data-ttu-id="c8b2e-119">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c8b2e-119">[identitySet][] collection</span></span> | <span data-ttu-id="c8b2e-120">Удостоверения пользователей, участвующих в ветви комментариев.</span><span class="sxs-lookup"><span data-stu-id="c8b2e-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="c8b2e-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="c8b2e-122">Remarks</span></span>

<span data-ttu-id="c8b2e-123">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c8b2e-123">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


