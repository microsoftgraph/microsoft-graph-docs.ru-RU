---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 58cae7f777d0ac9ee03b102b22325e63acf55358
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938890"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="f1c5e-103">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="f1c5e-103">messageRuleActions resource type</span></span>

> <span data-ttu-id="f1c5e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1c5e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f1c5e-106">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-106">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="f1c5e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1c5e-107">Properties</span></span>
| <span data-ttu-id="f1c5e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1c5e-108">Property</span></span>     | <span data-ttu-id="f1c5e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f1c5e-109">Type</span></span>   |<span data-ttu-id="f1c5e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f1c5e-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1c5e-111">assignCategories</span><span class="sxs-lookup"><span data-stu-id="f1c5e-111">assignCategories</span></span> | <span data-ttu-id="f1c5e-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f1c5e-112">String collection</span></span> | <span data-ttu-id="f1c5e-113">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-113">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="f1c5e-114">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="f1c5e-114">copyToFolder</span></span> | <span data-ttu-id="f1c5e-115">String</span><span class="sxs-lookup"><span data-stu-id="f1c5e-115">String</span></span> | <span data-ttu-id="f1c5e-116">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-116">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="f1c5e-117">delete</span><span class="sxs-lookup"><span data-stu-id="f1c5e-117">delete</span></span> | <span data-ttu-id="f1c5e-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1c5e-118">Boolean</span></span> | <span data-ttu-id="f1c5e-119">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="f1c5e-119">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="f1c5e-120">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="f1c5e-120">forwardAsAttachmentTo</span></span> | <span data-ttu-id="f1c5e-121">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f1c5e-121">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="f1c5e-122">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-122">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="f1c5e-123">forwardTo</span><span class="sxs-lookup"><span data-stu-id="f1c5e-123">forwardTo</span></span> | <span data-ttu-id="f1c5e-124">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f1c5e-124">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="f1c5e-125">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-125">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="f1c5e-126">markAsRead</span><span class="sxs-lookup"><span data-stu-id="f1c5e-126">markAsRead</span></span> | <span data-ttu-id="f1c5e-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1c5e-127">Boolean</span></span> | <span data-ttu-id="f1c5e-128">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-128">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="f1c5e-129">markImportance</span><span class="sxs-lookup"><span data-stu-id="f1c5e-129">markImportance</span></span> | <span data-ttu-id="f1c5e-130">String</span><span class="sxs-lookup"><span data-stu-id="f1c5e-130">String</span></span> | <span data-ttu-id="f1c5e-131">Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-131">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="f1c5e-132">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="f1c5e-132">moveToFolder</span></span> |  <span data-ttu-id="f1c5e-133">String</span><span class="sxs-lookup"><span data-stu-id="f1c5e-133">String</span></span>| <span data-ttu-id="f1c5e-134">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-134">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="f1c5e-135">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="f1c5e-135">permanentDelete</span></span> | <span data-ttu-id="f1c5e-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1c5e-136">Boolean</span></span> | <span data-ttu-id="f1c5e-137">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="f1c5e-137">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="f1c5e-138">redirectTo</span><span class="sxs-lookup"><span data-stu-id="f1c5e-138">redirectTo</span></span> | [<span data-ttu-id="f1c5e-139">recipient</span><span class="sxs-lookup"><span data-stu-id="f1c5e-139">recipient</span></span>](recipient.md) | <span data-ttu-id="f1c5e-140">Электронный адрес, на который должно быть перенаправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-140">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="f1c5e-141">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="f1c5e-141">stopProcessingRules</span></span> | <span data-ttu-id="f1c5e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1c5e-142">Boolean</span></span> | <span data-ttu-id="f1c5e-143">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-143">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f1c5e-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1c5e-144">JSON representation</span></span>
<span data-ttu-id="f1c5e-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1c5e-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
