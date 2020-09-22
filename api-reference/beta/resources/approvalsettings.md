---
title: сложный тип Аппровалсеттингс
description: Используется для свойства Рекуестаппровалсеттингс политики назначения пакетов Access. Предоставляет дополнительные параметры для выбора лиц, которые должны утверждать каждый запрос.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a3c674b6bb21ddebfbb63f60d1ec2d2b62077f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050152"
---
# <a name="approvalsettings-complex-type"></a><span data-ttu-id="54430-104">сложный тип Аппровалсеттингс</span><span class="sxs-lookup"><span data-stu-id="54430-104">approvalSettings complex type</span></span>

<span data-ttu-id="54430-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54430-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54430-106">Используется для `requestApprovalSettings` свойства [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="54430-106">Used for the `requestApprovalSettings` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="54430-107">Предоставляет дополнительные параметры для выбора лиц, которые должны утверждать каждый запрос.</span><span class="sxs-lookup"><span data-stu-id="54430-107">Provides additional settings to select who must approve each request.</span></span> 

## <a name="properties"></a><span data-ttu-id="54430-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="54430-108">Properties</span></span>

| <span data-ttu-id="54430-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="54430-109">Property</span></span>                     | <span data-ttu-id="54430-110">Тип</span><span class="sxs-lookup"><span data-stu-id="54430-110">Type</span></span>                      | <span data-ttu-id="54430-111">Описание</span><span class="sxs-lookup"><span data-stu-id="54430-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="54430-112">исаппровалрекуиред</span><span class="sxs-lookup"><span data-stu-id="54430-112">isApprovalRequired</span></span> | <span data-ttu-id="54430-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="54430-113">Boolean</span></span> | <span data-ttu-id="54430-114">Если задано значение false, то для запросов в этой политике утверждение не требуется.</span><span class="sxs-lookup"><span data-stu-id="54430-114">If false, then approval is not required for requests in this policy.</span></span> |
| <span data-ttu-id="54430-115">исаппровалрекуиредфорекстенсион</span><span class="sxs-lookup"><span data-stu-id="54430-115">isApprovalRequiredForExtension</span></span> | <span data-ttu-id="54430-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="54430-116">Boolean</span></span>| <span data-ttu-id="54430-117">Если задано значение false, то утверждение не требуется для пользователя, который уже имеет назначение для расширения назначения.</span><span class="sxs-lookup"><span data-stu-id="54430-117">If false, then approval is not required for a user who already has an assignment to extend their assignment.</span></span> |
| <span data-ttu-id="54430-118">исрекуесторжустификатионрекуиред</span><span class="sxs-lookup"><span data-stu-id="54430-118">isRequestorJustificationRequired</span></span> | <span data-ttu-id="54430-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="54430-119">Boolean</span></span> | <span data-ttu-id="54430-120">Указывает, требуется ли запрашивающему для предоставления обоснования в запросе.</span><span class="sxs-lookup"><span data-stu-id="54430-120">Indicates whether the requestor is required to supply a justification in their request.</span></span> |
| <span data-ttu-id="54430-121">аппровалмоде</span><span class="sxs-lookup"><span data-stu-id="54430-121">approvalMode</span></span>| <span data-ttu-id="54430-122">Строка</span><span class="sxs-lookup"><span data-stu-id="54430-122">String</span></span> | <span data-ttu-id="54430-123">Один из `NoApproval` , `SingleStage` или `Serial` .</span><span class="sxs-lookup"><span data-stu-id="54430-123">One of `NoApproval`, `SingleStage` or `Serial`.</span></span> <span data-ttu-id="54430-124">`NoApproval`Используется при `isApprovalRequired` значении false.</span><span class="sxs-lookup"><span data-stu-id="54430-124">The `NoApproval` is used when `isApprovalRequired` is false.</span></span> |
| <span data-ttu-id="54430-125">аппровалстажес</span><span class="sxs-lookup"><span data-stu-id="54430-125">approvalStages</span></span> | <span data-ttu-id="54430-126">Коллекция [аппровалстаже](approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="54430-126">[approvalStage](approvalstage.md) collection</span></span>| <span data-ttu-id="54430-127">Если необходимо утверждение, то один или два элемента этой коллекции определяют каждый из стадий утверждения.</span><span class="sxs-lookup"><span data-stu-id="54430-127">If approval is required, the one or two elements of this collection define each of the stages of approval.</span></span> <span data-ttu-id="54430-128">Пустой массив, если утверждение не нужно.</span><span class="sxs-lookup"><span data-stu-id="54430-128">An empty array if no approval is required.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="54430-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54430-129">JSON representation</span></span>

<span data-ttu-id="54430-130">Ниже приведено представление свойства параметров утверждения запроса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54430-130">The following is a JSON representation of the request approval settings property.</span></span>

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


