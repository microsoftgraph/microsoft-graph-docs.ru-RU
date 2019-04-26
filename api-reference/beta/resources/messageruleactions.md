---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5582bbe2d6dcf054b276bd583a8544752d6d5eb4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342235"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="e7903-103">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="e7903-103">messageRuleActions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7903-104">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="e7903-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="e7903-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7903-105">Properties</span></span>
| <span data-ttu-id="e7903-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7903-106">Property</span></span>     | <span data-ttu-id="e7903-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e7903-107">Type</span></span>   |<span data-ttu-id="e7903-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e7903-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e7903-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="e7903-109">assignCategories</span></span> | <span data-ttu-id="e7903-110">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e7903-110">String collection</span></span> | <span data-ttu-id="e7903-111">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="e7903-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="e7903-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="e7903-112">copyToFolder</span></span> | <span data-ttu-id="e7903-113">String</span><span class="sxs-lookup"><span data-stu-id="e7903-113">String</span></span> | <span data-ttu-id="e7903-114">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="e7903-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="e7903-115">delete</span><span class="sxs-lookup"><span data-stu-id="e7903-115">delete</span></span> | <span data-ttu-id="e7903-116">Логический</span><span class="sxs-lookup"><span data-stu-id="e7903-116">Boolean</span></span> | <span data-ttu-id="e7903-117">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="e7903-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="e7903-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="e7903-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="e7903-119">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="e7903-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="e7903-120">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="e7903-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="e7903-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="e7903-121">forwardTo</span></span> | <span data-ttu-id="e7903-122">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="e7903-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="e7903-123">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="e7903-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="e7903-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="e7903-124">markAsRead</span></span> | <span data-ttu-id="e7903-125">Логический</span><span class="sxs-lookup"><span data-stu-id="e7903-125">Boolean</span></span> | <span data-ttu-id="e7903-126">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="e7903-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="e7903-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="e7903-127">markImportance</span></span> | <span data-ttu-id="e7903-128">String</span><span class="sxs-lookup"><span data-stu-id="e7903-128">String</span></span> | <span data-ttu-id="e7903-129">Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e7903-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="e7903-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="e7903-130">moveToFolder</span></span> |  <span data-ttu-id="e7903-131">String</span><span class="sxs-lookup"><span data-stu-id="e7903-131">String</span></span>| <span data-ttu-id="e7903-132">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="e7903-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="e7903-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="e7903-133">permanentDelete</span></span> | <span data-ttu-id="e7903-134">Логический</span><span class="sxs-lookup"><span data-stu-id="e7903-134">Boolean</span></span> | <span data-ttu-id="e7903-135">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="e7903-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="e7903-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="e7903-136">redirectTo</span></span> | [<span data-ttu-id="e7903-137">recipient</span><span class="sxs-lookup"><span data-stu-id="e7903-137">recipient</span></span>](recipient.md) | <span data-ttu-id="e7903-138">Электронный адрес, на который должно быть перенаправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="e7903-138">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="e7903-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="e7903-139">stopProcessingRules</span></span> | <span data-ttu-id="e7903-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7903-140">Boolean</span></span> | <span data-ttu-id="e7903-141">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="e7903-141">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e7903-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7903-142">JSON representation</span></span>
<span data-ttu-id="e7903-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7903-143">Here is a JSON representation of the resource.</span></span>

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
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
