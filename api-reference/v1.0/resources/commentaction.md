---
author: daspek
ms.author: dspektor
title: Тип ресурса commentAction
description: Объект commentAction предоставляет сведения о комментариях, сделанных для элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f1632847461b1aa0cde429edfc4d8c5cff11ee3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988333"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="0b74a-103">Тип ресурса commentAction</span><span class="sxs-lookup"><span data-stu-id="0b74a-103">commentAction resource type</span></span>

<span data-ttu-id="0b74a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b74a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b74a-105">Ресурс **commentAction** предоставляет сведения о [действиях][] с комментариями, выполняемых над элементом.</span><span class="sxs-lookup"><span data-stu-id="0b74a-105">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="0b74a-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0b74a-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="0b74a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b74a-108">Properties</span></span>

| <span data-ttu-id="0b74a-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0b74a-109">Property name</span></span>    | <span data-ttu-id="0b74a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0b74a-110">Type</span></span>                       | <span data-ttu-id="0b74a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0b74a-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="0b74a-112">isReply</span><span class="sxs-lookup"><span data-stu-id="0b74a-112">isReply</span></span>          | <span data-ttu-id="0b74a-113">boolean</span><span class="sxs-lookup"><span data-stu-id="0b74a-113">boolean</span></span>                    | <span data-ttu-id="0b74a-114">Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.</span><span class="sxs-lookup"><span data-stu-id="0b74a-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="0b74a-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="0b74a-115">parentAuthor</span></span>     | <span data-ttu-id="0b74a-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0b74a-116">[identitySet][]</span></span>            | <span data-ttu-id="0b74a-117">Удостоверение пользователя, начавшего ветвь комментариев.</span><span class="sxs-lookup"><span data-stu-id="0b74a-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="0b74a-118">participants</span><span class="sxs-lookup"><span data-stu-id="0b74a-118">participants</span></span>     | <span data-ttu-id="0b74a-119">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0b74a-119">[identitySet][] collection</span></span> | <span data-ttu-id="0b74a-120">Удостоверения пользователей, участвующих в ветви комментариев.</span><span class="sxs-lookup"><span data-stu-id="0b74a-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="0b74a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b74a-122">JSON representation</span></span>

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

