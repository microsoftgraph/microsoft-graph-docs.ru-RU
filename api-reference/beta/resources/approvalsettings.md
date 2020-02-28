---
title: сложный тип Аппровалсеттингс
description: Используется для свойства Рекуестаппровалсеттингс политики назначения пакетов Access. Предоставляет дополнительные параметры для выбора лиц, которые должны утверждать каждый запрос.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e248e47cf94e2c26e80b505cbaead450e03561d4
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331442"
---
# <a name="approvalsettings-complex-type"></a><span data-ttu-id="0e59f-104">сложный тип Аппровалсеттингс</span><span class="sxs-lookup"><span data-stu-id="0e59f-104">approvalSettings complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e59f-105">Используется для `requestApprovalSettings` свойства [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0e59f-105">Used for the `requestApprovalSettings` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="0e59f-106">Предоставляет дополнительные параметры для выбора лиц, которые должны утверждать каждый запрос.</span><span class="sxs-lookup"><span data-stu-id="0e59f-106">Provides additional settings to select who must approve each request.</span></span> 

## <a name="properties"></a><span data-ttu-id="0e59f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e59f-107">Properties</span></span>

| <span data-ttu-id="0e59f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e59f-108">Property</span></span>                     | <span data-ttu-id="0e59f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0e59f-109">Type</span></span>                      | <span data-ttu-id="0e59f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0e59f-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="0e59f-111">исаппровалрекуиред</span><span class="sxs-lookup"><span data-stu-id="0e59f-111">isApprovalRequired</span></span> | <span data-ttu-id="0e59f-112">Логический</span><span class="sxs-lookup"><span data-stu-id="0e59f-112">Boolean</span></span> | <span data-ttu-id="0e59f-113">Если задано значение false, то для запросов в этой политике утверждение не требуется.</span><span class="sxs-lookup"><span data-stu-id="0e59f-113">If false, then approval is not required for requests in this policy.</span></span> |
| <span data-ttu-id="0e59f-114">исаппровалрекуиредфорекстенсион</span><span class="sxs-lookup"><span data-stu-id="0e59f-114">isApprovalRequiredForExtension</span></span> | <span data-ttu-id="0e59f-115">Логический</span><span class="sxs-lookup"><span data-stu-id="0e59f-115">Boolean</span></span>| <span data-ttu-id="0e59f-116">Если задано значение false, то утверждение не требуется для пользователя, который уже имеет назначение для расширения назначения.</span><span class="sxs-lookup"><span data-stu-id="0e59f-116">If false, then approval is not required for a user who already has an assignment to extend their assignment.</span></span> |
| <span data-ttu-id="0e59f-117">исрекуесторжустификатионрекуиред</span><span class="sxs-lookup"><span data-stu-id="0e59f-117">isRequestorJustificationRequired</span></span> | <span data-ttu-id="0e59f-118">Логический</span><span class="sxs-lookup"><span data-stu-id="0e59f-118">Boolean</span></span> | <span data-ttu-id="0e59f-119">Указывает, требуется ли запрашивающему для предоставления обоснования в запросе.</span><span class="sxs-lookup"><span data-stu-id="0e59f-119">Indicates whether the requestor is required to supply a justification in their request.</span></span> |
| <span data-ttu-id="0e59f-120">аппровалмоде</span><span class="sxs-lookup"><span data-stu-id="0e59f-120">approvalMode</span></span>| <span data-ttu-id="0e59f-121">String</span><span class="sxs-lookup"><span data-stu-id="0e59f-121">String</span></span> | <span data-ttu-id="0e59f-122">Один из `NoApproval`, `SingleStage` или `Serial`.</span><span class="sxs-lookup"><span data-stu-id="0e59f-122">One of `NoApproval`, `SingleStage` or `Serial`.</span></span> <span data-ttu-id="0e59f-123">`NoApproval` Используется при `isApprovalRequired` значении false.</span><span class="sxs-lookup"><span data-stu-id="0e59f-123">The `NoApproval` is used when `isApprovalRequired` is false.</span></span> |
| <span data-ttu-id="0e59f-124">аппровалстажес</span><span class="sxs-lookup"><span data-stu-id="0e59f-124">approvalStages</span></span> | <span data-ttu-id="0e59f-125">Коллекция [аппровалстаже](approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="0e59f-125">[approvalStage](approvalstage.md) collection</span></span>| <span data-ttu-id="0e59f-126">Если необходимо утверждение, то один или два элемента этой коллекции определяют каждый из стадий утверждения.</span><span class="sxs-lookup"><span data-stu-id="0e59f-126">If approval is required, the one or two elements of this collection define each of the stages of approval.</span></span> <span data-ttu-id="0e59f-127">Пустой массив, если утверждение не нужно.</span><span class="sxs-lookup"><span data-stu-id="0e59f-127">An empty array if no approval is required.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="0e59f-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e59f-128">JSON representation</span></span>

<span data-ttu-id="0e59f-129">Ниже приведено представление свойства параметров утверждения запроса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e59f-129">The following is a JSON representation of the request approval settings property.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings",
  "baseType": ""
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
