---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f92c253b400a5164c1def570daef6307c0f4a8bf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876547"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="1b500-103">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="1b500-103">messageRuleActions resource type</span></span>


<span data-ttu-id="1b500-104">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="1b500-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="1b500-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b500-105">Properties</span></span>
| <span data-ttu-id="1b500-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b500-106">Property</span></span>     | <span data-ttu-id="1b500-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1b500-107">Type</span></span>   |<span data-ttu-id="1b500-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1b500-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1b500-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="1b500-109">assignCategories</span></span> | <span data-ttu-id="1b500-110">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1b500-110">String collection</span></span> | <span data-ttu-id="1b500-111">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="1b500-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="1b500-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="1b500-112">copyToFolder</span></span> | <span data-ttu-id="1b500-113">String</span><span class="sxs-lookup"><span data-stu-id="1b500-113">String</span></span> | <span data-ttu-id="1b500-114">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="1b500-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="1b500-115">delete</span><span class="sxs-lookup"><span data-stu-id="1b500-115">delete</span></span> | <span data-ttu-id="1b500-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b500-116">Boolean</span></span> | <span data-ttu-id="1b500-117">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="1b500-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="1b500-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="1b500-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="1b500-119">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="1b500-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="1b500-120">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="1b500-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="1b500-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="1b500-121">forwardTo</span></span> | <span data-ttu-id="1b500-122">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="1b500-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="1b500-123">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="1b500-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="1b500-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="1b500-124">markAsRead</span></span> | <span data-ttu-id="1b500-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b500-125">Boolean</span></span> | <span data-ttu-id="1b500-126">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="1b500-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="1b500-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="1b500-127">markImportance</span></span> | <span data-ttu-id="1b500-128">importance</span><span class="sxs-lookup"><span data-stu-id="1b500-128">importance</span></span> | <span data-ttu-id="1b500-129">Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="1b500-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="1b500-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="1b500-130">moveToFolder</span></span> |  <span data-ttu-id="1b500-131">String</span><span class="sxs-lookup"><span data-stu-id="1b500-131">String</span></span>| <span data-ttu-id="1b500-132">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="1b500-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="1b500-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="1b500-133">permanentDelete</span></span> | <span data-ttu-id="1b500-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b500-134">Boolean</span></span> | <span data-ttu-id="1b500-135">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="1b500-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="1b500-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="1b500-136">redirectTo</span></span> | <span data-ttu-id="1b500-137">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="1b500-137">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="1b500-138">Адреса электронной почты, к которым необходимо перенаправить сообщение.</span><span class="sxs-lookup"><span data-stu-id="1b500-138">The email addresses to which a message should be redirected.</span></span> |
| <span data-ttu-id="1b500-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="1b500-139">stopProcessingRules</span></span> | <span data-ttu-id="1b500-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b500-140">Boolean</span></span> | <span data-ttu-id="1b500-141">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="1b500-141">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1b500-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b500-142">JSON representation</span></span>
<span data-ttu-id="1b500-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b500-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
