---
author: daspek
ms.author: dspektor
title: Тип ресурса commentAction
description: Объект commentAction предоставляет сведения о комментариях, сделанных для элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f3720d84624fa728a168515beb28422ab355b335
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531803"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="0908c-103">Тип ресурса commentAction</span><span class="sxs-lookup"><span data-stu-id="0908c-103">commentAction resource type</span></span>

<span data-ttu-id="0908c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0908c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0908c-105">Ресурс **commentAction** предоставляет сведения о [действиях][] с комментариями, выполняемых над элементом.</span><span class="sxs-lookup"><span data-stu-id="0908c-105">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="0908c-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0908c-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="0908c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0908c-108">Properties</span></span>

| <span data-ttu-id="0908c-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0908c-109">Property name</span></span>    | <span data-ttu-id="0908c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0908c-110">Type</span></span>                       | <span data-ttu-id="0908c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0908c-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="0908c-112">isReply</span><span class="sxs-lookup"><span data-stu-id="0908c-112">isReply</span></span>          | <span data-ttu-id="0908c-113">boolean</span><span class="sxs-lookup"><span data-stu-id="0908c-113">boolean</span></span>                    | <span data-ttu-id="0908c-114">Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.</span><span class="sxs-lookup"><span data-stu-id="0908c-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="0908c-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="0908c-115">parentAuthor</span></span>     | <span data-ttu-id="0908c-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0908c-116">[identitySet][]</span></span>            | <span data-ttu-id="0908c-117">Удостоверение пользователя, начавшего ветвь комментариев.</span><span class="sxs-lookup"><span data-stu-id="0908c-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="0908c-118">participants</span><span class="sxs-lookup"><span data-stu-id="0908c-118">participants</span></span>     | <span data-ttu-id="0908c-119">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0908c-119">[identitySet][] collection</span></span> | <span data-ttu-id="0908c-120">Удостоверения пользователей, участвующих в ветви комментариев.</span><span class="sxs-lookup"><span data-stu-id="0908c-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="0908c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0908c-122">JSON representation</span></span>

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
