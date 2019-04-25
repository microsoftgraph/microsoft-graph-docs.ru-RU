---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 33f1167d7317f941ebfa79b372e9cf575c14989b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548504"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="2ffdc-103">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="2ffdc-103">messageRuleActions resource type</span></span>


<span data-ttu-id="2ffdc-104">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="2ffdc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ffdc-105">Properties</span></span>
| <span data-ttu-id="2ffdc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ffdc-106">Property</span></span>     | <span data-ttu-id="2ffdc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2ffdc-107">Type</span></span>   |<span data-ttu-id="2ffdc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2ffdc-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2ffdc-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="2ffdc-109">assignCategories</span></span> | <span data-ttu-id="2ffdc-110">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2ffdc-110">String collection</span></span> | <span data-ttu-id="2ffdc-111">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="2ffdc-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="2ffdc-112">copyToFolder</span></span> | <span data-ttu-id="2ffdc-113">String</span><span class="sxs-lookup"><span data-stu-id="2ffdc-113">String</span></span> | <span data-ttu-id="2ffdc-114">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="2ffdc-115">delete</span><span class="sxs-lookup"><span data-stu-id="2ffdc-115">delete</span></span> | <span data-ttu-id="2ffdc-116">Логический</span><span class="sxs-lookup"><span data-stu-id="2ffdc-116">Boolean</span></span> | <span data-ttu-id="2ffdc-117">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="2ffdc-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="2ffdc-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="2ffdc-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="2ffdc-119">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="2ffdc-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="2ffdc-120">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="2ffdc-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="2ffdc-121">forwardTo</span></span> | <span data-ttu-id="2ffdc-122">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="2ffdc-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="2ffdc-123">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="2ffdc-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="2ffdc-124">markAsRead</span></span> | <span data-ttu-id="2ffdc-125">Логический</span><span class="sxs-lookup"><span data-stu-id="2ffdc-125">Boolean</span></span> | <span data-ttu-id="2ffdc-126">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="2ffdc-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="2ffdc-127">markImportance</span></span> | <span data-ttu-id="2ffdc-128">importance</span><span class="sxs-lookup"><span data-stu-id="2ffdc-128">importance</span></span> | <span data-ttu-id="2ffdc-129">Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="2ffdc-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="2ffdc-130">moveToFolder</span></span> |  <span data-ttu-id="2ffdc-131">String</span><span class="sxs-lookup"><span data-stu-id="2ffdc-131">String</span></span>| <span data-ttu-id="2ffdc-132">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="2ffdc-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="2ffdc-133">permanentDelete</span></span> | <span data-ttu-id="2ffdc-134">Логический</span><span class="sxs-lookup"><span data-stu-id="2ffdc-134">Boolean</span></span> | <span data-ttu-id="2ffdc-135">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="2ffdc-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="2ffdc-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="2ffdc-136">redirectTo</span></span> | <span data-ttu-id="2ffdc-137">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="2ffdc-137">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="2ffdc-138">Адреса электронной почты, на которые необходимо перенаправить сообщение.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-138">The email addresses to which a message should be redirected.</span></span> |
| <span data-ttu-id="2ffdc-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="2ffdc-139">stopProcessingRules</span></span> | <span data-ttu-id="2ffdc-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ffdc-140">Boolean</span></span> | <span data-ttu-id="2ffdc-141">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-141">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2ffdc-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2ffdc-142">JSON representation</span></span>
<span data-ttu-id="2ffdc-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ffdc-143">Here is a JSON representation of the resource.</span></span>

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
