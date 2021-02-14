---
author: daspek
title: Тип ресурса commentAction
description: Объект commentAction предоставляет сведения о комментарии к элементу.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f2f3ab7f0798ee1020b107c38262a912fdae53ef
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238416"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="1fc4e-103">Тип ресурса commentAction</span><span class="sxs-lookup"><span data-stu-id="1fc4e-103">commentAction resource type</span></span>

<span data-ttu-id="1fc4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fc4e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1fc4e-105">Ресурс **commentAction** предоставляет сведения о действии при [комментарии][] к элементу.</span><span class="sxs-lookup"><span data-stu-id="1fc4e-105">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="1fc4e-106">**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1fc4e-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="1fc4e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fc4e-108">Properties</span></span>

| <span data-ttu-id="1fc4e-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1fc4e-109">Property name</span></span>    | <span data-ttu-id="1fc4e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1fc4e-110">Type</span></span>                       | <span data-ttu-id="1fc4e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1fc4e-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="1fc4e-112">isReply</span><span class="sxs-lookup"><span data-stu-id="1fc4e-112">isReply</span></span>          | <span data-ttu-id="1fc4e-113">boolean</span><span class="sxs-lookup"><span data-stu-id="1fc4e-113">boolean</span></span>                    | <span data-ttu-id="1fc4e-114">Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.</span><span class="sxs-lookup"><span data-stu-id="1fc4e-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="1fc4e-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="1fc4e-115">parentAuthor</span></span>     | <span data-ttu-id="1fc4e-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1fc4e-116">[identitySet][]</span></span>            | <span data-ttu-id="1fc4e-117">Удостоверение пользователя, начавшего ветвь комментариев.</span><span class="sxs-lookup"><span data-stu-id="1fc4e-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="1fc4e-118">participants</span><span class="sxs-lookup"><span data-stu-id="1fc4e-118">participants</span></span>     | <span data-ttu-id="1fc4e-119">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1fc4e-119">[identitySet][] collection</span></span> | <span data-ttu-id="1fc4e-120">Удостоверения пользователей, участвующих в ветви комментариев.</span><span class="sxs-lookup"><span data-stu-id="1fc4e-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="1fc4e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1fc4e-122">JSON representation</span></span>

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

