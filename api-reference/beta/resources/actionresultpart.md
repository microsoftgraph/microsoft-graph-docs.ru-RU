---
title: Тип ресурса actionResultType
description: Абстрактный тип для моделирования ответов массовых операций.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a092fa4a322d0d207550947559cb5dfff4ad4625
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664004"
---
# <a name="actionresultpart-resource-type"></a><span data-ttu-id="d1cd5-103">Тип ресурса actionResultPart</span><span class="sxs-lookup"><span data-stu-id="d1cd5-103">actionResultPart resource type</span></span>

<span data-ttu-id="d1cd5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1cd5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1cd5-105">Абстрактный тип, который служит основой для моделирования ответов массовых операций.</span><span class="sxs-lookup"><span data-stu-id="d1cd5-105">An abstract type that serves as a base for modeling responses of bulk operations.</span></span> <span data-ttu-id="d1cd5-106">Свойство **ошибки** заполняется выборочно в зависимости от того, представляет ли ответ ошибку.</span><span class="sxs-lookup"><span data-stu-id="d1cd5-106">The **error** property is selectively populated based on whether the response represents an error.</span></span>

## <a name="properties"></a><span data-ttu-id="d1cd5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1cd5-107">Properties</span></span>

| <span data-ttu-id="d1cd5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1cd5-108">Property</span></span> | <span data-ttu-id="d1cd5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d1cd5-109">Type</span></span>   | <span data-ttu-id="d1cd5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d1cd5-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d1cd5-111">error</span><span class="sxs-lookup"><span data-stu-id="d1cd5-111">error</span></span>|[<span data-ttu-id="d1cd5-112">publicError</span><span class="sxs-lookup"><span data-stu-id="d1cd5-112">publicError</span></span>](publicerror.md) |<span data-ttu-id="d1cd5-113">Ошибка, которая произошла (если она возникла) в ходе массовой операции.</span><span class="sxs-lookup"><span data-stu-id="d1cd5-113">The error that occurred, if any, during the course of the bulk operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1cd5-114">Связи</span><span class="sxs-lookup"><span data-stu-id="d1cd5-114">Relationships</span></span>
<span data-ttu-id="d1cd5-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d1cd5-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1cd5-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d1cd5-116">JSON representation</span></span>
<span data-ttu-id="d1cd5-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1cd5-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.actionResultPart"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.actionResultPart",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  }
}
```
## <a name="see-also"></a><span data-ttu-id="d1cd5-118">См. также</span><span class="sxs-lookup"><span data-stu-id="d1cd5-118">See also</span></span>

- [<span data-ttu-id="d1cd5-119">aadUserConversationMemberResult</span><span class="sxs-lookup"><span data-stu-id="d1cd5-119">aadUserConversationMemberResult</span></span>](aadUserConversationMemberResult.md)
- [<span data-ttu-id="d1cd5-120">Массовое добавление участников в команду</span><span class="sxs-lookup"><span data-stu-id="d1cd5-120">Add members in bulk to team</span></span>](../api/conversationmembers-add.md)

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


