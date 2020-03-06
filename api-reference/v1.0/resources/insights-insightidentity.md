---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3a23344a18979c7d1aa69b8e841007812797b238
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531299"
---
# <a name="insightidentity"></a><span data-ttu-id="d9bcd-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="d9bcd-103">insightIdentity</span></span>

<span data-ttu-id="d9bcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9bcd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9bcd-105">Сложный тип, содержащий свойства элементов [шарединсигхт](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="d9bcd-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="d9bcd-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9bcd-106">JSON representation</span></span>
<span data-ttu-id="d9bcd-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d9bcd-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d9bcd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9bcd-108">Properties</span></span>

| <span data-ttu-id="d9bcd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9bcd-109">Property</span></span>              | <span data-ttu-id="d9bcd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d9bcd-110">Type</span></span>          | <span data-ttu-id="d9bcd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d9bcd-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="d9bcd-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d9bcd-112">displayName</span></span>       | <span data-ttu-id="d9bcd-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d9bcd-113">String</span></span>          | <span data-ttu-id="d9bcd-114">Отображаемое имя пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="d9bcd-114">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="d9bcd-115">id</span><span class="sxs-lookup"><span data-stu-id="d9bcd-115">id</span></span>              | <span data-ttu-id="d9bcd-116">String</span><span class="sxs-lookup"><span data-stu-id="d9bcd-116">String</span></span>        | <span data-ttu-id="d9bcd-117">Идентификатор пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="d9bcd-117">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="d9bcd-118">address</span><span class="sxs-lookup"><span data-stu-id="d9bcd-118">address</span></span>             | <span data-ttu-id="d9bcd-119">String</span><span class="sxs-lookup"><span data-stu-id="d9bcd-119">String</span></span>      | <span data-ttu-id="d9bcd-120">Адрес электронной почты пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="d9bcd-120">The email address of the user who shared the item.</span></span>  |
