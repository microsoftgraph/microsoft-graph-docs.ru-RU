---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: aae9420f3d1b6e329a007eda3917ce7eaa8c4dda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971547"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="f7cb6-103">Тип ресурса messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="f7cb6-103">messageRuleActions resource type</span></span>

<span data-ttu-id="f7cb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7cb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7cb6-105">Представляет набор действий, доступных для правила.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-105">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="f7cb6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7cb6-106">Properties</span></span>
| <span data-ttu-id="f7cb6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7cb6-107">Property</span></span>     | <span data-ttu-id="f7cb6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f7cb6-108">Type</span></span>   |<span data-ttu-id="f7cb6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f7cb6-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7cb6-110">assignCategories</span><span class="sxs-lookup"><span data-stu-id="f7cb6-110">assignCategories</span></span> | <span data-ttu-id="f7cb6-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f7cb6-111">String collection</span></span> | <span data-ttu-id="f7cb6-112">Список категорий, которые необходимо назначить сообщению.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-112">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="f7cb6-113">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="f7cb6-113">copyToFolder</span></span> | <span data-ttu-id="f7cb6-114">String</span><span class="sxs-lookup"><span data-stu-id="f7cb6-114">String</span></span> | <span data-ttu-id="f7cb6-115">Идентификатор папки, в которую необходимо скопировать сообщение.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-115">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="f7cb6-116">delete</span><span class="sxs-lookup"><span data-stu-id="f7cb6-116">delete</span></span> | <span data-ttu-id="f7cb6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7cb6-117">Boolean</span></span> | <span data-ttu-id="f7cb6-118">Указывает, нужно ли перемещать сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="f7cb6-118">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="f7cb6-119">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="f7cb6-119">forwardAsAttachmentTo</span></span> | <span data-ttu-id="f7cb6-120">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f7cb6-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="f7cb6-121">Электронные адреса получателей, которым необходимо переслать сообщение как вложение.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-121">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="f7cb6-122">forwardTo</span><span class="sxs-lookup"><span data-stu-id="f7cb6-122">forwardTo</span></span> | <span data-ttu-id="f7cb6-123">Коллекция [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="f7cb6-123">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="f7cb6-124">Электронные адреса получателей, которым необходимо переслать сообщение.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-124">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="f7cb6-125">markAsRead</span><span class="sxs-lookup"><span data-stu-id="f7cb6-125">markAsRead</span></span> | <span data-ttu-id="f7cb6-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7cb6-126">Boolean</span></span> | <span data-ttu-id="f7cb6-127">Указывает, необходимо ли отмечать сообщение как прочтенное.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-127">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="f7cb6-128">markImportance</span><span class="sxs-lookup"><span data-stu-id="f7cb6-128">markImportance</span></span> | <span data-ttu-id="f7cb6-129">String</span><span class="sxs-lookup"><span data-stu-id="f7cb6-129">String</span></span> | <span data-ttu-id="f7cb6-130">Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-130">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="f7cb6-131">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="f7cb6-131">moveToFolder</span></span> |  <span data-ttu-id="f7cb6-132">String</span><span class="sxs-lookup"><span data-stu-id="f7cb6-132">String</span></span>| <span data-ttu-id="f7cb6-133">Идентификатор папки, в которую сообщение будет перемещено.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-133">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="f7cb6-134">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="f7cb6-134">permanentDelete</span></span> | <span data-ttu-id="f7cb6-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7cb6-135">Boolean</span></span> | <span data-ttu-id="f7cb6-136">Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="f7cb6-136">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="f7cb6-137">redirectTo</span><span class="sxs-lookup"><span data-stu-id="f7cb6-137">redirectTo</span></span> | [<span data-ttu-id="f7cb6-138">recipient</span><span class="sxs-lookup"><span data-stu-id="f7cb6-138">recipient</span></span>](recipient.md) | <span data-ttu-id="f7cb6-139">Электронный адрес, на который должно быть перенаправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-139">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="f7cb6-140">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="f7cb6-140">stopProcessingRules</span></span> | <span data-ttu-id="f7cb6-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7cb6-141">Boolean</span></span> | <span data-ttu-id="f7cb6-142">Указывает, должны ли обрабатываться последующие правила.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-142">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f7cb6-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7cb6-143">JSON representation</span></span>
<span data-ttu-id="f7cb6-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7cb6-144">Here is a JSON representation of the resource.</span></span>

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


