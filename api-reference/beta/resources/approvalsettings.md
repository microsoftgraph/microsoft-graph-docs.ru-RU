---
title: Сложный тип approvalSettings
description: Используется для свойства requestApprovalSettings политики назначения пакета доступа. Предоставляет дополнительные параметры для выбора, кто должен утвердить каждый запрос.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 85d47e09de1b4d8f687a8dff2abf6aff1af0f21f
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777731"
---
# <a name="approvalsettings-complex-type"></a><span data-ttu-id="eba6a-104">Сложный тип approvalSettings</span><span class="sxs-lookup"><span data-stu-id="eba6a-104">approvalSettings complex type</span></span>

<span data-ttu-id="eba6a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eba6a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eba6a-106">Используется для `requestApprovalSettings` свойства политики назначения пакета [доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eba6a-106">Used for the `requestApprovalSettings` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="eba6a-107">Предоставляет дополнительные параметры для выбора, кто должен утвердить каждый запрос.</span><span class="sxs-lookup"><span data-stu-id="eba6a-107">Provides additional settings to select who must approve each request.</span></span> 

## <a name="properties"></a><span data-ttu-id="eba6a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eba6a-108">Properties</span></span>

| <span data-ttu-id="eba6a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eba6a-109">Property</span></span>                     | <span data-ttu-id="eba6a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eba6a-110">Type</span></span>                      | <span data-ttu-id="eba6a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eba6a-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="eba6a-112">isApprovalRequired</span><span class="sxs-lookup"><span data-stu-id="eba6a-112">isApprovalRequired</span></span> | <span data-ttu-id="eba6a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="eba6a-113">Boolean</span></span> | <span data-ttu-id="eba6a-114">Если задается false, утверждение для запросов в этой политике не требуется.</span><span class="sxs-lookup"><span data-stu-id="eba6a-114">If false, then approval is not required for requests in this policy.</span></span> |
| <span data-ttu-id="eba6a-115">isApprovalRequiredForExtension</span><span class="sxs-lookup"><span data-stu-id="eba6a-115">isApprovalRequiredForExtension</span></span> | <span data-ttu-id="eba6a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="eba6a-116">Boolean</span></span>| <span data-ttu-id="eba6a-117">Если задается false, то для пользователя, у которого уже есть назначение для расширения назначения, утверждение не требуется.</span><span class="sxs-lookup"><span data-stu-id="eba6a-117">If false, then approval is not required for a user who already has an assignment to extend their assignment.</span></span> |
| <span data-ttu-id="eba6a-118">isRequestorJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="eba6a-118">isRequestorJustificationRequired</span></span> | <span data-ttu-id="eba6a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="eba6a-119">Boolean</span></span> | <span data-ttu-id="eba6a-120">Указывает, требуется ли запрашивать обоснование в своем запросе.</span><span class="sxs-lookup"><span data-stu-id="eba6a-120">Indicates whether the requestor is required to supply a justification in their request.</span></span> |
| <span data-ttu-id="eba6a-121">approvalMode</span><span class="sxs-lookup"><span data-stu-id="eba6a-121">approvalMode</span></span>| <span data-ttu-id="eba6a-122">String</span><span class="sxs-lookup"><span data-stu-id="eba6a-122">String</span></span> | <span data-ttu-id="eba6a-123">Один из `NoApproval` , `SingleStage` или `Serial` .</span><span class="sxs-lookup"><span data-stu-id="eba6a-123">One of `NoApproval`, `SingleStage` or `Serial`.</span></span> <span data-ttu-id="eba6a-124">Используется, `NoApproval` если `isApprovalRequired` заведомо неверно.</span><span class="sxs-lookup"><span data-stu-id="eba6a-124">The `NoApproval` is used when `isApprovalRequired` is false.</span></span> |
| <span data-ttu-id="eba6a-125">approvalStages</span><span class="sxs-lookup"><span data-stu-id="eba6a-125">approvalStages</span></span> | <span data-ttu-id="eba6a-126">[Коллекция approvalStage](approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="eba6a-126">[approvalStage](approvalstage.md) collection</span></span>| <span data-ttu-id="eba6a-127">Если требуется утверждение, один или два элемента этой коллекции определяют каждый из этапов утверждения.</span><span class="sxs-lookup"><span data-stu-id="eba6a-127">If approval is required, the one or two elements of this collection define each of the stages of approval.</span></span> <span data-ttu-id="eba6a-128">Пустой массив, если утверждение не требуется.</span><span class="sxs-lookup"><span data-stu-id="eba6a-128">An empty array if no approval is required.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="eba6a-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eba6a-129">JSON representation</span></span>

<span data-ttu-id="eba6a-130">Ниже приводится представление свойства параметров утверждения запроса в JSON.</span><span class="sxs-lookup"><span data-stu-id="eba6a-130">The following is a JSON representation of the request approval settings property.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings"
}-->

```json
{
    "isApprovalRequired": true,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": true,
    "approvalMode": "Serial",
    "approvalStages": [{"@odata.type": "microsoft.graph.approvalStage"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "approvalSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


