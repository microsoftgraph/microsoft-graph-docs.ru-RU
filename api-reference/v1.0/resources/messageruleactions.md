---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
ms.openlocfilehash: bc9051d5857d25e2e163b3ed1d737072fe16b8bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026713"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="aac80-103">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="aac80-103">messageRuleActions resource type</span></span>


<span data-ttu-id="aac80-104">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="aac80-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="aac80-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="aac80-105">Properties</span></span>
| <span data-ttu-id="aac80-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="aac80-106">Property</span></span>     | <span data-ttu-id="aac80-107">Тип</span><span class="sxs-lookup"><span data-stu-id="aac80-107">Type</span></span>   |<span data-ttu-id="aac80-108">Описание</span><span class="sxs-lookup"><span data-stu-id="aac80-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aac80-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="aac80-109">assignCategories</span></span> | <span data-ttu-id="aac80-110">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aac80-110">String collection</span></span> | <span data-ttu-id="aac80-111">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="aac80-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="aac80-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="aac80-112">copyToFolder</span></span> | <span data-ttu-id="aac80-113">String</span><span class="sxs-lookup"><span data-stu-id="aac80-113">String</span></span> | <span data-ttu-id="aac80-114">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="aac80-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="aac80-115">delete</span><span class="sxs-lookup"><span data-stu-id="aac80-115">delete</span></span> | <span data-ttu-id="aac80-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="aac80-116">Boolean</span></span> | <span data-ttu-id="aac80-117">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="aac80-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="aac80-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="aac80-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="aac80-119">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="aac80-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="aac80-120">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="aac80-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="aac80-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="aac80-121">forwardTo</span></span> | <span data-ttu-id="aac80-122">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="aac80-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="aac80-123">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="aac80-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="aac80-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="aac80-124">markAsRead</span></span> | <span data-ttu-id="aac80-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="aac80-125">Boolean</span></span> | <span data-ttu-id="aac80-126">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="aac80-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="aac80-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="aac80-127">markImportance</span></span> | <span data-ttu-id="aac80-128">importance</span><span class="sxs-lookup"><span data-stu-id="aac80-128">importance</span></span> | <span data-ttu-id="aac80-129">Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="aac80-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="aac80-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="aac80-130">moveToFolder</span></span> |  <span data-ttu-id="aac80-131">String</span><span class="sxs-lookup"><span data-stu-id="aac80-131">String</span></span>| <span data-ttu-id="aac80-132">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="aac80-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="aac80-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="aac80-133">permanentDelete</span></span> | <span data-ttu-id="aac80-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="aac80-134">Boolean</span></span> | <span data-ttu-id="aac80-135">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="aac80-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="aac80-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="aac80-136">redirectTo</span></span> | <span data-ttu-id="aac80-137">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="aac80-137">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="aac80-138">Адреса электронной почты, к которым необходимо перенаправить сообщение.</span><span class="sxs-lookup"><span data-stu-id="aac80-138">The email addresses to which a message should be redirected.</span></span> |
| <span data-ttu-id="aac80-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="aac80-139">stopProcessingRules</span></span> | <span data-ttu-id="aac80-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="aac80-140">Boolean</span></span> | <span data-ttu-id="aac80-141">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="aac80-141">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aac80-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aac80-142">JSON representation</span></span>
<span data-ttu-id="aac80-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aac80-143">Here is a JSON representation of the resource.</span></span>

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