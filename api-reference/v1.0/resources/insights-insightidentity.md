---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: f4b8bc6b66598753c0755d249ab37283810e8db7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054870"
---
# <a name="insightidentity"></a><span data-ttu-id="d285c-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="d285c-103">insightIdentity</span></span>

<span data-ttu-id="d285c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d285c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d285c-105">Сложный тип, содержащий свойства элементов [шарединсигхт](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="d285c-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="d285c-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d285c-106">JSON representation</span></span>
<span data-ttu-id="d285c-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d285c-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d285c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d285c-108">Properties</span></span>

| <span data-ttu-id="d285c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d285c-109">Property</span></span>              | <span data-ttu-id="d285c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d285c-110">Type</span></span>          | <span data-ttu-id="d285c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d285c-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="d285c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d285c-112">displayName</span></span>       | <span data-ttu-id="d285c-113">String</span><span class="sxs-lookup"><span data-stu-id="d285c-113">String</span></span>          | <span data-ttu-id="d285c-114">Отображаемое имя пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="d285c-114">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="d285c-115">id</span><span class="sxs-lookup"><span data-stu-id="d285c-115">id</span></span>              | <span data-ttu-id="d285c-116">String</span><span class="sxs-lookup"><span data-stu-id="d285c-116">String</span></span>        | <span data-ttu-id="d285c-117">Идентификатор пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="d285c-117">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="d285c-118">address</span><span class="sxs-lookup"><span data-stu-id="d285c-118">address</span></span>             | <span data-ttu-id="d285c-119">String</span><span class="sxs-lookup"><span data-stu-id="d285c-119">String</span></span>      | <span data-ttu-id="d285c-120">Адрес электронной почты пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="d285c-120">The email address of the user who shared the item.</span></span>  |

