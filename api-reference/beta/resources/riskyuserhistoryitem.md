---
title: тип ресурса riskyUserHistoryItem
description: Представляет историю рисков пользователей Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4ae6d5fbc28e8dddb4c782aa9e9b2fad79b347ad
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442859"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="bff50-103">тип ресурса riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="bff50-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="bff50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bff50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="bff50-105">Представляет историю рисков пользователя Azure AD, определяемую службой Azure AD Identity Protection.</span><span class="sxs-lookup"><span data-stu-id="bff50-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="bff50-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bff50-106">Methods</span></span>

| <span data-ttu-id="bff50-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bff50-107">Method</span></span>   | <span data-ttu-id="bff50-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bff50-108">Return Type</span></span>|<span data-ttu-id="bff50-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bff50-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bff50-110">История списка</span><span class="sxs-lookup"><span data-stu-id="bff50-110">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="bff50-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="bff50-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="bff50-112">Получите историю рисков пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bff50-112">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="bff50-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="bff50-113">Properties</span></span>

| <span data-ttu-id="bff50-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="bff50-114">Property</span></span>       | <span data-ttu-id="bff50-115">Тип</span><span class="sxs-lookup"><span data-stu-id="bff50-115">Type</span></span>    | <span data-ttu-id="bff50-116">Описание</span><span class="sxs-lookup"><span data-stu-id="bff50-116">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="bff50-117">userId</span><span class="sxs-lookup"><span data-stu-id="bff50-117">userId</span></span>         | <span data-ttu-id="bff50-118">строка</span><span class="sxs-lookup"><span data-stu-id="bff50-118">string</span></span>  | <span data-ttu-id="bff50-119">ID пользователя.</span><span class="sxs-lookup"><span data-stu-id="bff50-119">The id of the user.</span></span> |
| <span data-ttu-id="bff50-120">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="bff50-120">initiatedBy</span></span>    | <span data-ttu-id="bff50-121">bool</span><span class="sxs-lookup"><span data-stu-id="bff50-121">bool</span></span>    | <span data-ttu-id="bff50-122">ID субъекта, который делает операцию.</span><span class="sxs-lookup"><span data-stu-id="bff50-122">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="bff50-123">действие</span><span class="sxs-lookup"><span data-stu-id="bff50-123">activity</span></span>       | [<span data-ttu-id="bff50-124">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="bff50-124">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="bff50-125">Действие, связанное с изменением уровня риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="bff50-125">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="bff50-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bff50-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "string",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyUserHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->


