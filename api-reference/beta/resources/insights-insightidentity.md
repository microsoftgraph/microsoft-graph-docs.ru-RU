---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fee67727e610e44ab8cfcf15f973160310575136
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495874"
---
# <a name="insightidentity"></a><span data-ttu-id="a3d45-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="a3d45-103">insightIdentity</span></span>

<span data-ttu-id="a3d45-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a3d45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3d45-105">Сложный тип, содержащий свойства элементов [шарединсигхт](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="a3d45-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="a3d45-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3d45-106">JSON representation</span></span>
<span data-ttu-id="a3d45-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="a3d45-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a3d45-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3d45-108">Properties</span></span>

| <span data-ttu-id="a3d45-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3d45-109">Property</span></span>              | <span data-ttu-id="a3d45-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a3d45-110">Type</span></span>          | <span data-ttu-id="a3d45-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a3d45-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="a3d45-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a3d45-112">displayName</span></span>       | <span data-ttu-id="a3d45-113">Строка</span><span class="sxs-lookup"><span data-stu-id="a3d45-113">String</span></span>          | <span data-ttu-id="a3d45-114">Отображаемое имя пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="a3d45-114">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="a3d45-115">id</span><span class="sxs-lookup"><span data-stu-id="a3d45-115">id</span></span>              | <span data-ttu-id="a3d45-116">String</span><span class="sxs-lookup"><span data-stu-id="a3d45-116">String</span></span>        | <span data-ttu-id="a3d45-117">Идентификатор пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="a3d45-117">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="a3d45-118">address</span><span class="sxs-lookup"><span data-stu-id="a3d45-118">address</span></span>             | <span data-ttu-id="a3d45-119">String</span><span class="sxs-lookup"><span data-stu-id="a3d45-119">String</span></span>      | <span data-ttu-id="a3d45-120">Адрес электронной почты пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="a3d45-120">The email address of the user who shared the item.</span></span>  |
