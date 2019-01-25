---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a786a225bb9d439d60a29d2395b2d438975fc16c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523234"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="f0c09-103">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="f0c09-103">messageRuleActions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0c09-104">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="f0c09-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="f0c09-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0c09-105">Properties</span></span>
| <span data-ttu-id="f0c09-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0c09-106">Property</span></span>     | <span data-ttu-id="f0c09-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f0c09-107">Type</span></span>   |<span data-ttu-id="f0c09-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f0c09-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f0c09-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="f0c09-109">assignCategories</span></span> | <span data-ttu-id="f0c09-110">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f0c09-110">String collection</span></span> | <span data-ttu-id="f0c09-111">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="f0c09-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="f0c09-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="f0c09-112">copyToFolder</span></span> | <span data-ttu-id="f0c09-113">String</span><span class="sxs-lookup"><span data-stu-id="f0c09-113">String</span></span> | <span data-ttu-id="f0c09-114">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="f0c09-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="f0c09-115">delete</span><span class="sxs-lookup"><span data-stu-id="f0c09-115">delete</span></span> | <span data-ttu-id="f0c09-116">Логическое</span><span class="sxs-lookup"><span data-stu-id="f0c09-116">Boolean</span></span> | <span data-ttu-id="f0c09-117">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="f0c09-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="f0c09-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="f0c09-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="f0c09-119">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f0c09-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="f0c09-120">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="f0c09-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="f0c09-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="f0c09-121">forwardTo</span></span> | <span data-ttu-id="f0c09-122">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f0c09-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="f0c09-123">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="f0c09-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="f0c09-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="f0c09-124">markAsRead</span></span> | <span data-ttu-id="f0c09-125">Логическое</span><span class="sxs-lookup"><span data-stu-id="f0c09-125">Boolean</span></span> | <span data-ttu-id="f0c09-126">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="f0c09-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="f0c09-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="f0c09-127">markImportance</span></span> | <span data-ttu-id="f0c09-128">String</span><span class="sxs-lookup"><span data-stu-id="f0c09-128">String</span></span> | <span data-ttu-id="f0c09-129">Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f0c09-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="f0c09-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="f0c09-130">moveToFolder</span></span> |  <span data-ttu-id="f0c09-131">String</span><span class="sxs-lookup"><span data-stu-id="f0c09-131">String</span></span>| <span data-ttu-id="f0c09-132">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="f0c09-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="f0c09-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="f0c09-133">permanentDelete</span></span> | <span data-ttu-id="f0c09-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0c09-134">Boolean</span></span> | <span data-ttu-id="f0c09-135">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="f0c09-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="f0c09-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="f0c09-136">redirectTo</span></span> | [<span data-ttu-id="f0c09-137">recipient</span><span class="sxs-lookup"><span data-stu-id="f0c09-137">recipient</span></span>](recipient.md) | <span data-ttu-id="f0c09-138">Электронный адрес, на который должно быть перенаправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="f0c09-138">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="f0c09-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="f0c09-139">stopProcessingRules</span></span> | <span data-ttu-id="f0c09-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0c09-140">Boolean</span></span> | <span data-ttu-id="f0c09-141">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="f0c09-141">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f0c09-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0c09-142">JSON representation</span></span>
<span data-ttu-id="f0c09-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0c09-143">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/messageruleactions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
