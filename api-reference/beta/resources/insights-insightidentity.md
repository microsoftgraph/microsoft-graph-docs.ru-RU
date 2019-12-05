---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 439b64cca61c6324aa72e5f4c845f1bd1598230b
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844981"
---
# <a name="insightidentity"></a><span data-ttu-id="2ad54-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="2ad54-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ad54-104">Сложный тип, содержащий свойства элементов [шарединсигхт](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="2ad54-104">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="2ad54-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ad54-105">JSON representation</span></span>
<span data-ttu-id="2ad54-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="2ad54-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="2ad54-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ad54-107">Properties</span></span>

| <span data-ttu-id="2ad54-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ad54-108">Property</span></span>              | <span data-ttu-id="2ad54-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2ad54-109">Type</span></span>          | <span data-ttu-id="2ad54-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2ad54-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="2ad54-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2ad54-111">displayName</span></span>       | <span data-ttu-id="2ad54-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2ad54-112">String</span></span>          | <span data-ttu-id="2ad54-113">Отображаемое имя пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="2ad54-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="2ad54-114">id</span><span class="sxs-lookup"><span data-stu-id="2ad54-114">id</span></span>              | <span data-ttu-id="2ad54-115">String</span><span class="sxs-lookup"><span data-stu-id="2ad54-115">String</span></span>        | <span data-ttu-id="2ad54-116">Идентификатор пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="2ad54-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="2ad54-117">address</span><span class="sxs-lookup"><span data-stu-id="2ad54-117">address</span></span>             | <span data-ttu-id="2ad54-118">String</span><span class="sxs-lookup"><span data-stu-id="2ad54-118">String</span></span>      | <span data-ttu-id="2ad54-119">Адрес электронной почты пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="2ad54-119">The email address of the user who shared the item.</span></span>  |
