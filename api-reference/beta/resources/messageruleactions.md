---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
author: angelgolfer-ms
ms.openlocfilehash: 515d31ff8c11b95a3aa0042449d22df883e0eecf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314996"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="d793f-103">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="d793f-103">messageRuleActions resource type</span></span>

> <span data-ttu-id="d793f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d793f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d793f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d793f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d793f-106">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="d793f-106">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="d793f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d793f-107">Properties</span></span>
| <span data-ttu-id="d793f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d793f-108">Property</span></span>     | <span data-ttu-id="d793f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d793f-109">Type</span></span>   |<span data-ttu-id="d793f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d793f-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d793f-111">assignCategories</span><span class="sxs-lookup"><span data-stu-id="d793f-111">assignCategories</span></span> | <span data-ttu-id="d793f-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d793f-112">String collection</span></span> | <span data-ttu-id="d793f-113">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="d793f-113">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="d793f-114">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="d793f-114">copyToFolder</span></span> | <span data-ttu-id="d793f-115">String</span><span class="sxs-lookup"><span data-stu-id="d793f-115">String</span></span> | <span data-ttu-id="d793f-116">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="d793f-116">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="d793f-117">delete</span><span class="sxs-lookup"><span data-stu-id="d793f-117">delete</span></span> | <span data-ttu-id="d793f-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d793f-118">Boolean</span></span> | <span data-ttu-id="d793f-119">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="d793f-119">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="d793f-120">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="d793f-120">forwardAsAttachmentTo</span></span> | <span data-ttu-id="d793f-121">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="d793f-121">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="d793f-122">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="d793f-122">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="d793f-123">forwardTo</span><span class="sxs-lookup"><span data-stu-id="d793f-123">forwardTo</span></span> | <span data-ttu-id="d793f-124">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="d793f-124">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="d793f-125">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="d793f-125">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="d793f-126">markAsRead</span><span class="sxs-lookup"><span data-stu-id="d793f-126">markAsRead</span></span> | <span data-ttu-id="d793f-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="d793f-127">Boolean</span></span> | <span data-ttu-id="d793f-128">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="d793f-128">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="d793f-129">markImportance</span><span class="sxs-lookup"><span data-stu-id="d793f-129">markImportance</span></span> | <span data-ttu-id="d793f-130">String</span><span class="sxs-lookup"><span data-stu-id="d793f-130">String</span></span> | <span data-ttu-id="d793f-131">Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d793f-131">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="d793f-132">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="d793f-132">moveToFolder</span></span> |  <span data-ttu-id="d793f-133">String</span><span class="sxs-lookup"><span data-stu-id="d793f-133">String</span></span>| <span data-ttu-id="d793f-134">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="d793f-134">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="d793f-135">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="d793f-135">permanentDelete</span></span> | <span data-ttu-id="d793f-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="d793f-136">Boolean</span></span> | <span data-ttu-id="d793f-137">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="d793f-137">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="d793f-138">redirectTo</span><span class="sxs-lookup"><span data-stu-id="d793f-138">redirectTo</span></span> | [<span data-ttu-id="d793f-139">recipient</span><span class="sxs-lookup"><span data-stu-id="d793f-139">recipient</span></span>](recipient.md) | <span data-ttu-id="d793f-140">Электронный адрес, на который должно быть перенаправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="d793f-140">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="d793f-141">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="d793f-141">stopProcessingRules</span></span> | <span data-ttu-id="d793f-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="d793f-142">Boolean</span></span> | <span data-ttu-id="d793f-143">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="d793f-143">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d793f-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d793f-144">JSON representation</span></span>
<span data-ttu-id="d793f-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d793f-145">Here is a JSON representation of the resource.</span></span>

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