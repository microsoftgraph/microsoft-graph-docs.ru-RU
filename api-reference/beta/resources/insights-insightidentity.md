---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8718ab248dada75f04d92d6a8717dd4f43ee8106
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333598"
---
# <a name="insightidentity"></a><span data-ttu-id="9ef41-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="9ef41-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ef41-104">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="9ef41-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="9ef41-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ef41-105">JSON representation</span></span>
<span data-ttu-id="9ef41-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="9ef41-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="9ef41-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ef41-107">Properties</span></span>

| <span data-ttu-id="9ef41-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ef41-108">Property</span></span>              | <span data-ttu-id="9ef41-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9ef41-109">Type</span></span>          | <span data-ttu-id="9ef41-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9ef41-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="9ef41-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9ef41-111">displayName</span></span>       | <span data-ttu-id="9ef41-112">Строка</span><span class="sxs-lookup"><span data-stu-id="9ef41-112">String</span></span>          | <span data-ttu-id="9ef41-113">Отображаемое имя пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="9ef41-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="9ef41-114">id</span><span class="sxs-lookup"><span data-stu-id="9ef41-114">id</span></span>              | <span data-ttu-id="9ef41-115">String</span><span class="sxs-lookup"><span data-stu-id="9ef41-115">String</span></span>        | <span data-ttu-id="9ef41-116">Идентификатор пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="9ef41-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="9ef41-117">address</span><span class="sxs-lookup"><span data-stu-id="9ef41-117">address</span></span>             | <span data-ttu-id="9ef41-118">String</span><span class="sxs-lookup"><span data-stu-id="9ef41-118">String</span></span>      | <span data-ttu-id="9ef41-119">Адрес электронной почты пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="9ef41-119">The email address of the user who shared the item.</span></span>  |
