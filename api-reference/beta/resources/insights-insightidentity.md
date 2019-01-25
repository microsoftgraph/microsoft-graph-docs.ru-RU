---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 45ac8874a30ebb4f3196f03a675229bf1fab750c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523059"
---
# <a name="insightidentity"></a><span data-ttu-id="bfaab-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="bfaab-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfaab-104">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="bfaab-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="bfaab-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfaab-105">JSON representation</span></span>
<span data-ttu-id="bfaab-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="bfaab-106">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="bfaab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfaab-107">Properties</span></span>

| <span data-ttu-id="bfaab-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfaab-108">Property</span></span>              | <span data-ttu-id="bfaab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bfaab-109">Type</span></span>          | <span data-ttu-id="bfaab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bfaab-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="bfaab-111">displayName</span><span class="sxs-lookup"><span data-stu-id="bfaab-111">displayName</span></span>       | <span data-ttu-id="bfaab-112">String</span><span class="sxs-lookup"><span data-stu-id="bfaab-112">String</span></span>          | <span data-ttu-id="bfaab-113">Отображаемое имя пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="bfaab-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="bfaab-114">id</span><span class="sxs-lookup"><span data-stu-id="bfaab-114">id</span></span>              | <span data-ttu-id="bfaab-115">Строка</span><span class="sxs-lookup"><span data-stu-id="bfaab-115">String</span></span>        | <span data-ttu-id="bfaab-116">Идентификатор пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="bfaab-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="bfaab-117">address</span><span class="sxs-lookup"><span data-stu-id="bfaab-117">address</span></span>             | <span data-ttu-id="bfaab-118">String</span><span class="sxs-lookup"><span data-stu-id="bfaab-118">String</span></span>      | <span data-ttu-id="bfaab-119">Адрес электронной почты пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="bfaab-119">The email address of the user who shared the item.</span></span>  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
