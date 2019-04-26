---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 45ac8874a30ebb4f3196f03a675229bf1fab750c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549575"
---
# <a name="insightidentity"></a><span data-ttu-id="2e3c9-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="2e3c9-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e3c9-104">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="2e3c9-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="2e3c9-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e3c9-105">JSON representation</span></span>
<span data-ttu-id="2e3c9-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="2e3c9-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="2e3c9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e3c9-107">Properties</span></span>

| <span data-ttu-id="2e3c9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e3c9-108">Property</span></span>              | <span data-ttu-id="2e3c9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2e3c9-109">Type</span></span>          | <span data-ttu-id="2e3c9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e3c9-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="2e3c9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2e3c9-111">displayName</span></span>       | <span data-ttu-id="2e3c9-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2e3c9-112">String</span></span>          | <span data-ttu-id="2e3c9-113">Отображаемое имя пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="2e3c9-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="2e3c9-114">id</span><span class="sxs-lookup"><span data-stu-id="2e3c9-114">id</span></span>              | <span data-ttu-id="2e3c9-115">String</span><span class="sxs-lookup"><span data-stu-id="2e3c9-115">String</span></span>        | <span data-ttu-id="2e3c9-116">Идентификатор пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="2e3c9-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="2e3c9-117">address</span><span class="sxs-lookup"><span data-stu-id="2e3c9-117">address</span></span>             | <span data-ttu-id="2e3c9-118">String</span><span class="sxs-lookup"><span data-stu-id="2e3c9-118">String</span></span>      | <span data-ttu-id="2e3c9-119">Адрес электронной почты пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="2e3c9-119">The email address of the user who shared the item.</span></span>  |
