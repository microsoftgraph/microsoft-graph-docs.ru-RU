---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 406632618c4200fc217b993a7df8631b13db3cc8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468348"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="9d3ff-103">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="9d3ff-103">messageRuleActions resource type</span></span>

<span data-ttu-id="9d3ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d3ff-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="9d3ff-105">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-105">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="9d3ff-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d3ff-106">Properties</span></span>
| <span data-ttu-id="9d3ff-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d3ff-107">Property</span></span>     | <span data-ttu-id="9d3ff-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9d3ff-108">Type</span></span>   |<span data-ttu-id="9d3ff-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9d3ff-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9d3ff-110">assignCategories</span><span class="sxs-lookup"><span data-stu-id="9d3ff-110">assignCategories</span></span> | <span data-ttu-id="9d3ff-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9d3ff-111">String collection</span></span> | <span data-ttu-id="9d3ff-112">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-112">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="9d3ff-113">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="9d3ff-113">copyToFolder</span></span> | <span data-ttu-id="9d3ff-114">String</span><span class="sxs-lookup"><span data-stu-id="9d3ff-114">String</span></span> | <span data-ttu-id="9d3ff-115">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-115">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="9d3ff-116">delete</span><span class="sxs-lookup"><span data-stu-id="9d3ff-116">delete</span></span> | <span data-ttu-id="9d3ff-117">Логический</span><span class="sxs-lookup"><span data-stu-id="9d3ff-117">Boolean</span></span> | <span data-ttu-id="9d3ff-118">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="9d3ff-118">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="9d3ff-119">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="9d3ff-119">forwardAsAttachmentTo</span></span> | <span data-ttu-id="9d3ff-120">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="9d3ff-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="9d3ff-121">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-121">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="9d3ff-122">forwardTo</span><span class="sxs-lookup"><span data-stu-id="9d3ff-122">forwardTo</span></span> | <span data-ttu-id="9d3ff-123">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="9d3ff-123">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="9d3ff-124">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-124">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="9d3ff-125">markAsRead</span><span class="sxs-lookup"><span data-stu-id="9d3ff-125">markAsRead</span></span> | <span data-ttu-id="9d3ff-126">Логический</span><span class="sxs-lookup"><span data-stu-id="9d3ff-126">Boolean</span></span> | <span data-ttu-id="9d3ff-127">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-127">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="9d3ff-128">markImportance</span><span class="sxs-lookup"><span data-stu-id="9d3ff-128">markImportance</span></span> | <span data-ttu-id="9d3ff-129">importance</span><span class="sxs-lookup"><span data-stu-id="9d3ff-129">importance</span></span> | <span data-ttu-id="9d3ff-130">Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-130">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="9d3ff-131">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="9d3ff-131">moveToFolder</span></span> |  <span data-ttu-id="9d3ff-132">String</span><span class="sxs-lookup"><span data-stu-id="9d3ff-132">String</span></span>| <span data-ttu-id="9d3ff-133">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-133">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="9d3ff-134">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="9d3ff-134">permanentDelete</span></span> | <span data-ttu-id="9d3ff-135">Логический</span><span class="sxs-lookup"><span data-stu-id="9d3ff-135">Boolean</span></span> | <span data-ttu-id="9d3ff-136">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="9d3ff-136">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="9d3ff-137">redirectTo</span><span class="sxs-lookup"><span data-stu-id="9d3ff-137">redirectTo</span></span> | <span data-ttu-id="9d3ff-138">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="9d3ff-138">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="9d3ff-139">Адреса электронной почты, на которые необходимо перенаправить сообщение.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-139">The email addresses to which a message should be redirected.</span></span> |
| <span data-ttu-id="9d3ff-140">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="9d3ff-140">stopProcessingRules</span></span> | <span data-ttu-id="9d3ff-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d3ff-141">Boolean</span></span> | <span data-ttu-id="9d3ff-142">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-142">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9d3ff-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d3ff-143">JSON representation</span></span>
<span data-ttu-id="9d3ff-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d3ff-144">Here is a JSON representation of the resource.</span></span>

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
