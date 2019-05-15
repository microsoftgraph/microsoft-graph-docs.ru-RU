---
author: daspek
ms.author: dspektor
title: Тип ресурса commentAction
description: Объект commentAction предоставляет сведения о комментариях, сделанных для элемента.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 12e6cd68d5809b8e4c1765234eeb77b40b30a78e
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970789"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="9b36f-103">Тип ресурса commentAction</span><span class="sxs-lookup"><span data-stu-id="9b36f-103">commentAction resource type</span></span>

<span data-ttu-id="9b36f-104">Ресурс **commentAction** предоставляет сведения о действиях с [][] комментариями, выполняемых над элементом.</span><span class="sxs-lookup"><span data-stu-id="9b36f-104">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="9b36f-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9b36f-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="9b36f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b36f-107">Properties</span></span>

| <span data-ttu-id="9b36f-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9b36f-108">Property name</span></span>    | <span data-ttu-id="9b36f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9b36f-109">Type</span></span>                       | <span data-ttu-id="9b36f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9b36f-110">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="9b36f-111">isReply</span><span class="sxs-lookup"><span data-stu-id="9b36f-111">isReply</span></span>          | <span data-ttu-id="9b36f-112">boolean</span><span class="sxs-lookup"><span data-stu-id="9b36f-112">boolean</span></span>                    | <span data-ttu-id="9b36f-113">Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.</span><span class="sxs-lookup"><span data-stu-id="9b36f-113">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="9b36f-114">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="9b36f-114">parentAuthor</span></span>     | <span data-ttu-id="9b36f-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9b36f-115">[identitySet][]</span></span>            | <span data-ttu-id="9b36f-116">Удостоверение пользователя, начавшего ветвь комментариев.</span><span class="sxs-lookup"><span data-stu-id="9b36f-116">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="9b36f-117">participants</span><span class="sxs-lookup"><span data-stu-id="9b36f-117">participants</span></span>     | <span data-ttu-id="9b36f-118">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9b36f-118">[identitySet][] collection</span></span> | <span data-ttu-id="9b36f-119">Удостоверения пользователей, участвующих в ветви комментариев.</span><span class="sxs-lookup"><span data-stu-id="9b36f-119">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="9b36f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b36f-121">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "The commentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/commentAction",
  "suppressions": []
}
-->
