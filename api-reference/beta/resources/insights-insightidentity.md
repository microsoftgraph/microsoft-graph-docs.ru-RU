---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 6b5a4b3c6e43f0314860935af810d20d91663c96
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005753"
---
# <a name="insightidentity"></a><span data-ttu-id="f922e-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="f922e-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f922e-104">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="f922e-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="f922e-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f922e-105">JSON representation</span></span>
<span data-ttu-id="f922e-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f922e-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="f922e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f922e-107">Properties</span></span>

| <span data-ttu-id="f922e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f922e-108">Property</span></span>              | <span data-ttu-id="f922e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f922e-109">Type</span></span>          | <span data-ttu-id="f922e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f922e-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="f922e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f922e-111">displayName</span></span>       | <span data-ttu-id="f922e-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f922e-112">String</span></span>          | <span data-ttu-id="f922e-113">Отображаемое имя пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="f922e-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="f922e-114">id</span><span class="sxs-lookup"><span data-stu-id="f922e-114">id</span></span>              | <span data-ttu-id="f922e-115">String</span><span class="sxs-lookup"><span data-stu-id="f922e-115">String</span></span>        | <span data-ttu-id="f922e-116">Идентификатор пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="f922e-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="f922e-117">address</span><span class="sxs-lookup"><span data-stu-id="f922e-117">address</span></span>             | <span data-ttu-id="f922e-118">String</span><span class="sxs-lookup"><span data-stu-id="f922e-118">String</span></span>      | <span data-ttu-id="f922e-119">Адрес электронной почты пользователя, который предоставил общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="f922e-119">The email address of the user who shared the item.</span></span>  |
