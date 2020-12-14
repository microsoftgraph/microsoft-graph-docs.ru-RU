---
title: Тип ресурса aadUserConversationMemberResult
description: Ресурс для моделирования ответов массовых операций в aadUserConversationMember.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8251107c325bdbe2c5ff9e6df95a2d08277dde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663911"
---
# <a name="aaduserconversationmemberresult-resource-type"></a><span data-ttu-id="2a9ef-103">Тип ресурса aadUserConversationMemberResult</span><span class="sxs-lookup"><span data-stu-id="2a9ef-103">aadUserConversationMemberResult resource type</span></span>

<span data-ttu-id="2a9ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a9ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a9ef-105">Представляет отдельный ответ для каждого члена, указанного в массовой операции, состоящей из [aadUserConversationMember(s)](aadUserConversationMember.md) в запросе.</span><span class="sxs-lookup"><span data-stu-id="2a9ef-105">Represents the individual response for each member specified in a bulk operation comprising of [aadUserConversationMember(s)](aadUserConversationMember.md) in the request.</span></span>
<span data-ttu-id="2a9ef-106">Этот ресурс является производным от [ресурса actionResultPart.](actionresultpart.md)</span><span class="sxs-lookup"><span data-stu-id="2a9ef-106">This resource is the derivative of the [actionResultPart](actionresultpart.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="2a9ef-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a9ef-107">Properties</span></span>

| <span data-ttu-id="2a9ef-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a9ef-108">Property</span></span> | <span data-ttu-id="2a9ef-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2a9ef-109">Type</span></span>   | <span data-ttu-id="2a9ef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2a9ef-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2a9ef-111">userId</span><span class="sxs-lookup"><span data-stu-id="2a9ef-111">userId</span></span>|`String`|<span data-ttu-id="2a9ef-112">ИД объекта пользователя Azure AD, добавляемого в рамках массовой операции.</span><span class="sxs-lookup"><span data-stu-id="2a9ef-112">The user object ID of the Azure AD user that was being added as part of the bulk operation.</span></span>|
|<span data-ttu-id="2a9ef-113">error</span><span class="sxs-lookup"><span data-stu-id="2a9ef-113">error</span></span>|[<span data-ttu-id="2a9ef-114">publicError</span><span class="sxs-lookup"><span data-stu-id="2a9ef-114">publicError</span></span>](publicerror.md) |<span data-ttu-id="2a9ef-115">Ошибка, которая произошла (если она возникла) в ходе массовой операции.</span><span class="sxs-lookup"><span data-stu-id="2a9ef-115">The error that occurred, if any, during the course of the bulk operation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a9ef-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a9ef-116">JSON representation</span></span>

<span data-ttu-id="2a9ef-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a9ef-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.aadUserConversationMemberResult"
}-->

```json
{
    "userId": "string",
    "error": "microsoft.graph.publicError"
}
```

## <a name="see-also"></a><span data-ttu-id="2a9ef-118">См. также</span><span class="sxs-lookup"><span data-stu-id="2a9ef-118">See also</span></span>

- [<span data-ttu-id="2a9ef-119">Массовое добавление участников в команду</span><span class="sxs-lookup"><span data-stu-id="2a9ef-119">Add members in bulk to team</span></span>](../api/conversationmembers-add.md)

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "actionResultPart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


